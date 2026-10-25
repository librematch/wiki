# [POST] /game/invitation/extendInvitation

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/invitation/extendInvitation HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 172
```

| parameter         | type      | value | comments |
| ----------------- | --------- | ----- | -------- |
| callNum           | int       | 123   |          |
| connect_id        | str       |       |          |
| gatheringid       | int       |       |          |
| gatheringpassword | str       |       |          |
| inviteeid         | int       |       |          |
| lastCallTime      | timestamp |       |          |
| sessionID         | str       |       |          |

### Response

```
[
    0 // result status code: 0 = success, 2 = error
]
```

The sample above is the error form. A successful invitation returns `[0]` and
the invitee receives a WSS `ExtendInvitationMessage` with
`[inviterProfileInfo, gatheringid, gatheringpassword]`.

### Notes

- The server must validate that the gathering exists, that `gatheringpassword`
  matches and that the caller is already a peer of it. The invitee is identified
  by **profile ID** (`inviteeid`), not by platform user ID.
- The answer comes back through
  [replyToInvitation](./replytoinvitation.md); see the
  [invitation flow notes](./notes.md) for the full captured sequence.
