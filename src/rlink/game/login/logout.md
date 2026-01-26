# [POST] /game/login/logout

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/login/logout HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 524
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type      | value                          | comments                         |
| ------------ | --------- | ------------------------------ | -------------------------------- |
| callNum      | int       | 412                            | count of calls to Relic Link API |
| connect_id   | str       | 6cpdi7mdhsxq5rqa1znxsxp3dtvtey | same as sessionID                |
| lastCallTime | timestamp | 111                            |                                  |
| sessionID    | timestamp | 6cpdi7mdhsxq5rqa1znxsxp3dtvtey |                                  |

### Response

```
[
   0 // result status code
]
```

## AoE4

### Request

Most likely the same as other games

### Response

Most likely the same as other games

## AoE4

### Request

```
POST /game/login/logout HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 115
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=365&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=3200633&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19
```

| parameter    | type      | value                          | comments                         |
| ------------ | --------- | ------------------------------ | -------------------------------- |
| callNum      | int       | 412                            | count of calls to Relic Link API |
| connect_id   | str       | 6cpdi7mdhsxq5rqa1znxsxp3dtvtey | same as sessionID                |
| lastCallTime | timestamp | 111                            |                                  |
| sessionID    | timestamp | 6cpdi7mdhsxq5rqa1znxsxp3dtvtey |                                  |

### Response

```
[
   0 // result status code
]
```
