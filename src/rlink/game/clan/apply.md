# [POST] /game/clan/apply

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/clan/apply HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 133

callNum=72&clanList_name=TURK&connect_id=mfukppp90s845hti7ktv7wc7e50hkv&lastCallTime=1994252&sessionID=mfukppp90s845hti7ktv7wc7e50hkv
```

| parameter     | type | value | comments    |
| ------------- | ---- | ----- | ----------- |
| callNum       | int  | 40    |             |
| clanList_name | str  | TURK  |             |
| connect_id    | str  |       | =sessionID  |
| lastCallTime  | int  |       |             |
| sessionID     | str  |       | =connect_id |

### Response

```
[
    6 // result status code; 0 = invite sent, 6 = Clan is full
]
```
