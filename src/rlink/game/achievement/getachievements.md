# [GET] /game/Achievement/getAchievements

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/Achievement/getAchievements?callNum=123&connect_id=ccc&lastCallTime=111&profileIDs=[1,1]&sessionID=zzz HTTP/1.1
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
| profileIDs   | array[int] | [1,3] |          |
| sessionID    | str        |       |          |

### Response

```
[
    0, // result status code
    [
        [
            233334, // self profile_id
            [
                [
                    38, // achievement_id (lookup with `getAvailableAchievements`)
                    1605802963
                ],
                [
                    46,
                    1605807055
                ],
                [
                    37,
                    1606317489
                ],
                [
                    6,
                    1606360352
                ],
                [
                    129,
                    1606360353
                ],
                [
                    131,
                    1606664422
                ],
                [
                    127,
                    1606877828
                ],
                [
                    137,
                    1607022190
                ],
                [
                    126,
                    1607022876
                ],
                [
                    135,
                    1607511361
                ],
                [
                    40,
                    1607598250
                ],
                [
                    125,
                    1632263195
                ],
                [
                    133,
                    1635842528
                ],
                [
                    132,
                    1635844687
                ],
                [
                    117,
                    1635845941
                ],
                [
                    119,
                    1635847743
                ],
                [
                    23,
                    1635848345
                ],
                [
                    48,
                    1635902087
                ],
                [
                    32,
                    1635902378
                ],
                [
                    21,
                    1635928068
                ],
                [
                    16,
                    1635931683
                ],
                [
                    134,
                    1636003806
                ],
                [
                    24,
                    1636004183
                ],
                [
                    7,
                    1636014445
                ],
                [
                    170,
                    1636033434
                ],
                [
                    168,
                    1636036263
                ],
                [
                    39,
                    1636203151
                ],
                [
                    115,
                    1636221352
                ],
                [
                    113,
                    1636225836
                ],
                [
                    5,
                    1636226890
                ],
                [
                    167,
                    1636279812
                ],
                [
                    116,
                    1636375679
                ],
                [
                    30,
                    1636540490
                ],
                [
                    22,
                    1636550163
                ],
                [
                    25,
                    1636629408
                ],
                [
                    33,
                    1636654440
                ],
                [
                    3,
                    1637334910
                ],
                [
                    85,
                    1638094091
                ],
                [
                    35,
                    1638201135
                ],
                [
                    4,
                    1638204100
                ],
                [
                    28,
                    1638354027
                ],
                [
                    15,
                    1640894830
                ],
                [
                    18,
                    1640958146
                ],
                [
                    34,
                    1642049273
                ],
                [
                    36,
                    1642332046
                ],
                [
                    29,
                    1642429347
                ],
                [
                    31,
                    1642444499
                ],
                [
                    11,
                    1642538349
                ],
                [
                    10,
                    1642590273
                ],
                [
                    138,
                    1642592022
                ],
                [
                    19,
                    1642592409
                ],
                [
                    27,
                    1642623915
                ],
                [
                    17,
                    1642782188
                ],
                [
                    14,
                    1645422635
                ],
                [
                    13,
                    1645692489
                ],
                [
                    12,
                    1646301580
                ],
                [
                    2,
                    1646986871
                ],
                [
                    169,
                    1651037876
                ],
                [
                    26,
                    1655886197
                ],
                [
                    20,
                    1655894869
                ],
                [
                    114,
                    1655981638
                ],
                [
                    191,
                    1656250094
                ],
                [
                    188,
                    1656250385
                ],
                [
                    8,
                    1657473441
                ],
                [
                    153,
                    1657666053
                ],
                [
                    151,
                    1657666956
                ],
                [
                    186,
                    1657702911
                ],
                [
                    187,
                    1658288110
                ],
                [
                    9,
                    1658875943
                ],
                [
                    190,
                    1658924813
                ],
                [
                    189,
                    1661853651
                ],
                [
                    44,
                    1663108280
                ],
                [
                    152,
                    1664313299
                ]
            ]
        ]
    ]
]
```

## AoE3:DE

### Request

```
GET /game/Achievement/getAchievements?callNum=20&connect_id=fflxvvhtmtcx7tmbxff2kauyfdq8n3&lastCallTime=8040&profileIDs=%5B9655781%5D&sessionID=fflxvvhtmtcx7tmbxff2kauyfdq8n3 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: deflate, gzip
Cookie: ApplicationGatewayAffinity=29259ca9e836dd7648ed1ca403a17cde;ApplicationGatewayAffinityCORS=29259ca9e836dd7648ed1ca403a17cde;worldsedgelink=-1321719403;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type       | value | comments |
| ------------ | ---------- | ----- | -------- |
| callNum      | int        | 123   |          |
| connect_id   |            |       |          |
| lastCallTime | timestamp  |       |          |
| profileIDs   | array[int] | [1,3] |          |
| sessionID    | str        |       |          |

### Response

```
[
    0,
    [
        [
            9633781,
            []
        ]
    ]
]
```

## AoE4

### Request

```
GET /game/Achievement/getAchievements?callNum=173&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=1986330&profileIDs=%5B233334%5D&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
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
| profileIDs   | array[int] | [1,3] |          |
| sessionID    | str        |       |          |

### Response

```
[
    0, // result code
    [
        [
            233334, // self profile_id
            [
                [
                    2033486,
                    1666824050
                ]
            ]
        ]
    ]
]
```
