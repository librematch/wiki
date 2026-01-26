# [GET] /game/Leaderboard/getStatsForLeaderboardByProfileName

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/Leaderboard/getStatsForLeaderboardByProfileName?callNum=40&connect_id=6mikb1saqrmud2kte7ovswogamd2th&lastCallTime=64136&leaderboard_id=-1&profileids=%5B233334%5D&sessionID=6mikb1saqrmud2kte7ovswogamd2th HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter      | type       | value              | comments               |
| -------------- | ---------- | ------------------ | ---------------------- |
| callNum        | int        | 123                |                        |
| connect_id     |            |                    |                        |
| lastCallTime   | timestamp  |                    |                        |
| sessionID      | str        |                    |                        |
| leaderboard_id | int        | 13                 |                        |
| profileids     | array[int] | [2132331,31323213] | Without an underscore! |

### Response

```
[
    0, // result status code
    [
        [
            5056,
            "",
            "",
            1,
            [
                211257
            ]
        ],
        [
            20075,
            "",
            "",
            1,
            [
                223576
            ]
        ],
        [
            2818,
            "",
            "",
            1,
            [
                209525
            ]
        ]
    ],
    [
        [
            29916,
            211257, // profile_id
            "/steam/76561198221312408",
            "{\"icon\":\"PR5-033\"}",
            "真男人天降正义", // name
            "WWP", // clan
            5056, // some id
            1809,
            1,
            2,
            null,
            "76561198221312408",
            3,
            []
        ],
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
        ],
        [
            11548,
            209525,
            "/steam/76561197995781128",
            "{\"icon\":\"PR7-041\"}",
            "aoe2companion.com",
            "AE2C",
            2818,
            416,
            1,
            0,
            null,
            "76561197995781128",
            3,
            []
        ]
    ],
    [
        [
            5056, // some id
            3, // leaderboard_id
            403, // wins
            346, // losses
            1, // streak
            0,
            19, // drops
            -1, // rank?
            40798,
            -1, // some other field related to ranking
            5029,
            0,
            1836, // rating
            1630355912 // last match time?
        ],
        [
            20075,
            3,
            168,
            175,
            1,
            0,
            6, // drops
            14188, // rank
            40798,
            6091,
            17959,
            1,
            1103,
            1644856698
        ],
        [
            2818,
            3,
            16,
            10,
            -1,
            0,
            0,
            -1,
            40798,
            -1,
            17959,
            0,
            1189,
            1611445874
        ]
    ]
]
```

## AoE3:DE

### Request

```
GET /game/Leaderboard/getStatsForLeaderboardByProfileName?callNum=131&connect_id=fflxvvhtmtcx7tmbxff2kauyfdq8n3&lastCallTime=5503&leaderboard_id=3&profileids=%5B9652381%5D&sessionID=fflxvvhtmtcx7tmbxff2kauyfdq8n3 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: deflate, gzip
Cookie: ApplicationGatewayAffinity=29259ca9e836dd7648ed1ca403a17cde;ApplicationGatewayAffinityCORS=29259ca9e836dd7648ed1ca403a17cde;worldsedgelink=-1321719403;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter      | type       | value              | comments               |
| -------------- | ---------- | ------------------ | ---------------------- |
| callNum        | int        | 123                |                        |
| connect_id     |            |                    |                        |
| lastCallTime   | timestamp  |                    |                        |
| leaderboard_id | int        | 3                  |                        |
| profileids     | array[int] | [2132331,31323213] | Without an underscore! |
| sessionID      | str        |                    |                        |

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
                9652381
            ]
        ]
    ],
    [
        [
            20,
            9652381,
            "/steam/76561199233391480",
            "",
            "steam.aoe3",
            "",
            2075838,
            0,
            1,
            0,
            null,
            "76561199233391480",
            3,
            []
        ]
    ],
    []
]
```
