# [GET] /game/relationship/getPresenceData

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/relationship/getPresenceData?callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz HTTP/1.1
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
    "UThEX8G6hJPubrzFQHPQPua1vkrbAQ74iq+hi5BC7qQXQtCvlJfgtgcK2vITDBl/ysBOnxv04QPBKGk1O9XKcNdl/FsURU7lOUfvitX8I4iIBSvOjvclZvy6IKVv8DlStV+5pB93lCY5jQ54OA85nLW9LUg1GmzgPMVMysmRBw907L6fiH4bkE1Hk6qMjGiAAJ/odkPpukUx4Uou50noykEIiellHjZQXs5nc4mCmAzw/0QP5zJgCcG5A6bsmfQo8swLBKEdKsxHBUANQ8QpwWyWrBhBZlc/Dl/fGbPPiLbcVN1OzQdGwU0b9//a1jE2Qyq/dPkUOofWu6w80RepuQ=="
]
```

## AoE4

### Request

```
GET /game/relationship/getPresenceData?callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz HTTP/1.1
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
    0,
    [
        [
            0,
            "offline",
            "Offline",
            "0"
        ],
        [
            1,
            "online",
            "Online",
            "1"
        ],
        [
            2,
            "lobby_online",
            "Online",
            "2"
        ],
        [
            3,
            "appear_offline",
            "Offline",
            "3"
        ],
        [
            1409813,
            "campaign",
            "Campaign",
            "1409813"
        ],
        [
            1409814,
            "custom_game_browser",
            "Browsing Custom",
            "1409814"
        ],
        [
            1409815,
            "in_game",
            "In Game",
            "1409815"
        ],
        [
            1409816,
            "in_group",
            "In Group",
            "1409816"
        ],
        [
            1409817,
            "in_lobby",
            "In Lobby",
            "1409817"
        ],
        [
            1409818,
            "observer_game_browser",
            "Browsing Observer",
            "1409818"
        ],
        [
            1409821,
            "quick_play_searching",
            "Quick Play Searching",
            "1409821"
        ]
    ],
    "t/BN8WlzWUepFrTvDm2s4PVNEqMSF+HIjytIFa5WBCLwFaUAhpE0UD9qOwHb9/53/VDj+ZgrldButKoKxlFkENeNeszYq69VIseZn69/CheovvpN0Z9pTioDVSQLjvDiJ3Ho1eiiiO2h/VqHV7P3HFEZ2LUKx7qFyHnwPqUrjIXvPNs7iMrChLTl/6srNp4tsAuipHBj6Qetow/ZgisJvIBQKEyoubxOHVLEs8xPojGr2r4+gJyCFYR2+R3R+LxXgS+sj5+6cxGy5H9YJc3zG7wWMymDlOhjzzC+siBKsaFfuLGaJW2mJ47IDC+8JKO6rTzuvXtzKwd2nVBEk838CQ=="
]
```
