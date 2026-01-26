# [POST] /game/item/moveItem (Missing Response)

**AUTHENTICATION**

Response

## AoE2:DE

### Request

```
POST /game/item/moveItem HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 220
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

callNum=123&connect_id=ccc&itemIDs=[1,2]&itemLocationIDs=[0,2]&lastCallTime=111&posIDs=[-1,-1]&sessionID=zzz&slotIDs=[-1,-1]
```

| parameter       | type       | value   | comments |
| --------------- | ---------- | ------- | -------- |
| callNum         | int        | 123     |          |
| connect_id      |            |         |          |
| itemIDs         | array[int] | [4,5]   |          |
| itemLocationIDs | array[int] | [12,3]  |          |
| lastCallTime    | timestamp  |         |          |
| posIDs          | array[int] | [-1,-1] |          |
| sessionID       | str        |         |          |
| slotIDs         | array[int] | [1,3]   |          |

### Response

```
RESPONSE_TEMPLATE
```
