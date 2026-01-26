# [POST] /game/clan/update

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/clan/update HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 221

callNum=49&clanList_id=110061&connect_id=mfukppp90s845hti7ktv7wc7e50hkv&description=TestyRusty2&icon=CR-001
&joinPolicy=1&lastCallTime=1246820&messageOfTheDay=&metadata=&sessionID=mfukppp90s845hti7ktv7wc7e50hkv&tags=[]
```

| parameter       | type     | value  | comments    |
| --------------- | -------- | ------ | ----------- |
| callNum         | int      | 40     |             |
| clanList_id     | int      | 40     |             |
| connect_id      | str      |        | =sessionID  |
| description     | str      |        |             |
| icon            | str/enum | CR-001 |             |
| joinPolicy      | int      | 1      |             |
| lastCallTime    | int      |        |             |
| messageOfTheDay | str?     |        |             |
| metadata        | ?        |        |             |
| sessionID       | str      |        | =connect_id |
| tags            | arr[]    |        |             |

### Response

```
[
    0, // result status code
    [
        110061, // clan_id
        "yyyy", // tag
        "Rusty1312", // name
        "TestyRusty2", // description
        "",
        "CR-001", // icon
        1,
        0,
        1,
        "",
        "",
        6298829
    ]
]
```
