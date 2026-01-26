# [GET] /game/account/getProfileProperty (TODO Empty Response)

**AUTHENTICATION**

Response

## AoE2:DE

### Request

```
GET /game/account/getProfileProperty?callNum=123&connect_id=ccc&lastCallTime=111&profile_id=99&property_id=appearOffline&sessionID=zzz HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type      | value         | comments |
| ------------ | --------- | ------------- | -------- |
| callNum      | int       | 123           |          |
| connect_id   |           |               |          |
| lastCallTime | timestamp |               |          |
| sessionID    | str       |               |          |
| profile_id   | int       | 99            |          |
| property_id  | str/enum  | appearOffline |          |

### Response

```
RESPONSE_TEMPLATE
```

## AoE3:DE

### Request

```
GET /game/account/getProfileProperty?callNum=5&connect_id=fflxvvhtmtcx7tmbxff2kauyfdq8n3&lastCallTime=141&profile_id=-2&property_id=HaveShownNativeCivDisclaimer&sessionID=fflxvvhtmtcx7tmbxff2kauyfdq8n3 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: deflate, gzip
Cookie: ApplicationGatewayAffinity=29259ca9e836dd7648ed1ca403a17cde;ApplicationGatewayAffinityCORS=29259ca9e836dd7648ed1ca403a17cde;worldsedgelink=-1321719403;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type      | value         | comments |
| ------------ | --------- | ------------- | -------- |
| callNum      | int       | 123           |          |
| connect_id   |           |               |          |
| lastCallTime | timestamp |               |          |
| profile_id   | int       | -2            |          |
| property_id  | str/enum  | appearOffline |          |
| sessionID    | str       |               |          |

### Response

```
HTTP/1.1 400 Bad Request
Date: Wed, 26 Oct 2022 19:03:48 GMT
Content-Type: text/html;charset=iso-8859-1
Content-Length: 636
Connection: keep-alive
Request-Context: appId=cid-v1:26109784-3156-45bd-b9c0-963ca4949d0f
Request-Path: /game/account/getProfileProperty
Cache-Control: must-revalidate,no-cache,no-store
```

## AoE4

### Request

```
GET /game/account/getProfileProperty?callNum=148&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=918824&profile_id=233334&property_id=appearOffline&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type      | value         | comments |
| ------------ | --------- | ------------- | -------- |
| callNum      | int       | 123           |          |
| connect_id   |           |               |          |
| lastCallTime | timestamp |               |          |
| profile_id   | int       | 99            |          |
| property_id  | str/enum  | appearOffline |          |
| sessionID    | str       |               |          |

### Response

```
[
    0
]
```
