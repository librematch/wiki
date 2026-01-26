# [POST] /game/clan/create

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/clan/create HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=794ba560e22a634f229c95c54bb135c8;ApplicationGatewayAffinityCORS=794ba560e22a634f229c95c54bb135c8;worldsedgelink=1976371366;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 429

callNum=40&chat=[]&connect_id=mfukppp90s845hti7ktv7wc7e50hkv&cost=0&demote=[]&description=&disband=[]&editInfo=[]&editPermission=[]&fullName=Rusty&icon=CR-001&invite=[]&itemPrice_id=-1&joinPolicy=1&lastCallTime=631757&locStringID=[]&messageOfTheDay=&metadata=&name=Rusty&paymentitem=-1&permissionName=[]&promote=[]&rank=[]&remove=[]&sessionID=mfukppp90s845hti7ktv7wc7e50hkv&tags=[]
```

| parameter       | type     | value  | comments          |
| --------------- | -------- | ------ | ----------------- |
| callNum         | int      | 40     |                   |
| chat            | arr[str] |        |                   |
| connect_id      | str      |        | =sessionID        |
| cost            | int      | 0      |                   |
| demote          | arr[]    |        |                   |
| description     | str      |        |                   |
| disband         | arr[]    |        |                   |
| editInfo        | arr[]    |        |                   |
| editPermission  | arr[]    |        |                   |
| fullName        | str      |        |                   |
| icon            | str/enum | CR-001 |                   |
| invite          | arr[]    |        |                   |
| itemPrice_id    | int      | -1     |                   |
| joinPolicy      | int      | 1      |                   |
| lastCallTime    | int      |        |                   |
| locStringID     | arr[]    |        | maybe 'location'? |
| messageOfTheDay | str?     |        |                   |
| metadata        | ?        |        |                   |
| name            | str      |        |                   |
| paymentitem     | int      | -1     |                   |
| permissionName  | arr[]    |        |                   |
| promote         | arr[]    |        |                   |
| rank            | arr[]    |        |                   |
| remove          | arr[]    |        |                   |
| sessionID       | str      |        | =connect_id       |
| tags            | arr[]    |        |                   |

### Response

```
[
    3,
    null,
    null,
    []
]
```
