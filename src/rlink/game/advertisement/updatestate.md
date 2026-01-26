# [POST] /game/advertisement/updateState (Missing Response)

**AUTHENTICATION**

Response

## AoE2:DE

### Request

```
POST /game/advertisement/updateState HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 146
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

advertisementid=1&callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz&state=1
```

| parameter       | type      | value | comments |
| --------------- | --------- | ----- | -------- |
| advertisementid | int       | 1     |          |
| callNum         | int       | 123   |          |
| connect_id      |           |       |          |
| lastCallTime    | timestamp | 111   |          |
| sessionID       | str       |       |          |

### Response

```
RESPONSE_TEMPLATE
```
