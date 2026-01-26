# [POST] /game/party/sendMatchChat

**AUTHENTICATION**

## AoE2DE

### Request

```
POST /game/party/sendMatchChat HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 229
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

broadcast=0&callNum=150&connect_id=ebyb0gp9rsvu863i501263m9wjly55&lastCallTime=2616898&match_id=186444398&message=0*gg&messageTypeID=0&sessionID=ebyb0gp9rsvu863i501263m9wjly55
```

| parameter     | type      | value    | comments             |
| ------------- | --------- | -------- | -------------------- |
| broadcast     | int       | 1        | aoe4: 1, aoe2de: 0 ? |
| callNum       | int       | 123      |                      |
| connect_id    | str       | ccc      |                      |
| lastCallTime  | timestamp | 111      |                      |
| match_id      | int       | 555      |                      |
| message       | str       | dummymsg |                      |
| messageTypeID | int       | 2        |                      |
| sessionID     | str       | zzz      |                      |

### Response

```
[
   0 // result status code
]
```

## AoE4

### Request

```
POST /game/party/sendMatchChat HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 229
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

broadcast=1&callNum=123&connect_id=ccc&from_profile_id=111&lastCallTime=111&match_id=555&message=dummymsg&messageTypeID=2&sessionID=zzz&to_profile_id=222
```

| parameter       | type      | value    | comments             |
| --------------- | --------- | -------- | -------------------- |
| broadcast       | int       | 1        | aoe4: 1, aoe2de: 0 ? |
| callNum         | int       | 123      |                      |
| connect_id      | str       | ccc      |                      |
| from_profile_id | int       | 111      | only AoE4            |
| lastCallTime    | timestamp | 111      |                      |
| match_id        | int       | 555      |                      |
| message         | str       | dummymsg |                      |
| messageTypeID   | int       | 2        |                      |
| sessionID       | str       | zzz      |                      |
| to_profile_id   | id        | 222      | only AoE4            |

### Response

```
[
   0 // result status code
]
```
