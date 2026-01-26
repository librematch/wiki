# [POST] /game/leaderboard/setAvatarStatValues

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/leaderboard/setAvatarStatValues HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=9d14d30f6b4043bb709afd579149ef4d;ApplicationGatewayAffinityCORS=9d14d30f6b4043bb709afd579149ef4d;worldsedgelink=1976371361;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 177

avatarStat_ids=[156]&callNum=153&connect_id=ebyb0gp9rsvu863i501263m9wjly55&lastCallTime=2640288&sessionID=ebyb0gp9rsvu863i501263m9wjly55&updateTypes=[2]&values=[687]
```

| parameter      | type      | value | comments |
| -------------- | --------- | ----- | -------- |
| avatarStat_ids | arr[int]  | [156] |          |
| callNum        | int       | 123   |          |
| connect_id     |           |       |          |
| lastCallTime   | timestamp |       |          |
| sessionID      | str       |       |          |
| updateTypes    | arr[int]  | [2]   |          |
| values         | arr[int]  | [687] |          |

### Response

```
[
    0, // result status code
    [
        0
    ],
    [
        [
            156,
            233334, // self profile_id
            687,
            "",
            1666388285
        ]
    ]
]
```
