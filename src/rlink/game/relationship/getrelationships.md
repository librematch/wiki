# [GET] /game/relationship/getRelationships

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/relationship/getRelationships?callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz HTTP/1.1
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
]
```

## AoE4

### Request

```
GET /game/relationship/getRelationships?callNum=226&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=2939341&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
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
    0, // result status code
    [],
    [],
    [],
    [],
    [],
    [],
    []
]
```
