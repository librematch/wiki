# [POST] /game/account/setLanguage

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/account/setLanguage HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 135

callNum=31&connect_id=6mikb1saqrmud2kte7ovswogamd2th&language=en&lastCallTime=15557&sessionID=6mikb1saqrmud2kte7ovswogamd2th&title=age2
```

| parameter    | type       | value | comments |
| ------------ | ---------- | ----- | -------- |
| callNum      | int        | 123   |          |
| connect_id   |            |       |          |
| language     | ISO CODE   | en    |          |
| lastCallTime | timestamp  |       |          |
| sessionID    | str        |       |          |
| title        | enum(game) | age2  |          |

### Response

```
[
   0 // result status code
]
```
