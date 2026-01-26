# [GET] /game/clan/getClan

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/clan/getClan?callNum=58&connect_id=mfukppp90s845hti7ktv7wc7e50hkv&lastCallTime=1593197&names=%5B%22Liiit%22%5D&sessionID=mfukppp90s845hti7ktv7wc7e50hkv HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type     | value     | comments    |
| ------------ | -------- | --------- | ----------- |
| callNum      | int      | 40        |             |
| connect_id   | str      |           | =sessionID  |
| lastCallTime | int      |           |             |
| names        | arr[str] | ["Liiit"] |             |
| sessionID    | str      |           | =connect_id |

### Response

```
[
    0,
    [
        [
            11513, // clan_id
            "Liiit", // tag
            "Lithauen", // name
            "Pscht", // description
            "",
            "2",
            25,
            0,
            1,
            "",
            "",
            540532
        ]
    ]
]
```
