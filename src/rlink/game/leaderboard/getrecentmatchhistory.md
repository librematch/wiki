# [GET/POST] /game/Leaderboard/getRecentMatchHistory

**AUTHENTICATION**

**AoE3:DE POST REQUEST!**

## AoE2:DE

### Request

```
GET /game/Leaderboard/getRecentMatchHistory?callNum=123&connect_id=ccc&lastCallTime=111&profile_ids=[1,1]&sessionID=zzz HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type       | value              | comments |
| ------------ | ---------- | ------------------ | -------- |
| callNum      | int        | 123                |          |
| connect_id   |            |                    |          |
| lastCallTime | timestamp  |                    |          |
| sessionID    | str        |                    |          |
| profile_ids  | array[int] | [2132331,31323213] |          |

### Response (Basic)

```
[
    0, // result status code
    [
        [
            125793154, // match_id
            1627373,
            "my map",
            8,
            0,
            // zlib compressed settings 
            "eNpFUl1vgzAM/C/9BXxG2iNV0oluTsQUNLHHsipa2AqaNEH49XMSp+XpFN+dzzaHznQNfgXYOWtWRLxh0NDbvvwdPeTTpiyssS7YJWoqaZc6vrUMOtLoeT16xIdV2UZ4qLhBDXiY49vFA6mBvWXV7yX7fL2ezi/APyS8n3U/ze56W757nT1F7wHz9EGLGUugvFJjttDHZI8+PbvGHKWyYx71JmXL5T47ylaonypopB1RE7LVynbhDbTfweDhhvNskgvi3r0Kpec8eo04Zx/ru8B6yFpi1o1yb7DPOe0UveYt7lTgLsb1aAIulBVOdsTZkRO8RaWsoUwTepvojXXgzUqeDnjaeYt3EqfAty2TtBewwMCELA77FzRb6bOA7YnfM7jzhzSHwywF7dwpPu80M2Y3z5E7eR31hzLdQu5DukUNPN0Kqkd9TP9RLm2at3PKtnTLKdVLxZea+tbqNkW9Nuk/rYJ/2KnZ1FdGXga9JvKCxM3xbu7wD8aB4/c=",
            // zlib compressed player data 
            "eNrN1F1rgzAUBuD9lly7kRw10cJuuk5wrB/a2ZWNXYQamVi1qBuUsf8+DS0ubBl45a4Sc4Lh4c0JAeP5Ax2qMkn3wi+S8iqN0YRQYCYzDVQ3vEnLwp+1awZqBM+7KTZQwnfnQvtV8Z3opibt5kV2L97F/lQpsjlvdq8Px4Pcctn9J83FSlRexXMxX8t9aR0KHh/lMd2hb7VczkXDZ7zhaIL8zDPDyJsGkWcFj3E33kbbeBrJtXAaZLK2iDZyvNlsDtuwCM91b7X2r9Gn8RNrYYKZ6SpY6LFEhyXjW5/IQCthNnNtUINlPRa0WDa6dhkMTdZ2XQuAqlqn15paLR4/2/j3bO+0WgBCwCGK1u6xlg4L41/k5eCmJQzj9jIrWNpjbW2y/wCr6dqFPlnboZQpVre3Uq3VHf8WD+5ZChjaR0rt2W9aptVa4ycb//kev1x8AchgSzY=",
            "FFA Land Nomad (all random)", // name
            1635439384, // started
            1635446922, // finished
            0,
            [
                [
                    125793154,
                    1627373, // profile_id
                    0, // won
                    0,
                    36,
                    1,
                    "{}",
                    "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
                    1635439384
                ],
                [
                    125793154,
                    4010739,
                    0,
                    1,
                    1,
                    1,
                    "{}",
                    "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
                    1635439384
                ],
                [
                    125793154,
                    1757952,
                    0,
                    2,
                    17,
                    1,
                    "{}",
                    "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
                    1635439384
                ],
                [
                    125793154,
                    5994226,
                    0,
                    3,
                    10,
                    1,
                    "{}",
                    "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
                    1635439384
                ],
                [
                    125793154,
                    2211281,
                    0,
                    4,
                    21,
                    1,
                    "{}",
                    "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
                    1635439384
                ],
                [
                    125793154,
                    1700175,
                    1,
                    5,
                    11,
                    1,
                    "{}",
                    "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
                    1635439384
                ],
                [
                    125793154,
                    258667,
                    0,
                    6,
                    19,
                    1,
                    "{}",
                    "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
                    1635439384
                ],
                [
                    125793154,
                    6202757,
                    0,
                    7,
                    14,
                    1,
                    "{}",
                    "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
                    1635439384
                ]
            ],
            [],
            [],
            [
                "INVALID",
                "INVALID",
                "INVALID",
                0,
                0,
                54684,
                56950784
            ]
        ],
    ...
    ]
]
```

### Response (Match Settings)

```
// which boolean are inverted???
[
    'F',
    '62:3', // difficulty
    '0:0', // starting age
    '63:n', // full tech tree
    '93:30',
    '1:n', // allow cheats
    '88:y',
    '2:1',
    '61:0',
    '60:0',
    '90:n', // empire wars mode (inverted!)
    '5:0', // ending age
    '53:ZbSZcn1M/0msawKzRjbraw==',
    '6:0', // game mode
    '52:72',
    '65:n',
    '86:0',
    '96:',
    '1',
    '87:y',
    '7:75',
    '8:0',
    '57:2', // public or private lobby, 0 is private 2 is public
    '66:n', // lock speed
    '67:y',  // lock teams (inverted!)
    '9:4', // map size
    '10:0',
    '11:9', // location
    '94:0',
    '85:',
    '1',
    '84:',
    '1',
    '68:1',
    '69:5',
    '70:5',
    '71:1',
    '72:10',
    '13:50',
    '14:1',
    '15:70',
    '16:125',
    '17:1',
    '18:8',
    '19:1',
    '73:10000',
    '20:0',
    '21:1',
    '22:60',
    '23:2',
    '24:60',
    '74:125',
    '25:20',
    '26:1',
    '27:62',
    '28:3',
    '75:8',
    '29:150', // population
    '37:0',
    '76:y', // record game
    '92:n', // regicide mode (inverted!)
    '38:0', // resources
    '77:n', // shared exploration (inverted!)
    '56:1',
    '42:3', // speed
    '91:n', // sudden death mode (inverted!)
    '78:n', // team positions
    '79:y', // team together
    '58:5', // treaty length
    '80:n', // turbo mode (inverted!)
    '81:',
    '1',
    '82:9', // victory
    '83:0', // reveal map
    '59:2'
]
//    "39:default0.aoe2scenario" // custom scenario
//    "39:35319" // coop campaign
```

### Response (Player Data)

```
12,
[
   {
      "profileInfo.id":369536,
      "stationID":1,
      "teamID":0,
      "factionID":0,
      "raceID":9,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":1,
      "status":0,
      // double base64 encoded player info
      "metaData":"IkF3RUFBQUF3QVFBQUFERVRBQUFBVTJObGJtRnlhVzlRYkdGNVpYSkpibVJsZUFFQUFBQXhCQUFBQUZSbFlXMEJBQUFBTWc9PSI="
   },
   {
      "profileInfo.id":262049,
      "stationID":2,
      "teamID":1,
      "factionID":0,
      "raceID":21,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":1,
      "status":0,
      "metaData":"IkF3RUFBQUF3QVFBQUFEQVRBQUFBVTJObGJtRnlhVzlRYkdGNVpYSkpibVJsZUFFQUFBQXdCQUFBQUZSbFlXMEJBQUFBTXc9PSI="
   },
   {
      "profileInfo.id":270315,
      "stationID":3,
      "teamID":0,
      "factionID":0,
      "raceID":16,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":1,
      "status":0,
      "metaData":"IkF3RUFBQUF3QVFBQUFEVVRBQUFBVTJObGJtRnlhVzlRYkdGNVpYSkpibVJsZUFFQUFBQTFCQUFBQUZSbFlXMEJBQUFBTWc9PSI="
   },
   {
      "profileInfo.id":3101322,
      "stationID":4,
      "teamID":1,
      "factionID":0,
      "raceID":30,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":1,
      "status":0,
      "metaData":"IkF3RUFBQUF3QVFBQUFESVRBQUFBVTJObGJtRnlhVzlRYkdGNVpYSkpibVJsZUFFQUFBQXlCQUFBQUZSbFlXMEJBQUFBTXc9PSI="
   },
   {
      "profileInfo.id":280742,
      "stationID":6,
      "teamID":0,
      "factionID":0,
      "raceID":2,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":1,
      "status":0,
      "metaData":"IkF3RUFBQUF3QVFBQUFETVRBQUFBVTJObGJtRnlhVzlRYkdGNVpYSkpibVJsZUFFQUFBQXpCQUFBQUZSbFlXMEJBQUFBTWc9PSI="
   },
   {
      "profileInfo.id":1264695,
      "stationID":5,
      "teamID":1,
      "factionID":0,
      "raceID":24,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":1,
      "status":0,
      "metaData":"IkF3RUFBQUF3QVFBQUFEUVRBQUFBVTJObGJtRnlhVzlRYkdGNVpYSkpibVJsZUFFQUFBQTBCQUFBQUZSbFlXMEJBQUFBTXc9PSI="
   }
]
```

## AoE3:DE

### Request

```
POST /game/Leaderboard/getRecentMatchHistory?callNum=18&connect_id=fflxvvhtmtcx7tmbxff2kauyfdq8n3&lastCallTime=6989&profile_ids=%5B9655781%5D&sessionID=fflxvvhtmtcx7tmbxff2kauyfdq8n3 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: deflate, gzip
Cookie: ApplicationGatewayAffinity=29259ca9e836dd7648ed1ca403a17cde;ApplicationGatewayAffinityCORS=29259ca9e836dd7648ed1ca403a17cde;worldsedgelink=-1321719403;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 137

callNum=18&connect_id=fflxvvhtmtcx7tmbxff2kauyfdq8n3&lastCallTime=6989&profile_ids=[9655781]&sessionID=fflxvvhtmtcx7tmbxff2kauyfdq8n3
```

| parameter    | type       | value              | comments |
| ------------ | ---------- | ------------------ | -------- |
| callNum      | int        | 123                |          |
| connect_id   |            |                    |          |
| lastCallTime | timestamp  |                    |          |
| profile_ids  | array[int] | [2132331,31323213] |          |
| sessionID    | str        |                    |          |

### Response (Basic)

```
[
   0,
   // Recent Matches
   [
      [...],
      [...],
          [
      15230147,
      9146295,
      "set_landmaps",
      8,
      0,
      "eNpdkMEKwjAQRP2WnD0oeJDealEPIkjtD6zN0gbTbMmmaBH/3U1pafGWeRMmM/mo5nEv0YE3dIYGVbJZC8qRA3nUC5QRtbOMpyvpUeVYGXIqUUxdqBE4ABtQ4tyA+UVeixflFd43Cz16Vsl+jLm3iOJvJxnAB+OqtFo8dXR6Qru/e1KVOl8ijz2jl1pLr0yKBJ4zTsbKzjhAWXC6gZZjpbyzWHjQMsdRS7YfJw1YEvrCTKMju1CoZ3WwVD5h+Ibv6gd7KW/B",
      "eNq9001rwzAMBuD9Fp/dYvkjsXMug0ILo9tt7CBShZk2SUm8QRn9711CR2dYIJf59oKE/WBLIPnrFzt1beWPtG6qdun3rHCgM+kMZ33A4NtmvWIFcBYI61ussPwpCM46LGmI+RCbw4Y+6XgrNIcthvL95XwaOxbDMb6mJ+oeO6xp+zz2+X5HuD+Pebjzox9jTQFXGJAVjF34n84chIycaoZTisRQ46x1Ko+g5g6VU1Cd2glOSZ1FTjfDmf7jzfeAushp70415VSJncrYXOnYCWIGFFI/aKalEfGAwq+VF1NQkxiqwVow8cqDnLHz8K8z+vZwBa+fov4=",
      "2v2v2v2",
      1645630662,
      1645632973,
      0,
      [
        [
          15230147,
          9146295,
          0,
          1,
          7,
          0,
          "{\"rankedMatch\":0}",
          "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
          1645630662
        ],
        [
          15230147,
          9147102,
          0,
          1,
          20,
          0,
          "{\"rankedMatch\":0}",
          "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
          1645630662
        ],
        [
          15230147,
          5988937,
          0,
          2,
          4,
          0,
          "{\"rankedMatch\":0}",
          "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
          1645630662
        ],
        [
          15230147,
          5193246,
          0,
          2,
          7,
          0,
          "{\"rankedMatch\":0}",
          "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
          1645630662
        ],
        [
          15230147,
          9156299,
          1,
          3,
          3,
          0,
          "{\"rankedMatch\":0}",
          "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
          1645630662
        ],
        [
          15230147,
          3587349,
          1,
          3,
          1,
          0,
          "{\"rankedMatch\":0}",
          "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
          1645630662
        ],
        [
          15230147,
          9642507,
          0,
          0,
          5,
          0,
          "{\"rankedMatch\":0}",
          "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
          1645630662
        ],
        [
          15230147,
          4188152,
          0,
          1,
          17,
          0,
          "{\"rankedMatch\":0}",
          "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{}}",
          1645630662
        ]
      ],
      [],
      [],
      [
        "INVALID",
        "INVALID",
        "INVALID",
        0,
        1140697078,
        -1150490902,
        0
      ]
    ],
      ...
      [],
      
   ]
]
```

### Response (Match Settings)

```
{
    "mbScenarioGame":0,
    "mbRestoredGame":0,
    "mbCoopGame":0,
    "mGameMode":0,
    "mRegion":"southeastasia",
    "mPassword":"",
    "mMaxPlayers":8,
    "mGameSpeed":1,
    "mGameStartingAge":0,
    "mGameEndingAge":4,
    "mGameStartingResources":0,
    "mbGameAllowCheats":0,
    "mGameFilename":"landmaps",
    "mRuleTradeMonopoly":0,
    "mRuleTreatyTime":0,
    "mRuleKoth":0,
    "mRuleBlockade":0
}
```

### Response (Player Data)

```
12,
[
   {
      "profileInfo.id":9146295,
      "stationID":1,
      "teamID":1,
      "factionID":0,
      "raceID":17,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":0,
      "metaData":""
   },
   {
      "profileInfo.id":9147102,
      "stationID":2,
      "teamID":1,
      "factionID":0,
      "raceID":20,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":0,
      "metaData":""
   },
   {
      "profileInfo.id":5509445,
      "stationID":5,
      "teamID":2,
      "factionID":0,
      "raceID":7,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":0,
      "metaData":""
   },
   {
      "profileInfo.id":9654828,
      "stationID":6,
      "teamID":2,
      "factionID":0,
      "raceID":2,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":0,
      "metaData":""
   },
   {
      "profileInfo.id":7556510,
      "stationID":7,
      "teamID":3,
      "factionID":0,
      "raceID":11,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":0,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":3,
      "factionID":0,
      "raceID":1,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":0,
      "metaData":""
   },
   {
      "profileInfo.id":3591798,
      "stationID":10,
      "teamID":0,
      "factionID":0,
      "raceID":17,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":0,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":3,
      "factionID":0,
      "raceID":2,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":2,
      "metaData":""
   }
]
```

## AoE4

### Request

```
GET /game/Leaderboard/getRecentMatchHistory?callNum=198&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=2584339&profile_ids=%5B233334%5D&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type       | value              | comments |
| ------------ | ---------- | ------------------ | -------- |
| callNum      | int        | 123                |          |
| connect_id   |            |                    |          |
| lastCallTime | timestamp  |                    |          |
| profile_ids  | array[int] | [2132331,31323213] |          |
| sessionID    | str        |                    |          |

### Response (Basic)

```
[
   0,
   // Recent Matches
   [
      [...],
      [...],
      [
         // Current match unique id?
         22951120,
         // Relic id
         7791626,
         "generated_map",
         16,
         0,
         // Gzip / zLib compress data contains map details, mods (need to look more)
         "eNqtUdFugjAU3bfc15GMCjgw8aFM48wWdc63xSwdFEYs0EDVMeK/77Yg/sD60N5zTnvvPb0t5EzuGslhQiw4Z8ULbzB0A5cEAUEqzhIj1YpVqr7eWksdfwB9m4dg4UEpTadT2FtQFTHeIiPbtT0y8iwQZXSAiW3BMUMlIL7tuj6myZmKvk05gB49JSlMRv4Yy4lSGQRJirmfXdzCe9zov2CKvfY1N+FiiX3Bg17nnpcrlvOuMcEaXmmzeyMsePH+iwYD3xuTK/PKmvKokB07zo0NsxKpR8ch9vD09osdsdW/NcjrU2VMt5B/xkwx3cFleBvxYpgUE6I8z3/U5lDf8JbLK87LuJtRq8MNizTfXoww49L4QSSTZXHqfMpkxVUXZvXsK+1GVnMqRMaKiO84y3Xuy90f0bel5w==",
         
         // Gzip / zLib compress data contains Player details of the current match
         "eNrtVVGPojAQvt/is3eBImj3bV0FIYqKAsLlHijFiBQ0WmHxcv/9WnBXdy/mcskldyT7QGj7TWe+mU6/iqD99Xtrf9itYxLp2Xr3JcatBwV2lB4Q2q0jDWi8y/RB6wG0WzQKUj5kwDoIXwA2OwRhxIcigEDp8nmWjKM8Ihc0SyYBDTfLcl+ZfRaZrziNZtFBPQRpNFlUdvHRigJcVmMe+HSshmlEg0FAg9ZDKyoNugLkZAGV+gtdmTwVMXLgHmU+QZmVhxlZ+K6aRBxbVFiBNFX2V8Z1vd5Teq6cICAusaaWWO3nISBC4MKTvt09j59YHMkUvJXB1uTM1uA5WFl7BDrxNBZqHIi5r/Y3HqCzcMQx+axv9109fV2v5mvOw4WJpTlFWOqKK4rw3X6Nccw4duFGEbDmnmseLA1KKH3OPdeahynMwtQ513adYjJ45N+RxVuj1CG+5iRLFicUzBy7ssDyKOo4MvFdi/hDFm9kDpGET0iDG25/tXnlYqDEKVms8pLLmuWf+KvNzfqOXmr7ynPhymqYGXkY64qeqP25fe8bwtnCuOSv7m2N+QTw5LnPezxKWG31+AVbVhyhiJ90xRzosjlIgHlm/zr2Fkkm9dmZeAIssEZylE3iaXasztxzyQmr5jbQHOrbZHjNZR5Pt/NyupzL5jZkf7uqHx6RouqnkVDNQ01lPcVrTijrAZnlHI/LXj4uoTRbCjVHqb9htRFs4GzZ2Se/s3NGxh6xGHrM8V6OzwLU4+KGr0XCjOVzzw8wWD0wsbkfVy2j976ymjvWnA2y1SPSyAalJuG+LMfc8vpffaklWpG+l5Ij72t/xWpHKL7BnFDD7I4wTlXP1r4ZNxo5zont4b2NVvVZJEiQc6waLJ6VI5col1o+tn60fxWXbheKClDeiIt0FRfxrrhIHRmA/1xcFh/i8iEuH+Lyz8SF3/4bXanE4CIs4J6wCH9TU8Q3mvKnHKUGcOw0gKPcAI5KAzh2G8Cx1wCOsAEcRaEJJMUmkGzCUyM24a0Rm/DYiP/mtfn26Sf2tbeL",
         // Match name incase of custom game or AUTOMATCH if quick match
         "AUTOMATCH", 
         // Match Started Timestamp
         1642755573,
         // Match Started Timestamp
         1642756029,
         0,
         // List of players in this game
         [
            [
               22951120, // Current match uid?
               6946820, // relic id
               1,
               0, // team id
               129267, // civ id
               224,
               
               "{\"abil\":3,\"addonkill\":0,\"blost\":0,\"bprod\":1,\"cabil\":0,\"cflags\":0,\"cpearn\":0,\"dmgdone\":0,\"edeaths\":0,\"ekills\":0,\"elitekill\":0,\"erein\":0,\"gammaspnt\":0,\"gt\":437,\"inactperiod\":94,\"lowintperiod\":0,\"objdmh\":0,\"pcap\":0,\"plost\":0,\"popmax\":0,\"powearn\":0,\"powmax\":0,\"powspnt\":0,\"precap\":0,\"reqearn\":0,\"reqmax\":0,\"reqspnt\":0,\"sqkill\":0,\"sqlost\":0,\"sqprod\":4,\"structdmg\":0,\"svetrank\":0,\"svetxp\":0,\"totalcmds\":302,\"unitprod\":4,\"upg\":0,\"vabnd\":0,\"vcap\":0,\"vkill\":0,\"vlost\":0,\"vp0\":0,\"vp1\":0,\"vprod\":0,\"vvetrank\":0,\"vvetxp\":0,\"wpnpu\":0}",
               winReason
               "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{\"optionsVersion\":\"5\",\"statsVersion\":\"2004\",\"winReason\":\"Elimination\"}}",
               1642755573
            ],
            [
               22951120,
               7791626,
               0,
               1,
               134522,
               24,
               "{\"abil\":0,\"addonkill\":0,\"blost\":0,\"bprod\":2,\"cabil\":0,\"cflags\":0,\"cpearn\":0,\"dmgdone\":0,\"edeaths\":0,\"ekills\":0,\"elitekill\":0,\"erein\":0,\"gammaspnt\":0,\"gt\":437,\"inactperiod\":348,\"lowintperiod\":240,\"objdmh\":0,\"pcap\":0,\"plost\":0,\"popmax\":0,\"powearn\":0,\"powmax\":0,\"powspnt\":0,\"precap\":0,\"reqearn\":0,\"reqmax\":0,\"reqspnt\":0,\"sqkill\":0,\"sqlost\":0,\"sqprod\":0,\"structdmg\":0,\"svetrank\":0,\"svetxp\":0,\"totalcmds\":66,\"unitprod\":0,\"upg\":0,\"vabnd\":0,\"vcap\":0,\"vkill\":0,\"vlost\":0,\"vp0\":0,\"vp1\":0,\"vprod\":0,\"vvetrank\":0,\"vvetxp\":0,\"wpnpu\":0}",
               "{\"itemUpdates\":[],\"challengeUpdates\":[],\"clientUpdates\":{\"optionsVersion\":\"5\",\"statsVersion\":\"2004\",\"winReason\":\"Elimination\"}}",
               1642755573
            ]
         ],
         [
            [
               6946820,
               22951120,
               1667103,
               451704,
               0,
               1,
               "",
               2
            ],
            [
               6946820,
               22951120,
               257568664,
               453137,
               0,
               1,
               "{\"att\":{\"is_new\":{\"val\":\"0\"}}}",
               5
            ],
            [
               7791626,
               22951120,
               114708487,
               451806,
               0,
               1,
               "",
               2
            ],
            [
               7791626,
               22951120,
               249761767,
               453135,
               0,
               1,
               "{\"att\":{\"is_new\":{\"val\":\"0\"}}}",
               5
            ]
         ],
         [

         ],
         [
            "INVALID",
            "INVALID",
            "INVALID",
            0,
            725689794,
            10257,
            0
         ]
      ],
      ...
      [],
      
   ]
]
```

### Response (Match Settings)

```
{
    "mapType": 1,
    "winKey": 149419911,
    "dif": 1,
    "starts": 1,
    "winOpts": ["AQAA", "AQAAAA=="], // game setup see below
    "rnd": 3441690494,
    "lock": 0,
    "uid": 110946337,
    "matchKey": "",
    "matchCfg": 286,
    "slotCfg": "fgAAAH4AAAB+AAAAfgAAAH4AAAB+AAAAfgAAAH4AAAB+AAAAfgAAAH4AAAB+AAAAfgAAAH4AAAB+AAAAfgAAAA==",
    "matchPBGId": "/////w==",
    "mapName": "",
    "layers": [],
    "mapGenSz": 129303,
    "mapGenLayout": 163361, // map (here: dry arabia)
    "mapGenBio": 167578, // map biome
    "mapGenStarts": 1, // map team starting locations (0 = random locations)
    "mapGenRnd": 0, // map seed 8 characters (0123456789abcdef). '12a' = 256*1 + 16*2 + 1*10 = 298
    "mapGenOvrCfg": {"m_data": ""},
    "mapGenScenType": 1,
    "allowExtPks": 1,
    "allowRepPks": 1,
    "modOpts": {"modPacks": {}, "modDeps": []},
    "pfInv": "",
    "pfNet": "",
    "isDbg": 0,
    "useAllianceTeams": 1
}

NOTE: Only public games are found by findAdvertisements

// Sandbox
winOpts: [ 'AA==' ],

xA
starting res: standard=A, high=Q

// Standard
winOpts: [ 'AAAA', 'AAMBAg==' ],

AAAA
nothing

xQxx
landmarks

xxEx
sacred

xxxB
wonder

AAAAAA==

xQxxxx
display player scores: no=A, yes=Q

xxAxxx
starting res: standard=A, high=E, very high=I, maximum=M

xxxAxx
starting age: age I=A, age II=B, age III=C, age IV=D

xxxxxA
map state: concealed=A, revealed=g, explored=Q,
```

### Response (Player Data)

```
12,
[
   {
      "profileInfo.id":209525,
      "stationID":1,
      "teamID":0,
      "factionID":0,
      "raceID":131384,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":0,
      "metaData":"eyJtX2luR2FtZSI6MCwibV9pbnZlbnRvcnlSZWFkeSI6MCwibV9wbGF5ZXJSZWFkeSI6MCwibV9yYW5kb21TdGFydFBvc2l0aW9uIjoxLCJtX3N0YXJ0aW5nUG9zaXRpb24iOi0xLCJtX21vZFBhY2tPcHRpb25zIjp7Im1vZFBhY2tzIjp7fSwibW9kRGVwcyI6W119LCJtX21vZFBhY2tGbGFncyI6MCwibV9tb2RQYWNrRG93bmxvYWRQcm9ncmVzcyI6MC4wMDAwMDAsIm1fbmVlZGVkTW9kc0NvdW50IjowLCJtX25lZWRlZE1vZHNEb3dubG9hZGVkIjowLCJtX21vZFBhY2tJbkVycm9yIjp7Im1faW5kZXhJbkVycm9yIjotMSwibV9tb2RQYWNrSW5FcnJvciI6IkFBQUFBQUFBQUFBQUFBQUFBQUFBQUE9PSJ9LCJtX2FpUGVyc29uYWxpdHkiOiIiLCJtX2FpTG9hZG91dCI6NDI5NDk2NzI5NSwibV9jb3NtZXRpY09wdGlvbnMiOnsibV9wYWludFNjaGVtZUlEIjp7Im1faWQiOjQyOTQ5NjcyOTUsIm1fdHlwZSI6MH0sIm1fcGFpbnRQcmltYXJ5IjoiLy8vLy93PT0iLCJtX3BhaW50U2Vjb25kYXJ5IjoiLy8vLy93PT0iLCJtX3BhaW50VHJpbSI6Ii8vLy8vdz09IiwibV9wYWludFRlcnRpYXJ5IjoiLy8vLy93PT0iLCJtX2JhZGdlUHJpbWFyeSI6Ii8vLy8vdz09In0sIm1fdGVhbUFsbGlhbmNlIjoiRVNjQUFBPT0iLCJtX2FybXlBYmlsaXRpZXMiOltdLCJtX2FybXlVcGdyYWRlcyI6W10sIm1fYXJteVVuaXRzIjpbXSwibV9kb05vdFJhbmRvbWl6ZSI6MH0A"
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":1,
      "factionID":0,
      "raceID":106553,
      "rankLevel":1,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":2,
      "metaData":"eyJtX2luR2FtZSI6MCwibV9pbnZlbnRvcnlSZWFkeSI6MCwibV9wbGF5ZXJSZWFkeSI6MCwibV9yYW5kb21TdGFydFBvc2l0aW9uIjoxLCJtX3N0YXJ0aW5nUG9zaXRpb24iOi0xLCJtX21vZFBhY2tPcHRpb25zIjp7Im1vZFBhY2tzIjp7fSwibW9kRGVwcyI6W119LCJtX21vZFBhY2tGbGFncyI6MCwibV9tb2RQYWNrRG93bmxvYWRQcm9ncmVzcyI6MC4wMDAwMDAsIm1fbmVlZGVkTW9kc0NvdW50IjowLCJtX25lZWRlZE1vZHNEb3dubG9hZGVkIjowLCJtX21vZFBhY2tJbkVycm9yIjp7Im1faW5kZXhJbkVycm9yIjotMSwibV9tb2RQYWNrSW5FcnJvciI6IkFBQUFBQUFBQUFBQUFBQUFBQUFBQUE9PSJ9LCJtX2FpUGVyc29uYWxpdHkiOiIiLCJtX2FpTG9hZG91dCI6NDI5NDk2NzI5NSwibV9jb3NtZXRpY09wdGlvbnMiOnsibV9wYWludFNjaGVtZUlEIjp7Im1faWQiOjQyOTQ5NjcyOTUsIm1fdHlwZSI6MH0sIm1fcGFpbnRQcmltYXJ5IjoiLy8vLy93PT0iLCJtX3BhaW50U2Vjb25kYXJ5IjoiLy8vLy93PT0iLCJtX3BhaW50VHJpbSI6Ii8vLy8vdz09IiwibV9wYWludFRlcnRpYXJ5IjoiLy8vLy93PT0iLCJtX2JhZGdlUHJpbWFyeSI6Ii8vLy8vdz09In0sIm1fdGVhbUFsbGlhbmNlIjoiRVNjQUFBPT0iLCJtX2FybXlBYmlsaXRpZXMiOltdLCJtX2FybXlVcGdyYWRlcyI6W10sIm1fYXJteVVuaXRzIjpbXSwibV9kb05vdFJhbmRvbWl6ZSI6MH0A"
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":2,
      "factionID":0,
      "raceID":131384,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":3,
      "factionID":0,
      "raceID":129267,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":4,
      "factionID":0,
      "raceID":0,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":5,
      "factionID":0,
      "raceID":0,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":6,
      "factionID":0,
      "raceID":0,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":7,
      "factionID":0,
      "raceID":0,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":8,
      "factionID":0,
      "raceID":0,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":9,
      "factionID":0,
      "raceID":0,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":10,
      "factionID":0,
      "raceID":0,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":11,
      "factionID":0,
      "raceID":0,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":12,
      "factionID":0,
      "raceID":0,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":13,
      "factionID":0,
      "raceID":0,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":14,
      "factionID":0,
      "raceID":0,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   },
   {
      "profileInfo.id":-1,
      "stationID":-1,
      "teamID":15,
      "factionID":0,
      "raceID":0,
      "rankLevel":0,
      "rankMatchTypeID":-1,
      "timePerFrameMS":0,
      "isReady":0,
      "status":1,
      "metaData":""
   }
]
```

### Response (Player MetaData)

```
{
   "m_inGame":0,
   "m_inventoryReady":0,
   "m_playerReady":0,
   "m_randomStartPosition":1,
   "m_startingPosition":-1,
   "m_modPackOptions":{
      "modPacks":{
         
      },
      "modDeps":[
         
      ]
   },
   "m_modPackFlags":0,
   "m_modPackDownloadProgress":0.000000,
   "m_neededModsCount":0,
   "m_neededModsDownloaded":0,
   "m_modPackInError":{
      "m_indexInError":-1,
      "m_modPackInError":"AAAAAAAAAAAAAAAAAAAAAA=="
   },
   "m_aiPersonality":"",
   "m_aiLoadout":4294967295,
   "m_cosmeticOptions":{
      "m_paintSchemeID":{
         "m_id":4294967295,
         "m_type":0
      },
      "m_paintPrimary":"/////w==",
      "m_paintSecondary":"/////w==",
      "m_paintTrim":"/////w==",
      "m_paintTertiary":"/////w==",
      "m_badgePrimary":"/////w=="
   },
   "m_teamAlliance":"EScAAA==",
   "m_armyAbilities":[
      
   ],
   "m_armyUpgrades":[
      
   ],
   "m_armyUnits":[
      
   ],
   "m_doNotRandomize":0
}
```
