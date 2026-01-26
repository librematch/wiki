# [POST] /game/party/finalizeReplayUpload

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/party/finalizeReplayUpload HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=9d14d30f6b4043bb709afd579149ef4d;ApplicationGatewayAffinityCORS=9d14d30f6b4043bb709afd579149ef4d;worldsedgelink=1976371361;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 404

callNum=148&connect_id=ebyb0gp9rsvu863i501263m9wjly55&errorString=&finalizeResult=1&isSinglePlayer=0&lastCallTime=2613735&match_id=186444398&sessionID=ebyb0gp9rsvu863i501263m9wjly55&size=340242&url=https://rl0aoelivemk2blob.blob.core.windows.net/cloudfiles/436432/aoelive_/age2/replay/windows/4.0.0/0/M_186444398_8b31ed6602350cce7ee1736393cab532712c579e545fdd41995117491b1ae319.gz
```

| parameter      | type      | value                                                                                                                                                                                  | comments      |
| -------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- |
| callNum        | int       | 123                                                                                                                                                                                    |               |
| connect_id     | str       | ccc                                                                                                                                                                                    |               |
| errorString    | str       |                                                                                                                                                                                        |               |
| finalizeResult | int       | 1                                                                                                                                                                                      |               |
| isSinglePlayer | int       | 0                                                                                                                                                                                      |               |
| lastCallTime   | timestamp | 111                                                                                                                                                                                    |               |
| match_id       | int       | 555                                                                                                                                                                                    |               |
| sessionID      | str       | zzz                                                                                                                                                                                    |               |
| size           | int       | 3124                                                                                                                                                                                   | size in bytes |
| url            | str       | https://rl0aoelivemk2blob.blob.core.windows.net/cloudfiles/436432/aoelive_/age2/replay/windows/4.0.0/0/M_186444398_8b31ed6602350cce7ee1736393cab532712c579e545fdd41995117491b1ae319.gz |               |

### Response

```
[
   0 // result status code
]
```

## AoE4

### Request

```
POST /game/party/finalizeReplayUpload HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 404
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=114&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&errorString=&finalizeResult=1&isSinglePlayer=1&lastCallTime=650769&match_id=86651938&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&size=94758&url=https://rl0aoelivemk2blob.blob.core.windows.net/cloudfiles/436432/aoelive_/age4/replay/windows/4.0.0/24916/S_86651938_dc7e849e1c1c345607b4f1ee23788d246e9ce15955787ac520a40ea0c9ec0d77.gz
```

| parameter      | type      | value                                                                                                                                                                                     | comments      |
| -------------- | --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- |
| callNum        | int       | 123                                                                                                                                                                                       |               |
| connect_id     | str       | ccc                                                                                                                                                                                       |               |
| errorString    | str       |                                                                                                                                                                                           |               |
| finalizeResult | int       | 1                                                                                                                                                                                         |               |
| isSinglePlayer | int       | 1                                                                                                                                                                                         |               |
| lastCallTime   | timestamp | 111                                                                                                                                                                                       |               |
| match_id       | int       | 555                                                                                                                                                                                       |               |
| sessionID      | str       | zzz                                                                                                                                                                                       |               |
| size           | int       | 3124                                                                                                                                                                                      | size in bytes |
| url            | str       | https://rl0aoelivemk2blob.blob.core.windows.net/cloudfiles/436432/aoelive_/age4/replay/windows/4.0.0/24916/S_86651938_dc7e849e1c1c345607b4f1ee23788d246e9ce15955787ac520a40ea0c9ec0d77.gz |               |

### Response

```
[
   0 // result status code
]
```
