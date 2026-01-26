# [POST] /game/advertisement/join

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/advertisement/join HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 328
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

advertisementid=1&appbinarychecksum=4141&callNum=123&connect_id=ccc&datachecksum=-777&lastCallTime=111&moddllchecksum=0&moddllfile=INVALID&modname=INVALID&modversion=INVALID&party=66&password=&race=123&sessionID=zzz&statgroup=-1&team=-1&versionFlags=0
```

| parameter         | type      | value | comments |
| ----------------- | --------- | ----- | -------- |
| advertisementid   | int       | -1    |          |
| appBinaryChecksum | int       | 4141  |          |
| callNum           | int       | 123   |          |
| connect_id        |           |       |          |
| dataChecksum      | int       | -777  |          |
| lastCallTime      | timestamp | 111   |          |
| moddllchecksum    | str       | 0     |          |
| moddllfile        |           |       | INVALID  |
| modname           |           |       | INVALID  |
| modversion        |           |       | INVALID  |
| party             | int       | 66    |          |
| password          | ?         | None  |          |
| race              | int       | 123   |          |
| sessionID         | str       |       |          |
| statgroup         | int       | -1    |          |
| team              | int       | -1    |          |
| versionFlags      | int       | 0     |          |

### Response

```
[
    0,
    "/10.0.11.14",
    "20.121.50.111", // probably server lobby is being hosted on?
    27013,
    27113,
    27213,
    [
        [
            186625757, // advertisement_id
            233334, // self profile_id
            -1, // lobby full?
            33833,
            -1, // lobby full?
            -1, // lobby full?
            "/10.0.11.14"
        ]
    ]
]
```

## AoE4

### Request

```
POST /game/advertisement/join HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 333
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

advertisementid=50864995&appbinarychecksum=24916&callNum=302&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&datachecksum=-638535971&lastCallTime=3078735&moddllchecksum=0&moddllfile=INVALID&modname=INVALID&modversion=INVALID&party=50865084&password=&race=2039321&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&statgroup=-1&team=-1&versionFlags=0
```

| parameter         | type      | value    | comments |
| ----------------- | --------- | -------- | -------- |
| advertisementid   | int       | 50864995 |          |
| appBinaryChecksum | int       | 4141     |          |
| callNum           | int       | 123      |          |
| connect_id        |           |          |          |
| dataChecksum      | int       | -777     |          |
| lastCallTime      | timestamp | 111      |          |
| moddllchecksum    | str       | 0        |          |
| moddllfile        |           |          | INVALID  |
| modname           |           |          | INVALID  |
| modversion        |           |          | INVALID  |
| party             | int       | 66       |          |
| password          | ?         | None     |          |
| race              | int       | 123      |          |
| sessionID         | str       |          |          |
| statgroup         | int       | -1       |          |
| team              | int       | -1       |          |
| versionFlags      | int       | 0        |          |

### Response

```
[
    0,
    "/10.0.11.21",
    "20.214.220.152",
    27016,
    27116,
    27216,
    [
        [
            50864995,
            233334,
            -1,
            4275156,
            2039321,
            -1,
            "/10.0.11.21"
        ]
    ]
]
```
