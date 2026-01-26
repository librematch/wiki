# [POST] /game/account/setAvatarMetadata (Missing Response)

**AUTHENTICATION**

Response

## AoE2:DE

### Request

```
POST /game/account/setAvatarMetadata HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 151
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

callNum=123&connect_id=ccc&lastCallTime=111&metaData={"sharedHistory":0}&sessionID=zzz
```

| parameter    | type      | value               | comments |
| ------------ | --------- | ------------------- | -------- |
| callNum      | int       | 123                 |          |
| connect_id   |           |                     |          |
| lastCallTime | timestamp |                     |          |
| sessionID    | str       |                     |          |
| metaData     | Dict      | {"sharedHistory":0} |          |

### Response

```
RESPONSE_TEMPLATE
```
