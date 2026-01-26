# [POST] /game/chat/deleteOfflineMessage (Missing Response)

**AUTHENTICATION**

Response

## AoE2:DE

### Request

```
POST /game/chat/deleteOfflineMessage HTTP/1.1
Cookie: ApplicationGatewayAffinity=d0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 131
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| callNum      | int       | 123   |          |
| connect_id   |           |       |          |
| lastCallTime | timestamp |       |          |
| messageID    | int       |       |          |
| sessionID    | str       |       |          |

### Response

```
[
    0 // result status code
]
```

## AoE4

### Request

```
POST /game/chat/deleteOfflineMessage HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 131
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=47&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=24061&messageID=70218256&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| callNum      | int       | 123   |          |
| connect_id   |           |       |          |
| lastCallTime | timestamp |       |          |
| messageID    | int       |       |          |
| sessionID    | str       |       |          |

### Response

```
[
    0 // result status code
]
```
