# [GET] /game/Leaderboard/getStatGroupsByProfileIDs

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/Leaderboard/getStatGroupsByProfileIDs?callNum=123&connect_id=ccc&lastCallTime=111&profileids=[1,1]&sessionID=zzz HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type       | value              | comments                           |
| ------------ | ---------- | ------------------ | ---------------------------------- |
| callNum      | int        | 123                |                                    |
| connect_id   |            |                    |                                    |
| lastCallTime | timestamp  |                    |                                    |
| sessionID    | str        |                    |                                    |
| profileids   | array[int] | [2132331,31323213] | Without an underscore! (outdated?) |

### Response

```
[
    0, // result status code
    [
        [
            20075,
            "",
            "",
            1,
            [
                223576
            ]
        ]
    ],
    [
        [
            19614,
            223576,
            "/steam/76561198001031686",
            "{\"icon\":\"PR7-048\"}",
            "Sihing Mo",
            "AE2C",
            20075,
            797,
            1,
            0,
            null,
            "76561198001031686",
            3,
            []
        ]
    ],
    [
        [
            20075,
            4,
            556,
            637,
            -1,
            0,
            12,
            8838,
            65247,
            3594,
            28799,
            1,
            1946,
            1645037441
        ],
        [
            20075,
            0,
            38,
            30,
            1,
            0,
            1,
            29550,
            149911,
            10891,
            59515,
            1,
            1485,
            1645039032
        ],
        [
            20075,
            3,
            168,
            175,
            1,
            0,
            6,
            14189,
            40797,
            6091,
            17958,
            1,
            1103,
            1644856698
        ],
        [
            20075,
            8,
            2,
            3,
            -3,
            0,
            0,
            -1,
            -1,
            -1,
            -1,
            -1,
            1611,
            1606757931
        ],
        [
            20075,
            9,
            3,
            7,
            -3,
            0,
            0,
            -1,
            13729,
            -1,
            5762,
            0,
            1773,
            1606764206
        ],
        [
            20075,
            7,
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
            1697,
            1606074023
        ],
        [
            20075,
            10,
            0,
            2,
            -2,
            0,
            0,
            -1,
            -1,
            -1,
            -1,
            -1,
            917,
            1606137677
        ],
        [
            20075,
            14,
            35,
            32,
            6,
            0,
            0,
            -1,
            2359,
            -1,
            905,
            0,
            1067,
            1640275186
        ],
        [
            20075,
            13,
            14,
            9,
            -1,
            0,
            2,
            -1,
            1746,
            -1,
            690,
            0,
            1076,
            1640641202
        ]
    ]
]
```

## AoE3:DE

### Request

```
GET /game/Leaderboard/getStatGroupsByProfileIDs?callNum=21&connect_id=fflxvvhtmtcx7tmbxff2kauyfdq8n3&lastCallTime=8565&profileids=%5B9655781%5D&sessionID=fflxvvhtmtcx7tmbxff2kauyfdq8n3 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: deflate, gzip
Cookie: ApplicationGatewayAffinity=29259ca9e836dd7648ed1ca403a17cde;ApplicationGatewayAffinityCORS=29259ca9e836dd7648ed1ca403a17cde;worldsedgelink=-1321719403;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type       | value              | comments                           |
| ------------ | ---------- | ------------------ | ---------------------------------- |
| callNum      | int        | 123                |                                    |
| connect_id   |            |                    |                                    |
| lastCallTime | timestamp  |                    |                                    |
| sessionID    | str        |                    |                                    |
| profileids   | array[int] | [2132331,31323213] | Without an underscore! (outdated?) |

### Response

```
[
    0,
    [
        [
            2075838,
            "",
            "",
            1,
            [
                9633781 // self profile_id
            ]
        ]
    ],
    [
        [
            20,
            9633781, // self profile_id
            "/steam/76561199245791480", // self steam_id
            "",
            "NAME", // self steam_name
            "",
            2075838,
            0,
            1,
            0,
            null,
            "76561199245791480", // self steam_id64
            3,
            []
        ]
    ],
    []
]
```

## AoE4

### Request

```
GET /game/Leaderboard/getStatGroupsByProfileIDs?callNum=175&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=1987363&profileids=%5B233334%5D&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type       | value              | comments                           |
| ------------ | ---------- | ------------------ | ---------------------------------- |
| callNum      | int        | 123                |                                    |
| connect_id   |            |                    |                                    |
| lastCallTime | timestamp  |                    |                                    |
| profileids   | array[int] | [2132331,31323213] | Without an underscore! (outdated?) |
| sessionID    | str        |                    |                                    |

### Response

```
[
    0,
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
            24,
            233334, // self profile_id
            "/steam/76561197333367299", // self steam_id
            "",
            "ADSADAD", // self steam_name
            "",
            4275156,
            423,
            3,
            0,
            null,
            "76561197333367299", // self steam_id64
            3,
            []
        ]
    ],
    [
        [
            4275156,
            -1,
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
            1000,
            1666824365
        ]
    ]
]
```
