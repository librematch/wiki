# [POST] /game/item/detachItems

**AUTHENTICATION**

## AoE4

### Request

```
POST /game/item/detachItems HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 278
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=25&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&itemCharges=[1,1,1,1,1,1]&itemIDs=[449911890,449911890,449911888,449911890,449911888,449911889]&itemLocations=[0,0,0,0,0,0]&lastCallTime=12729&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19
```

| parameter     | type       | value         | comments |
| ------------- | ---------- | ------------- | -------- |
| callNum       | int        | 123           |          |
| connect_id    |            |               |          |
| itemCharges   | arr[int]   | [1,1,1,1,1,1] |          |
| itemIDs       | array[int] | [4,5]         |          |
| itemLocations | array[int] | [12,3]        |          |
| lastCallTime  | timestamp  |               |          |
| sessionID     | str        |               |          |

### Response

```
[
    0,
    [
        0,
        1,
        0,
        1,
        1,
        0
    ],
    [
        [
            449911890,
            3,
            454345,
            233334, // self profile_id
            1,
            0,
            "",
            1666823722,
            0,
            -1,
            35,
            -1
        ],
        [
            449911888,
            3,
            454343,
            233334, // self profile_id
            1,
            0,
            "",
            1666823722,
            0,
            -1,
            35,
            -1
        ],
        [
            449911889,
            3,
            454344,
            233334, // self profile_id
            1,
            0,
            "",
            1666823722,
            0,
            -1,
            35,
            -1
        ]
    ]
]
```
