# [GET] /game/cloud/getTempCredentials

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/cloud/getTempCredentials?callNum=27&connect_id=6mikb1saqrmud2kte7ovswogamd2th&key=%2Fcloudfiles%2Fgame%2F6b861a867ce5f4e66131c929fe13db8baa40b5bb412255adcc225e6604ff703f&lastCallTime=13534&sessionID=6mikb1saqrmud2kte7ovswogamd2th HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type      | value   | comments |
| ------------ | --------- | ------- | -------- |
| callNum      | int       | 123     |          |
| connect_id   |           |         |          |
| lastCallTime | timestamp |         |          |
| sessionID    | str       |         |          |
| key          | file      | file.gz |          |

### Response

```
[
    0,
    1666391406,
    "sig=CSRCwzAc9nw5UxvHoTmIJnGFOhldBtiMcSMS0Y9g7vw%3D&se=2022-10-21T22%3A30%3A06Z&sv=2019-02-02&sp=r&sr=b",
    "/cloudfiles/game/6b861a867ce5f4e66131c929fe13db8baa40b5bb412255adcc225e6604ff703f"
]
```
