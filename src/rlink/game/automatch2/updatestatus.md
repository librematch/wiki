# [POST] /game/automatch2/updateStatus

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/automatch2/updateStatus HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 152
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

callNum=123&connect_id=ccc&lastCallTime=111&matchID=555&result=1&resultCode=0&sessionID=zzz
```

| parameter    | type     | value | comments |
| ------------ | -------- | ----- | -------- |
| callNum      | int      | 123   |          |
| connect_id   | str      | ccc   |          |
| lastCallTime | int      | 111   |          |
| matchID      | int      | 555   |          |
| result       | int      | 1     |          |
| resultCode   | int/bool | 0     |          |
| sessionID    | str      | zzz   |          |

### Response

```
[
    0, // result status code
    0
]
```
