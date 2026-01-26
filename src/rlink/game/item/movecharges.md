# [POST] /game/item/moveCharges

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/item/moveCharges HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 202
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

callNum=123&charges=[123]&connect_id=ccc&deletes=[1]&fromItemIDs=[321]&lastCallTime=111&sessionID=zzz&toItemIDs=[456]
```

| parameter    | type       | value | comments |
| ------------ | ---------- | ----- | -------- |
| callNum      | int        | 123   |          |
| charges      | array[int] | [123] |          |
| connect_id   |            |       |          |
| deletes      | array[int] | [1]   |          |
| fromItemIDs  | array[int] | [4,5] |          |
| lastCallTime | timestamp  |       |          |
| sessionID    | str        |       |          |
| toItemIDs    | array[int] | [1,3] |          |

### Response

```
RESPONSE_TEMPLATE
```

## AoE4

### Request

```
POST /game/item/moveCharges HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 198
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=36&charges=[1]&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&deletes=[1]&fromItemIDs=[449911778]&lastCallTime=18396&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&toItemIDs=[449911716]
```

| parameter    | type       | value | comments |
| ------------ | ---------- | ----- | -------- |
| callNum      | int        | 123   |          |
| charges      | array[int] | [123] |          |
| connect_id   |            |       |          |
| deletes      | array[int] | [1]   |          |
| fromItemIDs  | array[int] | [4,5] |          |
| lastCallTime | timestamp  |       |          |
| sessionID    | str        |       |          |
| toItemIDs    | array[int] | [1,3] |          |

### Response

```
[
    0,
    [
        0
    ],
    [
        0
    ],
    [
        2
    ],
    [
        [
            449911716,
            1,
            454438,
            233334, // self profile_id
            2,
            0,
            "",
            1666823722,
            0,
            -1,
            3,
            -1
        ]
    ]
]
```
