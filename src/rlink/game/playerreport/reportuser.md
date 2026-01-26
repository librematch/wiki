# [POST] /game/playerreport/reportuser

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/playerreport/reportUser HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 278

callNum=79&comment=misclick&connect_id=mfukppp90s845hti7ktv7wc7e50hkv&lastCallTime=2262938&metadata={"location":4,"clanTag":"KAOS","clanName":"KAOS"}&reportReason=7&reportType=&reportee_profile_id=209072&sessionID=mfukppp90s845hti7ktv7wc7e50hkv
```

| parameter           | type | value                                               | comments      |
| ------------------- | ---- | --------------------------------------------------- | ------------- |
| callNum             | int  | 40                                                  |               |
| comment             | str  | "misclick"                                          |               |
| connect_id          | str  |                                                     | =sessionID    |
| lastCallTime        | int  |                                                     |               |
| metadata            | json | "{"location":4,"clanTag":"KAOS","clanName":"KAOS"}" |               |
| reportReason        | int  | 7                                                   | 7=all reasons |
| reportType          | ?    |                                                     |               |
| reportee_profile_id | int  |                                                     |               |
| sessionID           | str  |                                                     | =connect_id   |

### Response

```
[
    0, // result status code; success
    830398 // probably string value in binary to write to window (e.g. "We take reports very seriously")
]
```
