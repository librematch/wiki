# [POST] /game/advertisement/updateTags

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/advertisement/updateTags HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 476

advertisementid=186430525&callNum=51&connect_id=6mikb1saqrmud2kte7ovswogamd2th&lastCallTime=263636&numericTagNames=["CheatsEnabled","Dataset","TreatyLength","Ranked","Password"]&numericTagValues=[0,1,0,0,0]&sessionID=6mikb1saqrmud2kte7ovswogamd2th&stringTagNames=["GameType","MapStyleType","Speed","VictoryType","Server"]&stringTagValues=["0","0","2","9","westeurope"]
```

| parameter        | type          | value                                                          | comments |
| ---------------- | ------------- | -------------------------------------------------------------- | -------- |
| advertisementid  | int           | -1                                                             |          |
| callNum          | int           | 123                                                            |          |
| connect_id       |               |                                                                |          |
| lastCallTime     | timestamp     | 111                                                            |          |
| numericTagNames  | arr[enum/str] | ["CheatsEnabled","Dataset","TreatyLength","Ranked","Password"] |          |
| numericTagValues | arr[int]      | [0,1,0,0,0]                                                    |          |
| sessionID        | str           |                                                                |          |
| stringTagNames   | arr[enum/str] | ["GameType","MapStyleType","Speed","VictoryType","Server"]     |          |
| stringTagValues  | arr[str]      | ["0","0","2","9","westeurope"]                                 |          |

### Response

```
[
    0
]
```
