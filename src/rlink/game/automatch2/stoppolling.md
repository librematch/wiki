# [POST] /game/automatch2/stoppolling

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/automatch2/stoppolling HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 144
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

callNum=123&commit=0&connect_id=ccc&lastCallTime=111&ownerProfileID=444&sessionID=zzz
```

| parameter      | type     | value | comments |
| -------------- | -------- | ----- | -------- |
| callNum        | int      | 123   |          |
| commit         | int/bool | 0     |          |
| connect_id     | str      | ccc   |          |
| lastCallTime   | int      | 111   |          |
| ownerProfileID | int      | 444   |          |
| sessionID      | str      | zzz   |          |

### Response

```
[
    0 // result status code
]
```

## AoE4

### Request

```
POST /game/automatch2/stoppolling HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 146
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=279&commit=0&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=3028904&ownerProfileID=233334&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19
```

| parameter      | type     | value | comments |
| -------------- | -------- | ----- | -------- |
| callNum        | int      | 123   |          |
| commit         | int/bool | 0     |          |
| connect_id     | str      | ccc   |          |
| lastCallTime   | int      | 111   |          |
| ownerProfileID | int      | 444   |          |
| sessionID      | str      | zzz   |          |

### Response

```
[
    0 // result status code
]
```
