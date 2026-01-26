# [POST] /game/challenge/updateProgressBatched (Missing Response)

**AUTHENTICATION**

Response

## AoE2:DE

### Request

```
POST /game/challenge/updateProgressBatched HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 162
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

callNum=123&connect_id=ccc&lastCallTime=111&progressIDs=[999]&sessionID=zzz&updateAmounts=[1]
```

| parameter     | type       | value | comments |
| ------------- | ---------- | ----- | -------- |
| callNum       | int        | 123   |          |
| connect_id    |            |       |          |
| lastCallTime  | timestamp  |       |          |
| progressIDs   | array[int] | [999] |          |
| sessionID     | str        |       |          |
| updateAmounts | array[int] | [1]   |          |

### Response

```
[
    0 // result status code
]
```

## AoE4

### Request

```
POST /game/challenge/updateProgressBatched HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 164
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=86&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=327549&progressIDs=[646542981]&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&updateAmounts=[12]
```

| parameter     | type       | value | comments |
| ------------- | ---------- | ----- | -------- |
| callNum       | int        | 123   |          |
| connect_id    |            |       |          |
| lastCallTime  | timestamp  |       |          |
| progressIDs   | array[int] | [999] |          |
| sessionID     | str        |       |          |
| updateAmounts | array[int] | [1]   |          |

### Response

```
[
    0 // result status code
]
```
