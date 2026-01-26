# [GET] /game/Leaderboard/getPartyStat

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/Leaderboard/getPartyStat?callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz&statsids=[1,2] HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type       | value | comments |
| ------------ | ---------- | ----- | -------- |
| callNum      | int        | 123   |          |
| connect_id   |            |       |          |
| lastCallTime | timestamp  |       |          |
| sessionID    | str        |       |          |
| statsids     | array[int] | [2,3] |          |

### Response

```
[
    0, // result status code
    [
        [
            4037175,
            "",
            "",
            1,
            [
                4994658
            ]
        ],
        [
            33833,
            "",
            "",
            1,
            [
                233334 // self profile_id
            ]
        ]
    ],
    [
        [
            3180,
            4994658,
            "/steam/76561198841236701", // steam_id
            "{\"icon\":\"PR7-086\"}",
            "Atjov_", // in-game name
            "",
            4037175,
            151,
            1,
            0,
            null,
            "76561198841236701", // steam_id clean
            3,
            []
        ],
        [
            9813,
            233334,
            "/steam/76561197922222223", // self steam_id
            "{\"icon\":\"PR2-004\"}",
            "XXX", // self in-game name
            "",
            33833,
            1,
            1,
            0,
            null,
            "76561197922222223", // self clean steam_id
            3,
            []
        ]
    ],
    [
        [
            33833,
            0,
            0,
            1,
            -1,
            0,
            0,
            -1,
            -1,
            -1,
            -1,
            -1,
            986,
            1574923518
        ],
        [
            33833,
            3,
            1,
            0,
            1,
            0,
            0,
            -1,
            -1,
            -1,
            -1,
            -1,
            1050,
            1666400512
        ],
        [
            4037175,
            0,
            18,
            10,
            6,
            0,
            0,
            57043,
            178521,
            20733,
            67093,
            1,
            1181,
            1664054342
        ],
        [
            4037175,
            8,
            1,
            0,
            1,
            0,
            0,
            -1,
            -1,
            -1,
            -1,
            -1,
            1051,
            1631381819
        ],
        [
            4037175,
            3,
            82,
            81,
            -2,
            0,
            3,
            32119,
            39032,
            13021,
            15934,
            1,
            794,
            1666400512
        ],
        [
            4037175,
            4,
            7,
            11,
            2,
            0,
            1,
            -1,
            62642,
            -1,
            25180,
            0,
            850,
            1662682573
        ],
        [
            4037175,
            13,
            16,
            20,
            -1,
            0,
            1,
            2397,
            2666,
            956,
            1044,
            1,
            783,
            1665438962
        ],
        [
            4037175,
            14,
            3,
            7,
            -4,
            0,
            1,
            -1,
            2840,
            -1,
            986,
            0,
            835,
            1640210227
        ]
    ]
]
```

## AoE4

### Request

```
GET /game/Leaderboard/getPartyStat?callNum=233&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=2942957&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&statsids=%5B4275156%5D HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type       | value | comments |
| ------------ | ---------- | ----- | -------- |
| callNum      | int        | 123   |          |
| connect_id   |            |       |          |
| lastCallTime | timestamp  |       |          |
| sessionID    | str        |       |          |
| statsids     | array[int] | [2,3] |          |

### Response

```
[
    0, // result status code
    [
        [
            4275156,
            "",
            "",
            1,
            [
                233334
            ]
        ]
    ],
    [
        [
            31,
            233334,
            "/steam/765611933367299", // self full steam_id
            "",
            "DSADAS", // self steam_name
            "",
            4275156,
            735,
            4,
            0,
            null,
            "765611933367299", self steam_id64
            3,
            []
        ]
    ],
    [
        [
            4275156,
            -1,
            2,
            0,
            2,
            0,
            0,
            -1,
            -1,
            -1,
            -1,
            -1,
            1000,
            1666826657
        ]
    ]
]
```
