# [POST] /game/automatch2/polling

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/automatch2/polling HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 791
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

appBinCRC=9876&callNum=123&connect_id=ccc&dataCRC=6789&factionIDs=[0,0,0,0]&lastCallTime=111&matchTypes=[20,21,22,23]&modDLLFile=INVALID&modDllCRC=0&modName=INVALID&modVersion=INVALID&options=["","","",""]&partySessionID=444&raceInfoKey=[0,1,2,3]&raceInfoProfileID=[1,1,1,1]&raceInfoRaceID=[8,8,8,8]&relayPingTimes=[1,1,2,2,3,3,4,4,5]&relayRegion=eastus&relayRegions=["westeurope","ukwest","australiasoutheast","westindia","eastus","southeastasia","brazilsouth","westus2","koreacentral"]&sessionID=zzz&versionFlags=0
```

| parameter         | type            | value                                                                                                                    | comments             |
| ----------------- | --------------- | ------------------------------------------------------------------------------------------------------------------------ | -------------------- |
| appBinCRC         | CRC             | 9876                                                                                                                     |                      |
| callNum           | int             | 123                                                                                                                      |                      |
| connect_id        | str             | ccc                                                                                                                      |                      |
| dataCRC           | int             | 6789                                                                                                                     | backwards appBinCRC? |
| factionIDs        | array[int]      | [0,0,0,0]                                                                                                                |                      |
| lastCallTime      | int             | 111                                                                                                                      |                      |
| matchTypes        | array[int]      | [20,21,22,23]                                                                                                            |                      |
| modDLLFile        | ?               | INVALID                                                                                                                  |                      |
| modDllCRC         | int             | 0                                                                                                                        |                      |
| modName           | str             | INVALID                                                                                                                  |                      |
| modVersion        | int             | INVALID                                                                                                                  |                      |
| options           | array[str]      | ["","","",""]                                                                                                            |                      |
| partySessionID    | int             | 444                                                                                                                      |                      |
| raceInfoKey       | array[int]      | [0,1,2,3]                                                                                                                |                      |
| raceInfoProfileID | array[int]      | [1,1,1,1]                                                                                                                |                      |
| raceInfoRaceID    | array[int]      | [8,8,8,8]                                                                                                                |                      |
| relayPingTimes    | array[int]      | [1,1,2,2,3,3,4,4,5]                                                                                                      |                      |
| relayRegion       | str/enum        | eastus                                                                                                                   |                      |
| relayRegions      | array[str/enum] | ["westeurope","ukwest","australiasoutheast","westindia","eastus","southeastasia","brazilsouth","westus2","koreacentral"] |                      |
| sessionID         | str             | zzz                                                                                                                      |                      |
| versionFlags      | int             | 0                                                                                                                        |                      |

### Response

```
[
    0, // result status code
    [
        [
            "6",
            55,
            [
                [
                    0,
                    55
                ]
            ],
            "0"
        ]
    ],
    93826,
    null,
    233334,
    "Yucatan.rms", // map_name
    0,
    0,
    0,
    "2",
    "1",
    "6",
    186444398,
    "authtoken",
    "51.141.99.39", // matchmaking server ip?
    27014,
    27114,
    27214,
    "ukwest", // server location
    [
        [
            186444398,
            233334, // self player_id
            -1,
            33833,
            0,
            0,
            "/10.0.11.6"
        ],
        [
            186444398,
            4994658,
            31286,
            4037175,
            0,
            1,
            "/10.0.11.8"
        ]
    ],
    "",
    225
]
```

## AoE4

### Request

```
POST /game/automatch2/polling HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 2186
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Expect: 100-continue

appBinCRC=24916&callNum=275&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&dataCRC=-638535971&factionIDs=[0,0,0,0]&lastCallTime=3026838&matchTypes=[20,21,22,23]&modDLLFile=INVALID&modDllCRC=0&modName=INVALID&modVersion=INVALID&options=["","","",""]&partySessionID=50865084&raceInfoKey=[0,1,2,3]&raceInfoProfileID=[233334,233334,233334,233334]&raceInfoRaceID=[2039321,2039321,2039321,2039321]&relayPingTimes=[264,220,253,45,187,191,153,45,119]&relayRegion=ukwest&relayRegions=["australiasoutheast","brazilsouth","koreacentral","ukwest","southeastasia","westus2","westindia","westeurope","eastus"]&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&versionFlags=0&vetoMapKey=[0,0,0,0,0,0,0,0,0,0,0,0,1,1,1,1,1,1,1,1,1,1,1,1,2,2,2,2,2,2,2,2,2,2,2,2,3,3,3,3,3,3,3,3,3,3,3,3]&vetoMaps=["hideout_tiny","hideout_small","hideout_medium","hideout_large","archipelago_medium","high_view_small","archipelago_large","high_view_medium","archipelago_gigantic","high_view_large","archipelago_small","high_view_tiny","hideout_tiny","hideout_small","hideout_medium","hideout_large","archipelago_medium","high_view_small","archipelago_large","high_view_medium","archipelago_gigantic","high_view_large","archipelago_small","high_view_tiny","hideout_tiny","hideout_small","hideout_medium","hideout_large","archipelago_medium","high_view_small","archipelago_large","high_view_medium","archipelago_gigantic","high_view_large","archipelago_small","high_view_tiny","hideout_tiny","hideout_small","hideout_medium","hideout_large","archipelago_medium","high_view_small","archipelago_large","high_view_medium","archipelago_gigantic","high_view_large","archipelago_small","high_view_tiny"]
```

| parameter         | type            | value                                                                                                                    | comments |
| ----------------- | --------------- | ------------------------------------------------------------------------------------------------------------------------ | -------- |
| appBinCRC         | CRC             | 9876                                                                                                                     |          |
| callNum           | int             | 123                                                                                                                      |          |
| connect_id        | str             | ccc                                                                                                                      |          |
| dataCRC           | int             | 6789                                                                                                                     |          |
| factionIDs        | array[int]      | [0,0,0,0]                                                                                                                |          |
| lastCallTime      | int             | 111                                                                                                                      |          |
| matchTypes        | array[int]      | [20,21,22,23]                                                                                                            |          |
| modDLLFile        | ?               | INVALID                                                                                                                  |          |
| modDllCRC         | int             | 0                                                                                                                        |          |
| modName           | str             | INVALID                                                                                                                  |          |
| modVersion        | int             | INVALID                                                                                                                  |          |
| options           | array[str]      | ["","","",""]                                                                                                            |          |
| partySessionID    | int             | 444                                                                                                                      |          |
| raceInfoKey       | array[int]      | [0,1,2,3]                                                                                                                |          |
| raceInfoProfileID | array[int]      | [1,1,1,1]                                                                                                                |          |
| raceInfoRaceID    | array[int]      | [8,8,8,8]                                                                                                                |          |
| relayPingTimes    | array[int]      | [1,1,2,2,3,3,4,4,5]                                                                                                      |          |
| relayRegion       | str/enum        | eastus                                                                                                                   |          |
| relayRegions      | array[str/enum] | ["westeurope","ukwest","australiasoutheast","westindia","eastus","southeastasia","brazilsouth","westus2","koreacentral"] |          |
| sessionID         | str             | zzz                                                                                                                      |          |
| versionFlags      | int             | 0                                                                                                                        |          |
| vetoMapKey        | arr[int]        | [0,0,0,1,1,1,0]                                                                                                          |          |
| vetoMaps          | arr[int]        | ["hideout_tiny","hideout_small","hideout_medium","..."                                                                   |          |

### Response

```
[
    0,
    [
        [
            "20",
            20,
            [
                [
                    137266,
                    1
                ],
                [
                    129267,
                    2
                ],
                [
                    199703,
                    2
                ],
                [
                    2039321,
                    4
                ],
                [
                    2058393,
                    6
                ],
                [
                    106553,
                    3
                ],
                [
                    131384,
                    2
                ]
            ],
            "0"
        ],
        [
            "21",
            20,
            [
                [
                    137266,
                    1
                ],
                [
                    133008,
                    2
                ],
                [
                    129267,
                    2
                ],
                [
                    199703,
                    2
                ],
                [
                    136150,
                    1
                ],
                [
                    2039321,
                    3
                ],
                [
                    2058393,
                    6
                ],
                [
                    106553,
                    2
                ],
                [
                    134522,
                    1
                ],
                [
                    131384,
                    3
                ]
            ],
            "0"
        ],
        [
            "22",
            32,
            [
                [
                    137266,
                    2
                ],
                [
                    133008,
                    1
                ],
                [
                    129267,
                    2
                ],
                [
                    199703,
                    3
                ],
                [
                    136150,
                    1
                ],
                [
                    2039321,
                    9
                ],
                [
                    2058393,
                    10
                ],
                [
                    106553,
                    5
                ],
                [
                    134522,
                    3
                ],
                [
                    131384,
                    5
                ]
            ],
            "0"
        ],
        [
            "23",
            32,
            [
                [
                    137266,
                    2
                ],
                [
                    129267,
                    2
                ],
                [
                    199703,
                    1
                ],
                [
                    136150,
                    1
                ],
                [
                    2039321,
                    10
                ],
                [
                    2058393,
                    11
                ],
                [
                    106553,
                    6
                ],
                [
                    131384,
                    3
                ]
            ],
            "0"
        ]
    ],
    88302,
    null,
    -1,
    "",
    -1,
    -1,
    -1,
    "0",
    "0",
    "-1",
    -1,
    "authtoken",
    "0.0.0.0",
    0,
    0,
    0,
    "",
    [],
    null,
    0
]
```
