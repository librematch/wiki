# AoE2:DE party invitations - observed flow

These notes come from capturing a full party invitation between two AoE2:DE
clients connected to a local RLink-compatible server
([ageLANServer](https://github.com/luskaner/ageLANServer)). They describe what
the client actually sends, so a server can reproduce the flow without
implementing Steam friends.

> Empirical, from the PC client build tested in October 2026. Other versions may
> differ.

## Short version

Invitations are **pure RLink**: the client searches profiles, calls
`invitation/extendInvitation`, and the invitee answers with
`invitation/replyToInvitation`. The party itself is an ordinary advertisement
with `matchtype=1`. Steam is only used for the platform session ID; no Steam
friend list, lobby or `InviteUserToGame` call is involved, so a Steam emulator
without friends still works.

## Captured sequence

Profile IDs in the examples: host `2092636891`, invitee `1232055058`, gathering
`150963865`.

| #  | Who     | Endpoint                                                          | Relevant payload                                                                                                                                                                   |
| -- | ------- | ----------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1  | host    | `POST /game/advertisement/host`                                   | `advertisementid=-1`, `description=SESSION_MATCH_KEY`, `matchtype=1`, `maxplayers=4`, `mapname=`, `visible=0`, `joinable=1`, `passworded=0`, `party=-1`, `team=-1`, `statgroup=-1` |
| 2  | host    | `POST /game/party/peerAdd`                                        | `match_id=150963865`, `profile_ids=[2092636891]`, `race_ids=[0]`, `teamIDs=[-1]`                                                                                                   |
| 3  | host    | `POST /game/advertisement/updatePlatformSessionID`                | `matchID=150963865`, `onlinePlatform=STEAM`, `platformSessionID=...`                                                                                                               |
| 4  | host    | `POST /game/advertisement/update`                                 | same advertisement fields as step 1                                                                                                                                                |
| 5  | host    | `GET /game/account/FindProfiles?name=c`                           | called twice, with `c` and `C` (the client re-queries as the text changes)                                                                                                         |
| 6  | host    | `POST /game/invitation/extendInvitation`                          | `gatheringid=150963865`, `gatheringpassword=`, `inviteeid=1232055058`                                                                                                              |
| 7  | server  | WSS to invitee                                                    | `ExtendInvitationMessage`                                                                                                                                                          |
| 8  | invitee | `GET /game/advertisement/getAdvertisements?match_ids=[150963865]` |                                                                                                                                                                                    |
| 9  | invitee | `GET /game/account/getProfileName?profile_ids=[-1]`               | also seen in working flows, not an error by itself                                                                                                                                 |
| 10 | invitee | `POST /game/invitation/replyToInvitation`                         | `gatheringid=150963865`, `invitationreply=0`, `inviterid=2092636891`                                                                                                               |
| 11 | server  | WSS to inviter                                                    | `ReplyInvitationMessage`                                                                                                                                                           |
| 12 | invitee | `POST /game/advertisement/join`                                   | `advertisementid=150963865`, `party=-1`, `team=-1`, `statgroup=-1`, `race=-1`, `password=`                                                                                         |
| 13 | host    | `POST /game/party/peerAdd`                                        | `match_id=150963865`, `profile_ids=[1232055058]`, `teamIDs=[-1]`                                                                                                                   |
| 14 | host    | `POST /game/advertisement/update`                                 | advertisement now has two peers                                                                                                                                                    |

The advertisement ID returned by `advertisement/host` (here `150963865`) is the
`gatheringid` used by every invitation call and by `party/peerAdd` as
`match_id`.

## WSS messages

The invitation notifications are positional arrays, like most RLink WSS
payloads:

```jsonc
// ExtendInvitationMessage, sent to the invitee
[
    [ /* inviter profileInfo */ ],  // same shape as the profileInfo in the leaderboard responses
    150963865,                      // gatheringid
    ""                              // gathering password (empty when not passworded)
]

// ReplyInvitationMessage, sent to the inviter
[
    [ /* invitee profileInfo */ ],
    150963865,
    "1"                             // answer as a string: "1" accept, "0" otherwise
]
```

The invitee must receive `ExtendInvitationMessage` for the invitation popup to
appear; the inviter must receive `ReplyInvitationMessage` to update the party
UI.

## Parameters and gotchas

- `inviteeid` and `inviterid` are **profile IDs**, not platform user IDs and not
  stat group IDs. `statGroup_ids` appears only in `party/peerAdd`.
- `extendInvitation` is validated server-side against the gathering: it must
  exist, the `gatheringpassword` must match, and the caller must already be a
  peer of it. In our implementation any failure returns `[2]`; a successful
  call returns `[0]` (the sample in
  [extendInvitation](./extendinvitation.md) shows the error form).
- `FindProfiles` is the invite dialog's search. Our server matches aliases
  case-insensitively as a substring and returns **every** matching user,
  including the caller and offline profiles. The client does not need a Steam
  friend list to invite.
- `advertisement/join` for a party is the normal join endpoint with
  `party=-1`, `team=-1`, `statgroup=-1` and `race=-1`. Teams are not assigned by
  the party advertisement.
- Members are added with `teamIDs=[-1]` while the party is only a lobby. A
  later game start assigns real teams.
- `advertisement/updatePlatformSessionID` carries the Steam lobby/session ID
  (`onlinePlatform=STEAM`). A local server can accept and store it; the
  invitation flow keeps working without it as long as the advertisement exists.
- The party advertisement is also what the client uses as its session when it
  opens the matchmaking screen, so the `partySessionID` sent by
  `automatch2/polling` is a real ID even for a solo player (see
  [polling](../automatch2/polling.md)).
