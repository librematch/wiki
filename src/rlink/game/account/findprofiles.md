# [GET] /game/account/FindProfiles (Search by name)

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/account/FindProfiles?callNum=123&connect_id=ccc&lastCallTime=111&name=viper&sessionID=zzz HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type      | value    | comments |
| ------------ | --------- | -------- | -------- |
| callNum      | int       | 123      |          |
| connect_id   |           |          |          |
| lastCallTime | timestamp |          |          |
| name         | str       | username |          |
| sessionID    | str       |          |          |

### Response

```
[
    0, // result status code
    [
        [
            110,
            249641, // profile_id
            "/steam/76561198008248822", // platform_ids (/steam/, /xboxlive/)
            "",
            "Viper", // profile_name
            "",
            53114,
            1,
            1,
            0,
            null,
            "76561198008248822", // pure platform_id_number (steam, different that platform_id for xboxlive)
            3,
            []
        ],
        [
            855,
            300113,
            "/steam/76561197974443592",
            "{\"icon\":\"PR1-001\"}",
            "Viper",
            "",
            116533,
            6,
            1,
            3,
            null,
            "76561197974443592",
            3,
            []
        ],
        [
            51,
            348999,
            "/steam/76561198303411559",
            "",
            "viper",
            "",
            175516,
            0,
            1,
            2,
            null,
            "76561198303411559",
            3,
            []
        ],
        [
            773,
            395221,
            "/steam/76561197996564368",
            "{\"icon\":\"PR2-002\"}",
            "Viper",
            "",
            229018,
            21,
            1,
            0,
            null,
            "76561197996564368",
            3,
            []
        ]
    ]
]
```
