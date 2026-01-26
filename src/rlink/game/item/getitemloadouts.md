# [GET] /game/item/getItemLoadouts

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/item/getItemLoadouts?callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| callNum      | int       | 123   |          |
| connect_id   |           |       |          |
| lastCallTime | timestamp |       |          |
| sessionID    | str       |       |          |

### Response

```
[
    0, // result status code
    []
]
```

## AoE4

### Request

```
GET /game/item/getItemLoadouts?callNum=174&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=1986847&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| callNum      | int       | 123   |          |
| connect_id   |           |       |          |
| lastCallTime | timestamp |       |          |
| sessionID    | str       |       |          |

### Response

```
[
    0, // result status code
    []
]
```
