# [GET/POST] /game/cloud/getFileURL

**AUTHENTICATION**

**AoE3:DE POST REQUEST!**

## AoE2:DE

### Request

```
GET /game/cloud/getFileURL?callNum=123&connect_id=ccc&lastCallTime=111&names=["Attrib.sga","EngineData.sga"]&sessionID=zzz HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type            | value                           | comments |
| ------------ | --------------- | ------------------------------- | -------- |
| callNum      | int             | 123                             |          |
| connect_id   |                 |                                 |          |
| lastCallTime | timestamp       |                                 |          |
| names        | array[FileName] | ["Attrib.sga","EngineData.sga"] |          |
| sessionID    | str             |                                 |          |

### Response

```
[
    0, // result status code
    [
        [
            "_data.txt",
            24,
            741324928,
            "https://rl0aoelivemk2blob.blob.core.windows.net/cloudfiles/game/6b861a867ce5f4e66131c929fe13db8baa40b5bb412255adcc225e6604ff703f"
        ],
        [
            "_resources.txt",
            29,
            1779231939,
            "https://rl0aoelivemk2blob.blob.core.windows.net/cloudfiles/game/d3349d2d70bc16cb5bd54aa07e2171bb9ccc02212f0a1145045e8a8bda2ff164"
        ]
    ]
]
```

## AoE3:DE

### Request

```
POST /game/cloud/getFileURL?callNum=24&connect_id=fflxvvhtmtcx7tmbxff2kauyfdq8n3&lastCallTime=10141&names=%5B%22iconPacks%22%5D&sessionID=fflxvvhtmtcx7tmbxff2kauyfdq8n3 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: deflate, gzip
Cookie: ApplicationGatewayAffinity=29259ca9e836dd7648ed1ca403a17cde;ApplicationGatewayAffinityCORS=29259ca9e836dd7648ed1ca403a17cde;worldsedgelink=-1321719403;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 140

callNum=24&connect_id=fflxvvhtmtcx7tmbxff2kauyfdq8n3&lastCallTime=10141&names=["iconPacks"]&sessionID=fflxvvhtmtcx7tmbxff2kauyfdq8n3
```

| parameter    | type            | value         | comments |
| ------------ | --------------- | ------------- | -------- |
| callNum      | int             | 123           |          |
| connect_id   |                 |               |          |
| lastCallTime | timestamp       |               |          |
| names        | array[FileName] | ["iconPacks"] |          |
| sessionID    | str             |               |          |

### Response

```
[
    2,
    [
        null
    ]
]
```

## AoE4

### Request

```
GET /game/cloud/getFileURL?callNum=15&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=7596&names=%5B%22Attrib.5.0.24916.0.sga%22%2C%22CardinalCampaignData.5.0.24916.0.sga%22%2C%22CardinalCampaignTensorFlow.5.0.24916.0.sga%22%2C%22CardinalData.5.0.24916.0.sga%22%2C%22CardinalTensorFlow.5.0.24916.0.sga%22%2C%22CardinalUI.5.0.24916.0.sga%22%2C%22CardinalUIArt.5.0.24916.0.sga%22%2C%22EngineData.5.0.24916.0.sga%22%2C%22EngineUI.5.0.24916.0.sga%22%2C%22LocaleArabic.5.0.24916.0.sga%22%2C%22LocaleBrazilianPortuguese.5.0.24916.0.sga%22%2C%22LocaleCzech.5.0.24916.0.sga%22%2C%22LocaleDanish.5.0.24916.0.sga%22%2C%22LocaleDutch.5.0.24916.0.sga%22%2C%22LocaleEnglish.5.0.24916.0.sga%22%2C%22LocaleFinnish.5.0.24916.0.sga%22%2C%22LocaleFrench.5.0.24916.0.sga%22%2C%22LocaleGerman.5.0.24916.0.sga%22%2C%22LocaleGreek.5.0.24916.0.sga%22%2C%22LocaleHebrew.5.0.24916.0.sga%22%2C%22LocaleHindi.5.0.24916.0.sga%22%2C%22LocaleHungarian.5.0.24916.0.sga%22%2C%22LocaleItalian.5.0.24916.0.sga%22%2C%22LocaleJapanese.5.0.24916.0.sga%22%2C%22LocaleKorean.5.0.24916.0.sga%22%5D&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type            | value                                                          | comments |
| ------------ | --------------- | -------------------------------------------------------------- | -------- |
| callNum      | int             | 123                                                            |          |
| connect_id   |                 |                                                                |          |
| lastCallTime | timestamp       |                                                                |          |
| names        | array[FileName] | ["Attrib.5.0.24916.0.sga","EngineData.5.0.24916.0.sga", "..."] |          |
| sessionID    | str             |                                                                |          |

### Response

```
[
    2, // result status code
    [
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null,
        null
    ]
]
```
