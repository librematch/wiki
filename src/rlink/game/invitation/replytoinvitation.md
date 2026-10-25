# [POST] /game/invitation/replyToInvitation

**AUTHENTICATION**

Answer sent by the invitee after the client shows the invitation. The server
relays it to the inviter over WSS (`ReplyInvitationMessage`).

## AoE2:DE

### Request

```
POST /game/invitation/replyToInvitation HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
Pragma: no-cache

callNum=61&connect_id=yam8gu2dsn23p8fazf6oycimo3433p&gatheringid=150963865&invitationreply=0&inviterid=2092636891&sessionID=yam8gu2dsn23p8fazf6oycimo3433p
```

| parameter       | type | value      | comments                                                             |
| --------------- | ---- | ---------- | -------------------------------------------------------------------- |
| callNum         | int  | 61         |                                                                      |
| connect_id      | str  |            |                                                                      |
| gatheringid     | int  | 150963865  | Advertisement ID of the party/lobby, the same sent in the invitation |
| invitationreply | int  | 0          | Reply code, see the note below                                       |
| inviterid       | int  | 2092636891 | Profile ID of the inviter (not the stat group ID)                    |
| sessionID       | str  |            |                                                                      |

No `lastCallTime` was present in the captured request.

### Response

```
[
    0 // result status code: 0 = success, 2 = error
]
```

### Notes

- This endpoint is missing from the endpoint tables of older captures, but the
  client calls it on every invitation answer: without it the inviter never sees
  the answer and the invitee stops before joining.
- `invitationreply` polarity is not obvious. In our captures the client sent
  `0` when the user **accepted** and then joined the party, so `0` cannot be
  assumed to mean "decline". We did not capture a rejection.
- The server forwards the answer to the inviter as a **string** in
  `ReplyInvitationMessage` (`"1"` for accept, `"0"` otherwise in our
  implementation). See the [invitation flow notes](./notes.md).
- After a successful reply the invitee normally calls
  `advertisement/getAdvertisements?match_ids=[gatheringid]` and then
  `advertisement/join`; the inviter receives `party/peerAdd` and
  `advertisement/update` for the new member.
