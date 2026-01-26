# [POST] /game/item/openItemPack

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/item/openItemPack HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 171
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

callNum=123&choices=[]&connect_id=ccc&itemInstance_id=5678&itemLocation_id=0&lastCallTime=111&sessionID=zzz
```

| parameter       | type      | value | comments |
| --------------- | --------- | ----- | -------- |
| callNum         | int       | 123   |          |
| choices         | array[?]  | []    |          |
| connect_id      |           |       |          |
| itemInstance_id | int       | 5678  |          |
| itemLocation_id | int       | 0     |          |
| lastCallTime    | timestamp |       |          |
| sessionID       | str       |       |          |

### Response

```
RESPONSE_TEMPLATE
```

## AoE4

### Request

```
POST /game/item/openItemPack HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 173
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=128&choices=[]&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&itemInstance_id=449956852&itemLocation_id=0&lastCallTime=658002&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19
```

| parameter       | type      | value | comments |
| --------------- | --------- | ----- | -------- |
| callNum         | int       | 123   |          |
| choices         | array[?]  | []    |          |
| connect_id      |           |       |          |
| itemInstance_id | int       | 5678  |          |
| itemLocation_id | int       | 0     |          |
| lastCallTime    | timestamp |       |          |
| sessionID       | str       |       |          |

### Response

```
[
    0, // result status code
    [
        [
            449957613,
            1,
            452595,
            233334, // self profile_id
            45939,
            0,
            "",
            1666824381,
            0,
            -1,
            3,
            -1
        ]
    ]
]
```
