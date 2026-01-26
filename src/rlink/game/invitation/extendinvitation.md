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
    2 // result status code
]
```
