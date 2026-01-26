# [POST] /game/relationship/setPresenceProperty

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/relationship/setPresenceProperty HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 144
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

callNum=123&connect_id=ccc&lastCallTime=111&presencePropertyDef_id=-1&sessionID=zzz&value=
```

| parameter              | type      | value | comments |
| ---------------------- | --------- | ----- | -------- |
| callNum                | int       | 123   |          |
| connect_id             |           |       |          |
| lastCallTime           | timestamp |       |          |
| presencePropertyDef_id | int       | 3     |          |
| sessionID              | str       |       |          |
| value                  | int       | ?     |          |

### Response

```
[
   0 // result status code
]
```

## AoE4

### Request

```
POST /game/relationship/setPresenceProperty HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 153
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=56&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=209404&presencePropertyDef_id=1409823&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&value=-2
```

| parameter              | type      | value | comments |
| ---------------------- | --------- | ----- | -------- |
| callNum                | int       | 123   |          |
| connect_id             |           |       |          |
| lastCallTime           | timestamp |       |          |
| presencePropertyDef_id | int       | 3     |          |
| sessionID              | str       |       |          |
| value                  | int       | -2    |          |

### Response

```
[
   0 // result status code
]
```
