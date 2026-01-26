# [POST] /game/advertisement/leave

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/advertisement/leave HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 137
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

advertisementid=1&callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz
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
[
    0 // result status code
]
```

## AoE4

### Request

```
POST /game/advertisement/leave HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 140
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

advertisementid=50864995&callNum=317&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=3087885&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19
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
[
    0 // result status code
]
```
