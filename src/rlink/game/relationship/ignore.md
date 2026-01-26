# [POST] /game/relationship/ignore

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/relationship/ignore HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 150

blocklevel=2&callNum=82&connect_id=mfukppp90s845hti7ktv7wc7e50hkv&lastCallTime=2264462&sessionID=mfukppp90s845hti7ktv7wc7e50hkv&targetProfileID=209072
```

| parameter       | type | value | comments            |
| --------------- | ---- | ----- | ------------------- |
| blocklevel      | int  | 2     | 1=lobby ban, 2=mute |
| callNum         | int  | 40    |                     |
| connect_id      | str  |       | =sessionID          |
| lastCallTime    | int  |       |                     |
| sessionID       | str  |       | =connect_id         |
| targetProfileID | int  |       |                     |

### Response

```
[
    0, // result status code
    [
        21873,
        209072,
        "/steam/76561198024758674",
        "{\"icon\":\"PR5-012\"}",
        "[TF] Backyback",
        "KAOS",
        2187,
        1105,
        1,
        3,
        null,
        "76561198024758674",
        3,
        []
    ],
    []
]
```
