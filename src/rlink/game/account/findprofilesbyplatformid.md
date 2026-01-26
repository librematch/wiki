# [POST] /game/account/FindProfilesByPlatformID

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/account/FindProfilesByPlatformID HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 1688
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
Expect: 100-continue
```

| parameter    | type       | value   | comments |
| ------------ | ---------- | ------- | -------- |
| callNum      | int        | 123     |          |
| connect_id   |            |         |          |
| lastCallTime | timestamp  |         |          |
| platformIDs  | array[str] | ["",""] |          |
| sessionID    | str        |         |          |

### Response

```
[
    0, // result status code
    [
        [
            8,
            1,
            "admin",
            "",
            "",
            "",
            1,
            0,
            1,
            -1,
            null,
            "",
            4,
            []
        ],
        [
            0,
            2,
            "system",
            "",
            "",
            "",
            2,
            0,
            1,
            -1,
            null,
            "",
            4,
            []
        ],
        [
            0,
            3,
            "reader",
            "",
            "",
            "",
            3,
            0,
            1,
            -1,
            null,
            "",
            4,
            []
        ],
        [
            0,
            649236,
            "/partner//partner/WebAccess",
            "",
            "",
            "",
            509197,
            0,
            1,
            -1,
            null,
            "",
            1,
            []
        ],
        [
            0,
            2252570,
            "/partner//partner/web-access",
            "",
            "",
            "",
            2377787,
            0,
            1,
            -1,
            null,
            "",
            1,
            []
        ],
        [
            0,
            3127656,
            "/partner/sieberta-db-checks",
            "",
            "",
            "",
            2833167,
            0,
            1,
            -1,
            null,
            "",
            1,
            []
        ]
    ]
]
```

## AoE4

### Request

```
POST /game/account/FindProfilesByPlatformID HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 288
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=44&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=22511&platformIDs=[76561197960287614,76561197978627567,76561197978943286,76561198000229224,76561197972009043,76561197964180873,76561197966000898,76561197976722725]&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19
```

| parameter    | type       | value   | comments |
| ------------ | ---------- | ------- | -------- |
| callNum      | int        | 123     |          |
| connect_id   |            |         |          |
| lastCallTime | timestamp  |         |          |
| platformIDs  | array[str] | ["",""] |          |
| sessionID    | str        |         |          |

### Response

```
[
    0,
    [
        [
            25705,
            197751,
            "/steam/76561197964180873",
            "{\"sharedHistory\":1}",
            "GL.Nili",
            "",
            483,
            262771,
            140,
            0,
            null,
            "76561197964180873",
            3,
            []
        ]
    ]
]
```
