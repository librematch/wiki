# [POST] /game/advertisement/host

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/advertisement/host HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 941
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

advertisementid=-1&appbinarychecksum=4141&automatchPoll_id=-1&callNum=123&connect_id=ccc&datachecksum=-777&description=SESSION_MATCH_KEY&hostid=1&isObservable=1&lastCallTime=111&mapname=no_map&matchtype=19&maxplayers=8&moddllchecksum=0&moddllfile=INVALID&modname=INVALID&modversion=INVALID&observerDelay=180&observerPassword=&options=opts&party=-1&password=&passworded=0&race=123&relayRegion=eastus&serviceType=0&sessionID=zzz&slotinfo=slot&state=-1&statgroup=-1&team=-1&versionFlags=0&visible=0
```

| parameter         | type      | value              | comments        |
| ----------------- | --------- | ------------------ | --------------- |
| advertisementid   | int       | -1                 |                 |
| appBinaryChecksum | int       | 4141               |                 |
| automatchPoll_id  | int       | -1                 |                 |
| callNum           | int       | 123                |                 |
| connect_id        |           |                    |                 |
| dataChecksum      | int       | 0                  |                 |
| description       | str       | <Lobby_Title>      |                 |
| hostid            | int       | 1                  |                 |
| isObservable      | int       | 1                  |                 |
| lastCallTime      | timestamp | 111                |                 |
| mapname           | str       | no_map             |                 |
| matchtype         | int       | 19                 |                 |
| maxplayers        | int       | 8                  |                 |
| moddllchecksum    | str       | 0                  |                 |
| moddllfile        |           |                    | INVALID         |
| modname           |           |                    | INVALID         |
| modversion        |           |                    | INVALID         |
| observerDelay     | int       | 180                |                 |
| observerPassword  | str       | "unknown password" |                 |
| options           | ?         | opts               |                 |
| party             | int       | -1                 |                 |
| password          | ?         | None               |                 |
| passworded        | int/bool  | 0                  |                 |
| race              | int       | -1                 |                 |
| relayRegion       | str       | eastus             |                 |
| serviceType       | int       | 0                  |                 |
| sessionID         | str       |                    |                 |
| slotinfo          | ?         | slot               | zlib-compressed |
| state             | int       | -1                 |                 |
| statgroup         | int       | -1                 |                 |
| team              | int       | -1                 |                 |
| versionFlags      | int       | 0                  |                 |
| visible           | int       | 0                  |                 |

### Response

```
[
    0,
    186443884,
    "authtoken",
    "51.138.79.234",
    27017,
    27117,
    27217,
    "westeurope", // server location
    [
        [
            186443884,
            233334, // self profile_id
            -1,
            33833,
            0,
            -1,
            "/10.0.11.6"
        ]
    ],
    0,
    "0",
    "SESSION_MATCH_KEY"
]
```

## AoE4

### Request

```
POST /game/advertisement/host HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 1025
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Expect: 100-continue

advertisementid=-1&appbinarychecksum=24916&automatchPoll_id=-1&callNum=271&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&datachecksum=-638535971&description=SESSION_MATCH_KEY&hostid=233334&isObservable=1&lastCallTime=3024155&mapname=no_map&matchtype=19&maxplayers=8&moddllchecksum=0&moddllfile=INVALID&modname=INVALID&modversion=INVALID&observerDelay=180&observerPassword=&options=eNp1jtEKgjAUhnuWXS9wkpZeVhRRQqB0ExJDD7Vym7hZiPjubSuoi7o85/++/5we8RNtteRUF5eE1gfQEhSKjzk2iYIKCs2kQHFvRgdlXQ2rip4N5FnmwcRCipJZzImD3V4lE1AmVkhBKZNtligeE/x9L9W00Rnj8K5qqLhBSe7EfVHuaCdbvZ+vt9DZZhL50SzCxJ9OIg/7XhiQMMg/YgaUq9+qo1rx4v4gw+gJPtNd0w==&party=-1&password=&passworded=0&race=2039321&relayRegion=ukwest&serviceType=0&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&slotinfo=eNrtjkEKwjAQRT3LrKNYl10XoWBBqjtxMaQTHGySkoxCEe8uiaDewE127zMP5lUbdXrAFLzhkVpn/IoHqJeVgigo7F3bvKcQ2sRrBQb17yWgpi+7647uNGYxrQ5FX47z9FGELe0pbANa6g7Z49gTDnPm9PYWM1oSbFAQaoCnKpWlslSWyr9XnhcvuymdYw==&state=-1&statgroup=-1&team=-1&versionFlags=0&visible=0
```

| parameter         | type      | value   | comments        |
| ----------------- | --------- | ------- | --------------- |
| advertisementid   | int       | -1      |                 |
| appBinaryChecksum | int       | 4141    |                 |
| automatchPoll_id  | int       | -1      |                 |
| callNum           | int       | 123     |                 |
| connect_id        |           |         |                 |
| dataChecksum      | int       | 0       |                 |
| description       | str       |         | <Lobby_Title>   |
| hostid            | int       | 1       |                 |
| isObservable      | int       | 1       |                 |
| lastCallTime      | timestamp | 111     |                 |
| mapname           | str       | no_map  |                 |
| matchtype         | int       | 19      |                 |
| maxplayers        | int       | 8       |                 |
| moddllchecksum    | str       | 0       |                 |
| moddllfile        |           |         | INVALID         |
| modname           |           |         | INVALID         |
| modversion        |           |         | INVALID         |
| observerDelay     | int       | 180     |                 |
| observerPassword  | str       | ""      |                 |
| options           | str       | opts    |                 |
| party             | int       | -1      |                 |
| password          | ?         | None    |                 |
| passworded        | int/bool  | 0       |                 |
| race              | int       | 2039321 |                 |
| relayRegion       | str       | eastus  |                 |
| serviceType       | int       | 0       |                 |
| sessionID         | str       |         |                 |
| slotinfo          | str       | slot    | zlib-compressed |
| state             | int       | -1      |                 |
| statgroup         | int       | -1      |                 |
| team              | int       | -1      |                 |
| versionFlags      | int       | 0       |                 |
| visible           | int       | 0       |                 |

### Response

```
[
    0,
    50865084,
    "authtoken",
    "52.142.146.207",
    27015,
    27115,
    27215,
    "ukwest",
    [
        [
            50865084,
            233334,
            -1,
            4275156,
            2039321,
            -1,
            "/10.0.11.6"
        ]
    ],
    0,
    "0",
    "SESSION_MATCH_KEY"
]
```
