# [POST] /game/advertisement/startObserving

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/advertisement/startObserving HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 308
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

advertisementid=1&appbinarychecksum=8888&callNum=123&connect_id=ccc&datachecksum=-888&lastCallTime=111&moddllchecksum=0&moddllfile=INVALID&modname=INVALID&modversion=INVALID&password=&sessionID=zzz&versionFlags=0&withPartySessionID=333
```

| parameter          | type      | value | comments |
| ------------------ | --------- | ----- | -------- |
| advertisementid    | int       | -1    |          |
| appBinaryChecksum  | int       | 8888  |          |
| callNum            | int       | 123   |          |
| connect_id         |           |       |          |
| dataChecksum       | int       | -777  |          |
| lastCallTime       | timestamp | 111   |          |
| moddllchecksum     | str       | 0     |          |
| moddllfile         |           |       | INVALID  |
| modname            |           |       | INVALID  |
| modversion         |           |       | INVALID  |
| password           | ?         | None  |          |
| sessionID          | str       |       |          |
| versionFlags       | int       | 0     |          |
| withPartySessionID | int       | 333   |          |

### Response

```
[
    0,
    "20.84.120.105",
    27014,
    27114,
    27214,
    [
        [
            551863,
            []
        ],
        [
            539907,
            []
        ]
    ],
    1666489082,
    [
        [
            "551863",
            []
        ],
        [
            "539907",
            []
        ]
    ]
]
```

## AoE4

### Request

```
POST /game/advertisement/startObserving HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 312
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

advertisementid=50865077&appbinarychecksum=24916&callNum=332&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&datachecksum=-638535971&lastCallTime=3098691&moddllchecksum=0&moddllfile=INVALID&modname=INVALID&modversion=INVALID&password=&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&versionFlags=0&withPartySessionID=50865084
```

| parameter          | type      | value    | comments |
| ------------------ | --------- | -------- | -------- |
| advertisementid    | int       | 50865077 |          |
| appBinaryChecksum  | int       | 8888     |          |
| callNum            | int       | 123      |          |
| connect_id         |           |          |          |
| dataChecksum       | int       | -777     |          |
| lastCallTime       | timestamp | 111      |          |
| moddllchecksum     | str       | 0        |          |
| moddllfile         |           |          | INVALID  |
| modname            |           |          | INVALID  |
| modversion         |           |          | INVALID  |
| password           | ?         | None     |          |
| sessionID          | str       |          |          |
| versionFlags       | int       | 0        |          |
| withPartySessionID | int       | 333      |          |

### Response

```
[
    0,
    "20.121.139.95",
    27019,
    27119,
    27219,
    [
        [
            9303146,
            []
        ],
        [
            10956109,
            [
                "1668570"
            ]
        ],
        [
            9667303,
            []
        ],
        [
            11117538,
            []
        ],
        [
            7528032,
            []
        ],
        [
            8160212,
            []
        ],
        [
            666022,
            []
        ],
        [
            5946231,
            []
        ]
    ],
    1666826785,
    [
        [
            "9303146",
            [
                [
                    275049953,
                    6,
                    450847,
                    9303146,
                    1,
                    0,
                    "{}",
                    1642599109,
                    2,
                    -1,
                    19,
                    2147483647
                ],
                [
                    275049961,
                    1,
                    451960,
                    9303146,
                    1,
                    0,
                    "{}",
                    1642599109,
                    5,
                    -1,
                    3,
                    2147483647
                ]
            ]
        ],
        [
            "10956109",
            [
                [
                    382684327,
                    12,
                    450847,
                    10956109,
                    1,
                    0,
                    "{}",
                    1660740213,
                    2,
                    -1,
                    19,
                    2147483647
                ],
                [
                    382684323,
                    1,
                    453188,
                    10956109,
                    1,
                    0,
                    "{\"att\":{\"is_new\":{\"val\":\"0\"}},\"dlc\":1}",
                    1660740213,
                    5,
                    -1,
                    19,
                    -1
                ],
                [
                    382684335,
                    2,
                    451960,
                    10956109,
                    1,
                    0,
                    "{}",
                    1660740213,
                    5,
                    -1,
                    3,
                    2147483647
                ]
            ]
        ],
        [
            "9667303",
            [
                [
                    443317086,
                    1,
                    453169,
                    9667303,
                    1,
                    0,
                    "",
                    1666776199,
                    2,
                    -1,
                    19,
                    -1
                ],
                [
                    301985045,
                    2,
                    451960,
                    9667303,
                    1,
                    0,
                    "{}",
                    1645820978,
                    5,
                    -1,
                    3,
                    2147483647
                ],
                [
                    360386054,
                    5,
                    453123,
                    9667303,
                    1,
                    0,
                    "{\"att\":{\"is_new\":{\"val\":\"0\"}}}",
                    1657299576,
                    5,
                    -1,
                    51,
                    -1
                ]
            ]
        ],
        [
            "11117538",
            [
                [
                    400005401,
                    16,
                    451770,
                    11117538,
                    1,
                    0,
                    "{}",
                    1661645022,
                    2,
                    -1,
                    19,
                    2147483647
                ],
                [
                    400005404,
                    1,
                    451960,
                    11117538,
                    1,
                    0,
                    "{}",
                    1661645022,
                    5,
                    -1,
                    3,
                    2147483647
                ]
            ]
        ],
        [
            "7528032",
            [
                [
                    438067935,
                    3,
                    453169,
                    7528032,
                    1,
                    0,
                    "",
                    1666735153,
                    2,
                    -1,
                    19,
                    -1
                ],
                [
                    83404242,
                    2,
                    451960,
                    7528032,
                    1,
                    0,
                    "{}",
                    1635713927,
                    5,
                    -1,
                    3,
                    2147483647
                ],
                [
                    357982065,
                    7,
                    453334,
                    7528032,
                    1,
                    0,
                    "{\"att\":{\"is_new\":{\"val\":\"0\"}}}",
                    1656802924,
                    5,
                    -1,
                    51,
                    -1
                ]
            ]
        ],
        [
            "8160212",
            [
                [
                    438384255,
                    5,
                    453169,
                    8160212,
                    1,
                    0,
                    "",
                    1666737151,
                    2,
                    -1,
                    19,
                    -1
                ],
                [
                    160015526,
                    1,
                    451960,
                    8160212,
                    1,
                    0,
                    "{}",
                    1636681870,
                    5,
                    -1,
                    3,
                    2147483647
                ]
            ]
        ],
        [
            "666022",
            [
                [
                    203924509,
                    14,
                    450847,
                    666022,
                    1,
                    0,
                    "{}",
                    1638032379,
                    2,
                    -1,
                    19,
                    2147483647
                ],
                [
                    203924517,
                    1,
                    451960,
                    666022,
                    1,
                    0,
                    "{}",
                    1638032379,
                    5,
                    -1,
                    3,
                    2147483647
                ]
            ]
        ],
        [
            "5946231",
            [
                [
                    436826555,
                    1,
                    453199,
                    5946231,
                    1,
                    0,
                    "",
                    1666728871,
                    2,
                    -1,
                    19,
                    -1
                ],
                [
                    431450818,
                    1,
                    451960,
                    5946231,
                    1,
                    0,
                    "{}",
                    1666627897,
                    5,
                    -1,
                    3,
                    2147483647
                ]
            ]
        ]
    ]
]
```
