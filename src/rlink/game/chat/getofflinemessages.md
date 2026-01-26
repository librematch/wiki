# [GET] /game/chat/getOfflineMessages

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/chat/getOfflineMessages?callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz HTTP/1.1
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
    [],
    [
        [
            "233334", // self profile_id
            []
        ]
    ],
    [],
    [],
    []
]
```

## AoE4

### Request

```
GET /game/chat/getOfflineMessages?callNum=12&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=5996&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
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
    0,
    [
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
        ]
    ],
    [
        [
            "233334",
            [
                [
                    70218256,
                    233334,
                    2,
                    "SYSTEM_OFFLINEITEM_COMMUNITY_EVENT",
                    "Event Items Granted!",
                    "These items have been granted as part of the currently running event.",
                    1666823722,
                    "",
                    70213314
                ],
                [
                    70218257,
                    233334,
                    2,
                    "SYSTEM_OFFLINEITEM_COMMUNITY_EVENT",
                    "Event Items Granted!",
                    "These items have been granted as part of the currently running event.",
                    1666823722,
                    "",
                    70213315
                ],
                [
                    70218258,
                    233334,
                    2,
                    "SYSTEM_OFFLINEITEM_COMMUNITY_EVENT",
                    "Event Items Granted!",
                    "These items have been granted as part of the currently running event.",
                    1666823722,
                    "",
                    70213316
                ]
            ]
        ]
    ],
    [
        [
            70213314,
            2,
            233334,
            0,
            0,
            1,
            null,
            null
        ],
        [
            70213315,
            2,
            233334,
            0,
            0,
            1,
            null,
            null
        ],
        [
            70213316,
            2,
            233334,
            0,
            0,
            1,
            null,
            null
        ]
    ],
    [
        [
            "70213314",
            []
        ],
        [
            "70213315",
            []
        ],
        [
            "70213316",
            []
        ]
    ],
    [
        [
            "70213314",
            [
                [
                    449911890,
                    2,
                    454345,
                    233334,
                    1,
                    0,
                    "",
                    1666823722,
                    -1,
                    70213314,
                    35,
                    -1
                ]
            ]
        ],
        [
            "70213315",
            [
                [
                    449911888,
                    2,
                    454343,
                    233334,
                    1,
                    0,
                    "",
                    1666823722,
                    -1,
                    70213315,
                    35,
                    -1
                ]
            ]
        ],
        [
            "70213316",
            [
                [
                    449911889,
                    2,
                    454344,
                    233334,
                    1,
                    0,
                    "",
                    1666823722,
                    -1,
                    70213316,
                    35,
                    -1
                ]
            ]
        ]
    ]
]
```
