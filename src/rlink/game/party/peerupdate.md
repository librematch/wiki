# [POST] /game/party/peerUpdate (Missing Response)

**AUTHENTICATION**

Response

## AoE2:DE

### Request

```
POST /game/party/peerUpdate HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 247
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

callNum=123&connect_id=ccc&isNonParticipants=[0,0]&lastCallTime=111&match_id=555&profile_ids=[1,1]&race_ids=[1,2,3]&sessionID=zzz&teamIDs=[0,1]
```

| parameter         | type       | value   | comments |
| ----------------- | ---------- | ------- | -------- |
| callNum           | int        | 123     |          |
| connect_id        |            |         |          |
| isNonParticipants | array[int] | [0,0]   |          |
| lastCallTime      | timestamp  |         |          |
| match_id          | int        | 555     |          |
| profile_ids       | array[int] | [1,1]   |          |
| race_ids          | array[int] | [1,2,3] |          |
| sessionID         | str        | zzz     |          |
| teamIDs           | array      | [0,1]   |          |

### Response

```
RESPONSE_TEMPLATE
```
