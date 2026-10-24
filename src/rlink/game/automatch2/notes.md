# AoE2:DE Automatch2 — implementation notes

These notes come from building a **minimal 1v1 Automatch2** implementation in a
local RLink-compatible server ([ageLANServer](https://github.com/luskaner/ageLANServer))
and testing it with two AoE2:DE clients. They are intended to complement the
endpoint pages in this section with observed client behaviour and protocol
details that are easy to miss.

> These findings are empirical. They describe the client build tested in
> October 2026; other versions may differ.

## End-to-end flow observed

1. The client calls `GET /game/automatch2/getAutomatchMap`.
2. The client calls `POST /game/automatch2/polling` repeatedly. It sends several
   `matchTypes`; 1v1 queues may arrive as `1`, `6` or `20`.
3. When two compatible players are queued, the server returns a *matched*
   polling response containing the host profile ID, map, peers, BattleServer
   address/ports and an advertisement ID.
4. The **host** receives the matched response **before the advertisement
   exists**. It then creates the advertisement by calling
   `POST /game/advertisement/update` with the reserved advertisement ID.
   AoE2:DE does **not** use `/advertisement/host` for this flow.
5. The joiner keeps polling until the advertisement exists and then receives the
   real matched response.
6. The server notifies the joiner over WSS with an `Automatch2GameMessage`.
7. Both clients connect to the relay using the BattleServer address.

## Polling response notes

- Field `1` is the **elapsed wait time in seconds**, not a state enum.
- Field `4` is the **host profile ID** (`match.HostID`). The host should compare
  it with its own profile before starting the host flow.
- Peer/relay addresses must be resolved **per request** from the local address
  that client used to reach the server. Using a synthetic advertisement IP such
  as `/10.0.11.x` here makes the client try to resolve it as a hostname and fail.
- `getProfileName?profile_ids=[-1]` may appear during a join. It was also
  observed in working flows and is not by itself evidence of a bad host ID.

## `Automatch2GameMessage` (WSS)

The payload is a JSON **object** with named keys, including:

```json
{
    "hostProfileID": 123,
    "matchID": 456,
    "mapName": "Arabia.rms",
    "raceID": 0,
    "teamID": 1,
    "factionID": 0,
    "teamCount": 2,
    "maxPlayersPerTeam": 1,
    "relayAuthToken": "authtoken",
    "relayIP": "192.168.1.10",
    "relayPortRaw": 6079,
    "relayPortWebSockets": 6080,
    "relayPortOutOfBandSocket": 6081,
    "matchMembers": [
        {
            "sessionID": 123,
            "profileID": 123,
            "statGroupID": 456,
            "raceID": 0,
            "teamID": 0,
            "ranking": 0,
            "url": "192.168.1.10"
        },
        {
            "sessionID": 789,
            "profileID": 789,
            "statGroupID": 987,
            "raceID": 0,
            "teamID": 1,
            "ranking": 0,
            "url": ""
        }
    ],
    "options": ""
}
```

`matchMembers` entries are objects, not positional arrays. The host member's
`url` is the host relay address; joiner members normally have an empty `url`.

## Advertisement notes (AoE2:DE)

- An ordinary party/session host uses description `SESSION_MATCH_KEY`,
  `matchtype=1`, `maxplayers=4` and an empty map. It is **not** an automatch.
- Automatch advertisements use `matchtype=19` and/or a positive
  `automatchPoll_id`. The implementation sets `matchtype=19`, forces the 1v1
  map/max-player values, keeps the ad joinable, and preserves those fields when
  the host sends later updates.
- Automatch joins should bypass the random advertisement password; teams are
  assigned by the polling response, not by the advertisement peer team field.
- `updatePlatformLobbyID` may return `[0]` for a pending automatch session
  instead of an error.
- Store the platform session ID before the advertisement exists and copy it in
  when the advertisement is created.
- **Field count matters.** In our tests the current client rejected the 24-field
  advertisement layout with `WorldwideUpdateAdvertisementAsync - response was
  not formatted correctly` and `AdvertisementByIDCache - response was not
  formatted correctly`, for both ordinary and automatch advertisements. A
  27-field layout was accepted. See the note added to
  [getAdvertisements](../advertisement/getadvertisements.md).

## Minimal 1v1 rules used

- Accept aliases `20`, `6` and `1`; expose canonical queue/leaderboard `6`.
- Maximum 2 players, team size 1, map `Arabia.rms`.
- Pair the earliest queued host with the next compatible player.
- Reserve the match ID as the future advertisement ID.
- Host timeout: about 45 seconds while waiting for the advertisement.
- On cancel/failure, clean up the match and decide explicitly whether players
  are requeued. The current simple implementation requeues on host failure;
  this is a policy choice, not a protocol requirement.

## Ideas for future work

This minimal implementation is intentionally simple. The protocol leaves room
for:

- MMR/skill-based pairing and real leaderboard/rating updates.
- Multiple maps, map pools and queue types (team games, unranked, etc.).
- Host migration, better cancellation and retry policy.
- Region-aware BattleServer selection and NAT/relay fallback.
- Richer validation of `matchTypes`, races and party state.
- More robust handling of client-version differences in the advertisement and
  GameMessage formats.

## Reference implementation

- [ageLANServer](https://github.com/luskaner/ageLANServer) (upstream)
- Example fork/PR: [Chichimokers/ageLANServer PR #1](https://github.com/Chichimokers/ageLANServer/pull/1)
