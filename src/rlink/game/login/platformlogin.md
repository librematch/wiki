# [POST] /game/login/platformlogin

**AUTHENTICATION**

## AoE:DE

### Request

```
POST /game/login/platformlogin HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 524
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

accountType=STEAM&alias=aliasname&appID=1017900&auth=auth&callNum=0&clientLibVersion=151&connect_id=&country=DE&installationType=windows&language=en&lastCallTime=14901221&macAddress=mac&majorVersion=4.0.0&minorVersion=0&platformUserID=76561133333337299&startGameToken=&syncHash=[0,0]&timeoutOverride=0&title=age
```

| parameter        | type               | value   | comments    |
| ---------------- | ------------------ | ------- | ----------- |
| accountType      | str/enum           | STEAM   |             |
| alias            | str                | name    |             |
| appID            | int                | 1017900 |             |
| auth             | str                | authzzz |             |
| callNum          | int                | 0       | 0 = initial |
| clientLibVersion | int                | 151     |             |
| connect_id       | str                | None    |             |
| country          | ISO 3166-1 Alpha-2 | US      |             |
| installationType | str/enum           | windows |             |
| language         | str                | en      |             |
| lastCallTime     | timestamp          | 111     |             |
| macAddress       | str                | mac     |             |
| majorVersion     | semVer             | 4.0.0   |             |
| minorVersion     | int                | 0       |             |
| platformUserID   | int                | 666     | STEAM_ID    |
| startGameToken   | str                | None    |             |
| syncHash         | array[int]         | [0,0]   |             |
| timeoutOverride  | int/bool           | 0       |             |
| title            | str/enum           | age     |             |

## AoE2:DE

### Request

```
POST /game/login/platformlogin HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 524
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

accountType=STEAM&activeMatchId=-1&alias=name&appID=8888&auth=authzzz&callNum=123&clientLibVersion=5&connect_id=&country=US&installationType=windows&language=en&lastCallTime=111&macAddress=mac&majorVersion=0.0.0&minorVersion=7777&platformUserID=666&startGameToken=&syncHash=[0,0]&timeoutOverride=0&title=age4
```

| parameter        | type               | value   | comments    |
| ---------------- | ------------------ | ------- | ----------- |
| accountType      | str/enum           | STEAM   |             |
| activeMatchId    | int                | -1      |             |
| alias            | str                | name    |             |
| appID            | int                | 813780  |             |
| auth             | str                | authzzz |             |
| callNum          | int                | 0       | 0 = initial |
| clientLibVersion | int                | 169     |             |
| connect_id       | str                | None    |             |
| country          | ISO 3166-1 Alpha-2 | US      |             |
| installationType | str/enum           | windows |             |
| language         | str                | en      |             |
| lastCallTime     | timestamp          | 111     |             |
| macAddress       | str                | mac     |             |
| majorVersion     | semVer             | 4.0.0   |             |
| minorVersion     | int                | 0       |             |
| platformUserID   | int                | 666     | STEAM_ID    |
| startGameToken   | str                | None    |             |
| syncHash         | array[int]         | [0,0]   |             |
| timeoutOverride  | int/bool           | 0       |             |
| title            | str/enum           | age2    |             |

### Response

```
[
    0, // result status code
    "ebyb0gp9rsvu863i501263m9wjly55",
    840887830,
    1666397899,
    [
        233329,
        "/steam/765611933367299", // steam_id
        3,
        -1,
        0,
        "de",
        "eur",
        2,
        null
    ],
    [
        [
            9803,
            233334, // self profile_id
            "/steam/76561197333337299", // self steam_id
            "{\"icon\":\"PR2-004\"}",
            "username", // self in-game name
            "",
            33833,
            0,
            1,
            0,
            null,
            "765611979333337299", // self steam_id
            3,
            []
        ]
    ],
    0,
    0,
    null,
    [
        [
            "RL_AUTOMATCH2_FAILSAFE_SEC",
            "180"
        ],
        [
            "PHX_LOG_SYNCPLAYER",
            "1"
        ],
        [
            "PHX_LOG_SYNCAI",
            "1"
        ],
        [
            "PHX_LOG_SYNCRANDOM",
            "1"
        ],
        [
            "RL_USE_WEBSOCKET_PERCENT",
            "100"
        ],
        [
            "RL_KEEPALIVE",
            "20"
        ],
        [
            "RL_DISCONNECT",
            "30"
        ],
        [
            "RL_MISSPOLL",
            "3"
        ],
        [
            "RL_TELEMSERVICE",
            "0"
        ],
        [
            "RL_TELEMREPORTPCT",
            "1.0"
        ],
        [
            "RL_MATCHTELEMPERIOD",
            "600"
        ],
        [
            "RL_TELEMKINESISID",
            "AKIATP3EMETR5VNBZMKA"
        ],
        [
            "RL_TELEMKINESISKEY",
            "kbduLAQls86v4Q2+yMzESocLldrah6WAowEv8IYW"
        ],
        [
            "RL_TELEMKINESISHOST",
            "kinesis.us-east-1.amazonaws.com"
        ],
        [
            "RL_TELEMKINESISSTREAM",
            "s3DevStream"
        ],
        [
            "RL_TELEMCELLHOST",
            "phoenix.maelstrom.gameservices.xboxlive.com"
        ],
        [
            "RL_TELEMCELLPATH",
            "/tenants/phoenix/routes/steam/"
        ],
        [
            "RL_CLUSTERNAME",
            "aoelive_"
        ],
        [
            "RL_TITLEID",
            "24"
        ],
        [
            "RL_OBSERVERCUSTOMDELAY",
            "180"
        ],
        [
            "RL_OBSERVERMAX",
            "0"
        ],
        [
            "RL_USE_AUTOMATCH2",
            "1"
        ],
        [
            "RL_AUTOMATCH2_TEAM_FACTION_TYPE",
            "1"
        ],
        [
            "RL_UPLOAD_TIMEOUT",
            "300000"
        ],
        [
            "RL_CLOUDCACHETIME",
            "21600"
        ],
        [
            "RL_CLOUD_CREDENTIAL_PROVIDER",
            "AZURE"
        ],
        [
            "RL_ITEM_LOADOUTS_MAX",
            "50"
        ],
        [
            "RL_CLAN_INVITE_EXPIRE_TIME_SEC",
            "43200"
        ],
        [
            "RL_NUMBER_OF_GAMES_TO_RANK",
            "10"
        ],
        [
            "RL_NUMBER_OF_EVENT_GAMES_TO_RANK",
            "5"
        ],
        [
            "RL_WEB_ASSETS_ICONS_ROOT",
            "https://test-build-data.worldsedgelink.com/"
        ],
        [
            "RL_SSO_URL",
            "<https://sso.relic.com/en/steam?title=age2>&"
        ]
    ],
    [
        0,
        [
            9803,
            233334, // self profile_id
            "/steam/7656133337299", // self steam_id
            "{\"icon\":\"PR2-004\"}",
            "username", // self in-game
            "",
            33833,
            0,
            1,
            0,
            null,
            "7656119333337299", // self steam_id
            3,
            []
        ],
        [
            0,
            [],
            [],
            [],
            [],
            [
                [
                    4194,
                    453225,
                    "/steam/76561198041844374",
                    "{\"icon\":\"PR7-003\"}",
                    "How Do I Shoot ZweihÃ¤nder",
                    "",
                    294907,
                    161,
                    1,
                    3,
                    null,
                    "76561198041844374",
                    3,
                    [],
                    0,
                    null,
                    []
                ],
                [
                    1184,
                    518884,
                    "/steam/76561198023323630",
                    "{\"icon\":\"PR7-001\"}",
                    "CarbonbaseD",
                    "",
                    368202,
                    28,
                    1,
                    0,
                    null,
                    "76561198023323630",
                    3,
                    [],
                    0,
                    null,
                    []
                ],
                [
                    4763,
                    649416,
                    "/steam/76561198016961929",
                    "{\"icon\":\"PR5-004\"}",
                    "Hazza_",
                    "",
                    509274,
                    173,
                    1,
                    0,
                    null,
                    "76561198016961929",
                    3,
                    [],
                    0,
                    null,
                    []
                ]
            ],
            [],
            []
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
            ]
        ],
        [
            [
                2,
                233334, // self profile_id
                0,
                "",
                1574923522
            ],
            [
                3,
                233334, // self profile_id
                17,
                "",
                1663935508
            ],
            [
                4,
                233334, // self profile_id
                23,
                "",
                1663422369
            ],
            [
                5,
                233334, // self profile_id
                25,
                "",
                1664421686
            ],
            [
                6,
                233334, // self profile_id
                11,
                "",
                1645683101
            ],
            [
                7,
                233334, // self profile_id
                9,
                "",
                1665499346
            ],
            [
                8,
                233334, // self profile_id
                9,
                "",
                1663166578
            ],
            [
                9,
                233334, // self profile_id
                17,
                "",
                1663016190
            ],
            [
                10,
                233334, // self profile_id
                19,
                "",
                1666388280
            ],
            [
                11,
                233334, // self profile_id
                17,
                "",
                1657298979
            ],
            [
                12,
                233334, // self profile_id
                12,
                "",
                1646052001
            ],
            [
                13,
                233334, // self profile_id
                15,
                "",
                1662456235
            ],
            [
                14,
                233334, // self profile_id
                15,
                "",
                1663972327
            ],
            [
                15,
                233334, // self profile_id
                13,
                "",
                1662901335
            ],
            [
                16,
                233334, // self profile_id
                17,
                "",
                1666294929
            ],
            [
                17,
                233334, // self profile_id
                13,
                "",
                1655706528
            ],
            [
                18,
                233334, // self profile_id
                13,
                "",
                1666307388
            ],
            [
                19,
                233334, // self profile_id
                19,
                "",
                1664326346
            ],
            [
                20,
                233334, // self profile_id
                14,
                "",
                1660799960
            ],
            [
                21,
                233334, // self profile_id
                13,
                "",
                1651329686
            ],
            [
                22,
                233334, // self profile_id
                16,
                "",
                1663985417
            ],
            [
                23,
                233334, // self profile_id
                15,
                "",
                1655890531
            ],
            [
                24,
                233334, // self profile_id
                18,
                "",
                1665342599
            ],
            [
                25,
                233334, // self profile_id
                11,
                "",
                1664424748
            ],
            [
                26,
                233334, // self profile_id
                23,
                "",
                1666042834
            ],
            [
                27,
                233334, // self profile_id
                15,
                "",
                1663427178
            ],
            [
                28,
                233334, // self profile_id
                19,
                "",
                1663363479
            ],
            [
                29,
                233334, // self profile_id
                20,
                "",
                1662291690
            ],
            [
                30,
                233334, // self profile_id
                8,
                "",
                1666276759
            ],
            [
                31,
                233334, // self profile_id
                13,
                "",
                1664116487
            ],
            [
                32,
                233334, // self profile_id
                4,
                "",
                1651253562
            ],
            [
                33,
                233334, // self profile_id
                15,
                "",
                1658288109
            ],
            [
                34,
                233334, // self profile_id
                17,
                "",
                1659318418
            ],
            [
                35,
                233334, // self profile_id
                14,
                "",
                1659312567
            ],
            [
                36,
                233334, // self profile_id
                15,
                "",
                1664503204
            ],
            [
                37,
                233334, // self profile_id
                13,
                "",
                1665429700
            ],
            [
                38,
                233334, // self profile_id
                381,
                "",
                1666388280
            ],
            [
                39,
                233334, // self profile_id
                95727,
                "",
                1608164244
            ],
            [
                40,
                233334, // self profile_id
                51653,
                "",
                1636226889
            ],
            [
                41,
                233334, // self profile_id
                32367,
                "",
                1636279810
            ],
            [
                42,
                233334, // self profile_id
                8700,
                "",
                1578826971
            ],
            [
                43,
                233334, // self profile_id
                3900,
                "",
                1607783638
            ],
            [
                44,
                233334, // self profile_id
                272536,
                "",
                1666388280
            ],
            [
                45,
                233334, // self profile_id
                137492,
                "",
                1666388280
            ],
            [
                46,
                233334, // self profile_id
                314,
                "",
                1666118987
            ],
            [
                47,
                233334, // self profile_id
                30940,
                "",
                1666388280
            ],
            [
                48,
                233334, // self profile_id
                6016,
                "",
                1666307388
            ],
            [
                49,
                233334, // self profile_id
                13,
                "",
                1636219807
            ],
            [
                50,
                233334, // self profile_id
                2872,
                "",
                1666388280
            ],
            [
                52,
                233334, // self profile_id
                69,
                "",
                1658848644
            ],
            [
                53,
                233334, // self profile_id
                7199,
                "",
                1666388275
            ],
            [
                54,
                233334, // self profile_id
                3582,
                "",
                1666387217
            ],
            [
                55,
                233334, // self profile_id
                88,
                "",
                1664325799
            ],
            [
                56,
                233334, // self profile_id
                10240,
                "",
                1666387177
            ],
            [
                57,
                233334, // self profile_id
                992,
                "",
                1666388275
            ],
            [
                59,
                233334, // self profile_id
                907,
                "",
                1666388280
            ],
            [
                60,
                233334, // self profile_id
                1,
                "",
                1574923526
            ],
            [
                61,
                233334, // self profile_id
                757,
                "",
                1666388280
            ],
            [
                64,
                233334, // self profile_id
                15,
                "",
                1578921257
            ],
            [
                69,
                233334, // self profile_id
                44,
                "",
                1665429700
            ],
            [
                70,
                233334, // self profile_id
                27,
                "",
                1664326346
            ],
            [
                71,
                233334, // self profile_id
                27,
                "",
                1664116487
            ],
            [
                72,
                233334, // self profile_id
                20,
                "",
                1664421686
            ],
            [
                73,
                233334, // self profile_id
                19,
                "",
                1664313298
            ],
            [
                74,
                233334, // self profile_id
                20,
                "",
                1658770151
            ],
            [
                75,
                233334, // self profile_id
                30,
                "",
                1666042834
            ],
            [
                76,
                233334, // self profile_id
                15,
                "",
                1663422369
            ],
            [
                77,
                233334, // self profile_id
                28,
                "",
                1662899239
            ],
            [
                78,
                233334, // self profile_id
                29,
                "",
                1664471510
            ],
            [
                79,
                233334, // self profile_id
                22,
                "",
                1666051855
            ],
            [
                80,
                233334, // self profile_id
                29,
                "",
                1660994527
            ],
            [
                81,
                233334, // self profile_id
                23,
                "",
                1664503204
            ],
            [
                82,
                233334, // self profile_id
                36,
                "",
                1663016190
            ],
            [
                83,
                233334, // self profile_id
                23,
                "",
                1666307388
            ],
            [
                84,
                233334, // self profile_id
                32,
                "",
                1664313298
            ],
            [
                85,
                233334, // self profile_id
                19,
                "",
                1664503204
            ],
            [
                86,
                233334, // self profile_id
                34,
                "",
                1657896505
            ],
            [
                87,
                233334, // self profile_id
                27,
                "",
                1664471510
            ],
            [
                88,
                233334, // self profile_id
                20,
                "",
                1664421686
            ],
            [
                89,
                233334, // self profile_id
                23,
                "",
                1666294929
            ],
            [
                90,
                233334, // self profile_id
                31,
                "",
                1665429700
            ],
            [
                91,
                233334, // self profile_id
                37,
                "",
                1666276759
            ],
            [
                92,
                233334, // self profile_id
                20,
                "",
                1663363479
            ],
            [
                93,
                233334, // self profile_id
                37,
                "",
                1664503204
            ],
            [
                94,
                233334, // self profile_id
                31,
                "",
                1664471510
            ],
            [
                95,
                233334, // self profile_id
                27,
                "",
                1664381109
            ],
            [
                96,
                233334, // self profile_id
                24,
                "",
                1663974489
            ],
            [
                97,
                233334, // self profile_id
                39,
                "",
                1666276759
            ],
            [
                98,
                233334, // self profile_id
                29,
                "",
                1664063460
            ],
            [
                99,
                233334, // self profile_id
                32,
                "",
                1666118987
            ],
            [
                100,
                233334, // self profile_id
                26,
                "",
                1663974490
            ],
            [
                101,
                233334, // self profile_id
                32,
                "",
                1666042834
            ],
            [
                102,
                233334, // self profile_id
                30,
                "",
                1666307388
            ],
            [
                103,
                233334, // self profile_id
                22,
                "",
                1666051855
            ],
            [
                104,
                233334, // self profile_id
                423,
                "",
                1637072710
            ],
            [
                105,
                233334, // self profile_id
                4119,
                "",
                1608164245
            ],
            [
                106,
                233334, // self profile_id
                2713,
                "",
                1608164245
            ],
            [
                107,
                233334, // self profile_id
                35,
                "",
                1607513748
            ],
            [
                108,
                233334, // self profile_id
                520,
                "",
                1636226889
            ],
            [
                109,
                233334, // self profile_id
                125,
                "",
                1655582189
            ],
            [
                111,
                233334, // self profile_id
                2956,
                "",
                1666388280
            ],
            [
                142,
                233334, // self profile_id
                778,
                "",
                1666384615
            ],
            [
                143,
                233334, // self profile_id
                692,
                "",
                1666384615
            ],
            [
                144,
                233334, // self profile_id
                79,
                "",
                1662901421
            ],
            [
                153,
                233334, // self profile_id
                1561,
                "",
                1666387884
            ],
            [
                154,
                233334, // self profile_id
                340,
                "",
                1666300821
            ],
            [
                155,
                233334, // self profile_id
                78967,
                "",
                1666388135
            ],
            [
                156,
                233334, // self profile_id
                684,
                "",
                1666388285
            ],
            [
                157,
                233334, // self profile_id
                18,
                "",
                1666303875
            ],
            [
                158,
                233334, // self profile_id
                136628,
                "",
                1663166307
            ],
            [
                159,
                233334, // self profile_id
                2776,
                "",
                1663064929
            ],
            [
                160,
                233334, // self profile_id
                450,
                "",
                1621969170
            ],
            [
                161,
                233334, // self profile_id
                17,
                "",
                1609152796
            ],
            [
                163,
                233334, // self profile_id
                34,
                "",
                1621851397
            ],
            [
                165,
                233334, // self profile_id
                340,
                "",
                1666388280
            ],
            [
                166,
                233334, // self profile_id
                50925,
                "",
                1666388280
            ],
            [
                167,
                233334, // self profile_id
                2,
                "",
                1657469778
            ],
            [
                168,
                233334, // self profile_id
                1,
                "",
                1574923527
            ],
            [
                171,
                233334, // self profile_id
                1,
                "",
                1574923528
            ],
            [
                172,
                233334, // self profile_id
                61,
                "",
                1574923528
            ],
            [
                173,
                233334, // self profile_id
                1,
                "",
                1574923522
            ],
            [
                174,
                233334, // self profile_id
                5,
                "",
                1666118987
            ],
            [
                175,
                233334, // self profile_id
                1,
                "",
                1664313298
            ],
            [
                176,
                233334, // self profile_id
                4,
                "",
                1662456235
            ],
            [
                177,
                233334, // self profile_id
                9,
                "",
                1664326346
            ],
            [
                184,
                233334, // self profile_id
                5,
                "",
                1660821771
            ],
            [
                185,
                233334, // self profile_id
                2,
                "",
                1642790182
            ],
            [
                186,
                233334, // self profile_id
                8,
                "",
                1666388280
            ],
            [
                187,
                233334, // self profile_id
                17,
                "",
                1666118987
            ],
            [
                194,
                233334, // self profile_id
                23490,
                "",
                1660821771
            ],
            [
                195,
                233334, // self profile_id
                4,
                "",
                1663434019
            ],
            [
                196,
                233334, // self profile_id
                4,
                "",
                1663899427
            ],
            [
                197,
                233334, // self profile_id
                7,
                "",
                1666051855
            ],
            [
                198,
                233334, // self profile_id
                5,
                "",
                1666388280
            ],
            [
                199,
                233334, // self profile_id
                1,
                "",
                1664063460
            ],
            [
                200,
                233334, // self profile_id
                2,
                "",
                1664116487
            ],
            [
                2000,
                233334, // self profile_id
                12,
                "",
                1662900124
            ],
            [
                2001,
                233334, // self profile_id
                12,
                "",
                1662900501
            ],
            [
                2002,
                233334, // self profile_id
                12,
                "",
                1662901335
            ],
            [
                2007,
                233334, // self profile_id
                13,
                "",
                1633486933
            ],
            [
                2008,
                233334, // self profile_id
                13,
                "",
                1633486934
            ],
            [
                2009,
                233334, // self profile_id
                13,
                "",
                1633486934
            ],
            [
                2010,
                233334, // self profile_id
                13,
                "",
                1633486934
            ],
            [
                2011,
                233334, // self profile_id
                13,
                "",
                1633486934
            ],
            [
                2012,
                233334, // self profile_id
                13,
                "",
                1633486934
            ],
            [
                2013,
                233334, // self profile_id
                13,
                "",
                1633486934
            ],
            [
                2014,
                233334, // self profile_id
                12,
                "",
                1633486934
            ],
            [
                2015,
                233334, // self profile_id
                13,
                "",
                1633486934
            ],
            [
                2016,
                233334, // self profile_id
                12,
                "",
                1633486934
            ],
            [
                2017,
                233334, // self profile_id
                12,
                "",
                1633486934
            ],
            [
                2021,
                233334, // self profile_id
                12,
                "",
                1633486934
            ],
            [
                2022,
                233334, // self profile_id
                12,
                "",
                1633486934
            ],
            [
                2031,
                233334, // self profile_id
                12,
                "",
                1633486934
            ],
            [
                2036,
                233334, // self profile_id
                10,
                "",
                1633486934
            ],
            [
                2054,
                233334, // self profile_id
                12,
                "",
                1638094101
            ],
            [
                2055,
                233334, // self profile_id
                12,
                "",
                1638097571
            ],
            [
                2105,
                233334, // self profile_id
                12,
                "",
                1633486934
            ],
            [
                2106,
                233334, // self profile_id
                12,
                "",
                1633486934
            ],
            [
                2107,
                233334, // self profile_id
                12,
                "",
                1633486934
            ],
            [
                2137,
                233334, // self profile_id
                12,
                "",
                1638082852
            ],
            [
                2142,
                233334, // self profile_id
                12,
                "",
                1633486934
            ],
            [
                2143,
                233334, // self profile_id
                12,
                "",
                1633486934
            ],
            [
                2144,
                233334, // self profile_id
                12,
                "",
                1633486935
            ],
            [
                2147,
                233334, // self profile_id
                12,
                "",
                1633486935
            ],
            [
                2162,
                233334, // self profile_id
                12,
                "",
                1633486935
            ],
            [
                2163,
                233334, // self profile_id
                20,
                "",
                1633486935
            ],
            [
                2164,
                233334, // self profile_id
                12,
                "",
                1633486935
            ],
            [
                2190,
                233334, // self profile_id
                12,
                "",
                1633486935
            ],
            [
                2191,
                233334, // self profile_id
                12,
                "",
                1633486935
            ],
            [
                2192,
                233334, // self profile_id
                12,
                "",
                1633486935
            ],
            [
                2193,
                233334, // self profile_id
                12,
                "",
                1633486935
            ],
            [
                2196,
                233334, // self profile_id
                12,
                "",
                1633486935
            ],
            [
                2197,
                233334,
                12,
                "",
                1633486935
            ],
            [
                2198,
                233334, // self profile_id
                12,
                "",
                1633486935
            ],
            [
                2199,
                233334, // self profile_id
                20,
                "",
                1633486935
            ]
        ],
        null,
        [],
        null,
        1,
        []
    ],
    [],
    0,
    [
        [
            "brazilsouth",
            null,
            "20.206.146.43",
            27017,
            27117,
            27217
        ],
        [
            "australiasoutheast",
            null,
            "20.190.102.29",
            27017,
            27117,
            27217
        ],
        [
            "ukwest",
            null,
            "20.254.139.124",
            27014,
            27114,
            27214
        ],
        [
            "westindia",
            null,
            "52.183.137.243",
            27014,
            27114,
            27214
        ],
        [
            "southeastasia",
            null,
            "20.24.57.9",
            27013,
            27113,
            27213
        ],
        [
            "westeurope",
            null,
            "20.56.7.169",
            27015,
            27115,
            27215
        ],
        [
            "eastus",
            null,
            "20.121.139.95",
            27019,
            27119,
            27219
        ],
        [
            "koreacentral",
            null,
            "20.214.220.152",
            27015,
            27115,
            27215
        ],
        [
            "westus2",
            null,
            "20.120.161.1",
            27014,
            27114,
            27214
        ]
    ]
]
```

## AoE3:DE

### Request

```
POST /game/login/platformlogin?accountType=STEAM&activeMatchId=-1&alias=name&appID=933110&auth=CAEQh%2Bj4ow8YBSA%2FKnAmuq9rzcobxqDg3AFvfjRC2IBYyVd6iXfEF0EKrPGSX0hYLJ2E8jhAoQV%2BH2NvRA6ajMGyLAmzedvc%2FW7W4NXIzqPLPab9EajKPF6RccEpPKVYf%2FSYHCHhnl%2FV5oICSgVCBo5vD117SY6zihCjrCEo&callNum=0&clientLibVersion=162&connect_id=&country=DE&installationType=windows&language=en&lastCallTime=24649260&macAddress=D8-BB-C1-53-39-29&majorVersion=4.0.0&minorVersion=4&platformUserID=76561199333331480&startGameToken=&syncHash=%5B0%2C0%5D&timeoutOverride=0&title=age3 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: deflate, gzip
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 525

accountType=STEAM&activeMatchId=-1&alias=name&appID=933110&auth=CAEQh+j4ow8YBSA/KnAmuq9rzcobxqDg3AFvfjRC2IBYyVd6iXfEF0EKrPGSX0hYLJ2E8jhAoQV+H2NvRA6ajMGyLAmzedvc/W7W4NXIzqPLPab9EajKPF6RccEpPKVYf/SYHCHhnl/V5oICSgVCBo5vD117SY6zihCjrCEo&callNum=0&clientLibVersion=162&connect_id=&country=DE&installationType=windows&language=en&lastCallTime=24649260&macAddress=D8-BB-C1-53-39-29&majorVersion=4.0.0&minorVersion=4&platformUserID=76561199333331480&startGameToken=&syncHash=[0,0]&timeoutOverride=0&title=age3
```

| parameter        | type               | value   | comments    |
| ---------------- | ------------------ | ------- | ----------- |
| accountType      | str/enum           | STEAM   |             |
| activeMatchId    | int                | -1      |             |
| alias            | str                | name    |             |
| appID            | int                | 933110  |             |
| auth             | str                | authzzz |             |
| callNum          | int                | 0       | 0 = initial |
| clientLibVersion | int                | 169     |             |
| connect_id       | str                | None    |             |
| country          | ISO 3166-1 Alpha-2 | US      |             |
| installationType | str/enum           | windows |             |
| language         | str                | en      |             |
| lastCallTime     | timestamp          | 111     |             |
| macAddress       | str                | mac     |             |
| majorVersion     | semVer             | 4.0.0   |             |
| minorVersion     | int                | 4       |             |
| platformUserID   | int                | 666     | STEAM_ID    |
| startGameToken   | str                | None    |             |
| syncHash         | array[int]         | [0,0]   |             |
| timeoutOverride  | int/bool           | 0       |             |
| title            | str/enum           | age3    |             |

### Response

```
[
    0,
    "fflxvvhtmtcx7tmbxff2kauyfdq8n3",
    843084731,
    1666811025,
    [
        9655757,
        "/steam/76561199333331480",
        3,
        -1,
        0,
        "de",
        "eur",
        2,
        null
    ],
    [
        [
            20,
            9652381,
            "/steam/76561199333331480",
            "",
            "steam.aoe3",
            "",
            2075838,
            0,
            1,
            0,
            null,
            "76561199333331480",
            3,
            []
        ]
    ],
    0,
    0,
    null,
    [
        [
            "RL_USE_WEBSOCKET_PERCENT",
            "100"
        ],
        [
            "RL_KEEPALIVE",
            "20"
        ],
        [
            "RL_DISCONNECT",
            "30"
        ],
        [
            "RL_MISSPOLL",
            "3"
        ],
        [
            "RL_TELEMSERVICE",
            "0"
        ],
        [
            "RL_TELEMREPORTPCT",
            "1.0"
        ],
        [
            "RL_MATCHTELEMPERIOD",
            "600"
        ],
        [
            "RL_TELEMKINESISID",
            "AKIATP3EMETR5VNBZMKA"
        ],
        [
            "RL_TELEMKINESISKEY",
            "kbduLAQls86v4Q2+yMzESocLldrah6WAowEv8IYW"
        ],
        [
            "RL_TELEMKINESISHOST",
            "kinesis.us-east-1.amazonaws.com"
        ],
        [
            "RL_TELEMKINESISSTREAM",
            "s3DevStream"
        ],
        [
            "RL_TELEMCELLHOST",
            "boston.maelstrom.gameservices.xboxlive.com"
        ],
        [
            "RL_TELEMCELLPATH",
            "/tenants/boston/routes/steam/"
        ],
        [
            "RL_CLUSTERNAME",
            "aoelive_"
        ],
        [
            "RL_TITLEID",
            "25"
        ],
        [
            "RL_OBSERVERCUSTOMDELAY",
            "180"
        ],
        [
            "RL_OBSERVERMAX",
            "0"
        ],
        [
            "RL_USE_AUTOMATCH2",
            "1"
        ],
        [
            "RL_AUTOMATCH2_TEAM_FACTION_TYPE",
            "1"
        ],
        [
            "RL_UPLOAD_TIMEOUT",
            "300000"
        ],
        [
            "RL_CLOUDCACHETIME",
            "21600"
        ],
        [
            "RL_CLOUD_CREDENTIAL_PROVIDER",
            "AZURE"
        ],
        [
            "RL_ITEM_LOADOUTS_MAX",
            "50"
        ],
        [
            "RL_CLAN_INVITE_EXPIRE_TIME_SEC",
            "43200"
        ],
        [
            "RL_NUMBER_OF_GAMES_TO_RANK",
            "10"
        ],
        [
            "RL_NUMBER_OF_EVENT_GAMES_TO_RANK",
            "5"
        ],
        [
            "RL_SECURE_TITLE",
            "1"
        ],
        [
            "RL_WEB_ASSETS_ICONS_ROOT",
            "https://test-build-data.worldsedgelink.com/"
        ],
        [
            "RL_SSO_URL",
            "https://sso.relic.com/en/steam?title=age3&"
        ]
    ],
    [
        0,
        [
            20,
            9652381,
            "/steam/76561199333331480",
            "",
            "steam.aoe3",
            "",
            2075838,
            0,
            1,
            0,
            null,
            "76561199333331480",
            3,
            []
        ],
        [
            0,
            [],
            [],
            [],
            [],
            [],
            [],
            []
        ],
        [],
        [],
        null,
        [],
        null,
        1,
        []
    ],
    [],
    0,
    [
        [
            "brazilsouth",
            null,
            "20.206.146.44",
            27012,
            27112,
            27212
        ],
        [
            "australiasoutheast",
            null,
            "20.190.102.18",
            27012,
            27112,
            27212
        ],
        [
            "ukwest",
            null,
            "20.254.139.134",
            27012,
            27112,
            27212
        ],
        [
            "westindia",
            null,
            "52.183.137.243",
            27012,
            27112,
            27212
        ],
        [
            "southeastasia",
            null,
            "20.24.57.9",
            27012,
            27112,
            27212
        ],
        [
            "westeurope",
            null,
            "20.224.64.25",
            27012,
            27112,
            27212
        ],
        [
            "eastus",
            null,
            "20.121.50.102",
            27012,
            27112,
            27212
        ],
        [
            "koreacentral",
            null,
            "20.214.220.153",
            27012,
            27112,
            27212
        ],
        [
            "westus2",
            null,
            "20.120.170.40",
            27012,
            27112,
            27212
        ]
    ]
]
```

## AoE4

### Request

```
POST /game/login/platformlogin HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cache-Control: no-store
Content-Length: 584
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

accountType=STEAM&activeMatchId=-1&alias=NAME&appID=1466860&auth=CAEQ8r/r2AwYBSBLKoABBvLEPiLC/jFgMWrApLt1wEVq/gNVsjg/mrmECUAQM5669cvmj8SxWM9wLNBzjZCyVJqlocVi/4hIU7il2ToQoiiLOiWuURy2ebX/AEcd8jS/iqMGZW6qIdoT9eumDueQOyKw4cH26mSVc3/bLRi2sf0vThM2dkt3eQ4Mnfr5xQs=&callNum=0&clientLibVersion=176&connect_id=&country=DE&installationType=windows&language=en&lastCallTime=631095&macAddress=D4-BA-A1-43-29-19&majorVersion=4.0.0&minorVersion=24916&platformUserID=765613333337299&startGameToken=&storeLicenseToken=&storetoken=&syncHash=[0,0]&timeoutOverride=0&title=age4
```

| parameter         | type               | value   | comments    |
| ----------------- | ------------------ | ------- | ----------- |
| accountType       | str/enum           | STEAM   |             |
| activeMatchId     | int                | -1      |             |
| alias             | str                | name    |             |
| appID             | int                | 1466860 |             |
| auth              | str                | authzzz |             |
| callNum           | int                | 0       | 0 = initial |
| clientLibVersion  | int                | 169     |             |
| connect_id        | str                | None    |             |
| country           | ISO 3166-1 Alpha-2 | US      |             |
| installationType  | str/enum           | windows |             |
| language          | str                | en      |             |
| lastCallTime      | timestamp          | 111     |             |
| macAddress        | str                | mac     |             |
| majorVersion      | semVer             | 4.0.0   |             |
| minorVersion      | int                | 0       |             |
| platformUserID    | int                | 666     | STEAM_ID    |
| startGameToken    | str                | None    |             |
| storeLicenseToken | str                | None    |             |
| syncHash          | array[int]         | [0,0]   |             |
| timeoutOverride   | int/bool           | 0       |             |
| title             | str/enum           | age4    |             |

### Response

```
[
    0,
    "bgoo2n1murnn43kzdnnfc9fhp2no19",
    843160633,
    1666823720,
    [
        234629,
        "/steam/76561197333337299",
        3,
        -1,
        0,
        "de",
        "eur",
        2,
        null
    ],
    [
        [
            3,
            233334,
            "/steam/7656119333337299",
            "",
            "Name",
            "",
            4275156,
            0,
            1,
            0,
            null,
            "7656119333337299",
            3,
            []
        ]
    ],
    0,
    0,
    null,
    [
        [
            "RL_TELEMSHOULDNTSEND",
            "animation_played_count,CommandIssued,MusicIntensity,ResourcePosition,UnitContribution,InfluenceUpdate,MarketTrade,BuildOrder"
        ],
        [
            "RL_BATTLESERVER_USE_WEBSOCKETS",
            "1"
        ],
        [
            "RL_HEARTBEATINTERVAL",
            "60"
        ],
        [
            "CLIENT_AUTOMATCH_WIN_CONDITION",
            "00000000000000000000000000000000:149419911"
        ],
        [
            "CLIENT_AUTOMATCH_WIN_CONDITION_OPTIONS",
            "{\"section_diplomacy\":{\"option_diplomacy\":0,\"option_diplomacy_tribute\":0},\"section_inner_win_conditions\":{\"option_win_condition_capture_point\":0,\"option_win_condition_conquest\":1,\"option_win_condition_religious\":0},\"section_starting_conditions\":{\"option_age_start\":3}}"
        ],
        [
            "CLIENT_AUTOMATCH_MAP",
            "cdn_empty_mp"
        ],
        [
            "CLIENT_AUTOMATCH_RACE",
            "french"
        ],
        [
            "RL_HEARTBEATPERFORMANCEINTERVAL",
            "300"
        ],
        [
            "RL_OBSERVERMAX",
            "256"
        ],
        [
            "RL_USE_WEBSOCKET_PERCENT",
            "100"
        ],
        [
            "RL_KEEPALIVE",
            "20"
        ],
        [
            "RL_DISCONNECT",
            "30"
        ],
        [
            "RL_MISSPOLL",
            "3"
        ],
        [
            "RL_TELEMSERVICE",
            "0"
        ],
        [
            "RL_TELEMREPORTPCT",
            "1.0"
        ],
        [
            "RL_MATCHTELEMPERIOD",
            "600"
        ],
        [
            "RL_TELEMKINESISID",
            "AKIATP3EMETR5VNBZMKA"
        ],
        [
            "RL_TELEMKINESISKEY",
            "kbduLAQls86v4Q2+yMzESocLldrah6WAowEv8IYW"
        ],
        [
            "RL_TELEMKINESISHOST",
            "kinesis.us-east-1.amazonaws.com"
        ],
        [
            "RL_TELEMKINESISSTREAM",
            "s3DevStream"
        ],
        [
            "RL_TELEMCELLHOST",
            "cardinal.maelstrom.gameservices.xboxlive.com"
        ],
        [
            "RL_TELEMCELLPATH",
            "/tenants/cardinal/routes/steam/"
        ],
        [
            "RL_CLUSTERNAME",
            "aoelive_"
        ],
        [
            "RL_TITLEID",
            "23"
        ],
        [
            "RL_OBSERVERCUSTOMDELAY",
            "180"
        ],
        [
            "RL_OBSERVERMAX",
            "0"
        ],
        [
            "RL_USE_AUTOMATCH2",
            "1"
        ],
        [
            "RL_AUTOMATCH2_TEAM_FACTION_TYPE",
            "1"
        ],
        [
            "RL_UPLOAD_TIMEOUT",
            "300000"
        ],
        [
            "RL_CLOUDCACHETIME",
            "21600"
        ],
        [
            "RL_CLOUD_CREDENTIAL_PROVIDER",
            "AZURE"
        ],
        [
            "RL_ITEM_LOADOUTS_MAX",
            "50"
        ],
        [
            "RL_CLAN_INVITE_EXPIRE_TIME_SEC",
            "43200"
        ],
        [
            "RL_NUMBER_OF_GAMES_TO_RANK",
            "10"
        ],
        [
            "RL_NUMBER_OF_EVENT_GAMES_TO_RANK",
            "5"
        ],
        [
            "RL_SECURE_TITLE",
            "1"
        ],
        [
            "RL_WEB_ASSETS_ICONS_ROOT",
            "https://test-build-data.worldsedgelink.com/"
        ],
        [
            "RL_SSO_URL",
            "https://sso.relic.com/en/steam?title=age4&"
        ]
    ],
    [
        0,
        [
            3,
            233334, // self profile_id
            "/steam/76561197333337299", // self steam_id
            "",
            "Name", // self steam_name
            "",
            4275156,
            0,
            1,
            0,
            null,
            "76561197333337299", // self steam_id64
            3,
            []
        ],
        [
            0,
            [],
            [],
            [],
            [],
            [],
            [],
            []
        ],
        [],
        [],
        null,
        [],
        null,
        1,
        []
    ],
    [],
    0,
    [
        [
            "brazilsouth",
            "Brazil",
            "20.206.146.43",
            27013,
            27113,
            27213
        ],
        [
            "australiasoutheast",
            "Australia",
            "20.190.102.29",
            27016,
            27116,
            27216
        ],
        [
            "ukwest",
            "UK",
            "20.254.139.130",
            27016,
            27116,
            27216
        ],
        [
            "westindia",
            "India",
            "52.183.138.208",
            27018,
            27118,
            27218
        ],
        [
            "southeastasia",
            "Asia (SE)",
            "20.198.221.182",
            27016,
            27116,
            27216
        ],
        [
            "westeurope",
            "Europe (W)",
            "51.124.115.49",
            27017,
            27117,
            27217
        ],
        [
            "eastus",
            "USA (E)",
            "20.84.123.139",
            27014,
            27114,
            27214
        ],
        [
            "koreacentral",
            "Korea",
            "20.214.220.160",
            27014,
            27114,
            27214
        ],
        [
            "westus2",
            "USA (W)",
            "20.120.160.74",
            27015,
            27115,
            27215
        ]
    ]
]
```
