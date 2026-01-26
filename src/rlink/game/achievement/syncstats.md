# [POST] /game/achievement/syncStats (Missing Response)

**AUTHENTICATION**

Response

## AoE2:DE

### Request

```
POST /game/achievement/syncStats HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 136
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

accountType=STEAM&auth=&callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| accountType  | str/enum  | STEAM |          |
| auth         | token     | ?     |          |
| callNum      | int       | 123   |          |
| connect_id   | str       | ccc   |          |
| lastCallTime | timestamp | 111   |          |
| sessionID    | str       | zzz   |          |

### Response

```
RESPONSE_TEMPLATE
```

## AoE4

### Request

```
POST /game/achievement/syncStats HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 137
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

accountType=STEAM&auth=&callNum=87&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=328366&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| accountType  | str/enum  | STEAM |          |
| auth         | token     | ?     |          |
| callNum      | int       | 123   |          |
| connect_id   | str       | ccc   |          |
| lastCallTime | timestamp | 111   |          |
| sessionID    | str       | zzz   |          |

### Response

```
[
    0 // result status code
]
```
