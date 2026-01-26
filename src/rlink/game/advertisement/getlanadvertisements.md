# [GET] /game/advertisement/getLanAdvertisements

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/advertisement/getLanAdvertisements?appBinaryChecksum=71094&callNum=141&connect_id=6mikb1saqrmud2kte7ovswogamd2th&dataChecksum=0&lanServerGuids=%5B123e88e6-88e1-4aa7-ab3c-a2975fc0b04d%5D&lastCallTime=520895&matchType_id=0&modDLLChecksum=0&modDLLFile=INVALID&modName=INVALID&modVersion=INVALID&sessionID=6mikb1saqrmud2kte7ovswogamd2th&versionFlags=56950784 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

appBinaryChecksum=71094&callNum=141&connect_id=6mikb1saqrmud2kte7ovswogamd2th&dataChecksum=0&lanServerGuids=%5B123e88e6-88e1-4aa7-ab3c-a2975fc0b04d%5D&lastCallTime=520895&matchType_id=0&modDLLChecksum=0&modDLLFile=INVALID&modName=INVALID&modVersion=INVALID&sessionID=6mikb1saqrmud2kte7ovswogamd2th&versionFlags=56950784
```

| parameter         | type      | value                                  | comments |
| ----------------- | --------- | -------------------------------------- | -------- |
| appBinaryChecksum | int       |                                        |          |
| callNum           | int       | 123                                    |          |
| connect_id        | str       |                                        |          |
| dataChecksum      | str       | 0                                      |          |
| lanServerGuids    | arr[GUID] | [123e88e6-88e1-4aa7-ab3c-a2975fc0b04d] |          |
| lastCallTime      | timestamp |                                        |          |
| matchType_id      | int       | 0                                      |          |
| modDLLChecksum    | str       | 0                                      |          |
| modDLLFile        | ?         | INVALID                                |          |
| modName           | ?         | INVALID                                |          |
| modVersion        | ?         | INVALID                                |          |
| sessionID         | str       |                                        |          |
| versionFlags      | int       |                                        |          |

### Response

```
[
    0,
    [],
    []
]
```
