# [POST] /game/clan/disband

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/clan/disband HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 114

callNum=69&connect_id=mfukppp90s845hti7ktv7wc7e50hkv&lastCallTime=1852544&sessionID=mfukppp90s845hti7ktv7wc7e50hkv
```

| parameter    | type | value | comments    |
| ------------ | ---- | ----- | ----------- |
| callNum      | int  | 40    |             |
| connect_id   | str  |       | =sessionID  |
| lastCallTime | int  |       |             |
| sessionID    | str  |       | =connect_id |

### Response

```
[
    0 // result status code
]
```
