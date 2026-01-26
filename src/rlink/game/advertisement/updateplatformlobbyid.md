# [POST] /game/advertisement/updatePlatformLobbyID

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/advertisement/updatePlatformLobbyID HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 163
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

callNum=123&connect_id=ccc&lastCallTime=111&matchID=555&platformlobbyID=1&sessionID=zzz
```

| parameter       | type      | value | comments |
| --------------- | --------- | ----- | -------- |
| callNum         | int       | 123   |          |
| connect_id      |           |       |          |
| lastCallTime    | timestamp | 111   |          |
| matchID         | int       | 555   |          |
| platformlobbyID | int       | 1     |          |
| sessionID       | str       |       |          |

### Response

```
[
    0
]
```

## AoE4

### Request

```
POST /game/advertisement/updatePlatformLobbyID HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 167
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=273&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=3025521&matchID=50865084&platformlobbyID=109775243868575631&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19
```

| parameter       | type      | value | comments |
| --------------- | --------- | ----- | -------- |
| callNum         | int       | 123   |          |
| connect_id      |           |       |          |
| lastCallTime    | timestamp | 111   |          |
| matchID         | int       | 555   |          |
| platformlobbyID | int       | 1     |          |
| sessionID       | str       |       |          |

### Response

```
[
    0
]
```
