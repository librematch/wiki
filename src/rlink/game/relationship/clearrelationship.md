# [POST] /game/relationship/clearRelationship

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/relationship/clearRelationship HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Content-Length: 153

callNum=62&connect_id=fnlyrvpogu8eefn5g97slfa6s4quyh&lastCallTime=1312682&relationType=1&sessionID=fnlyrvpogu8eefn5g97slfa6s4quyh&targetProfileID=4994658
```

| parameter       | type | value | comments          |
| --------------- | ---- | ----- | ----------------- |
| callNum         | int  | 40    |                   |
| connect_id      | str  |       | =sessionID        |
| lastCallTime    | int  |       |                   |
| relationType    | int  | 1     | 1=Unban, 2=Unmute |
| sessionID       | str  |       | =connect_id       |
| targetProfileID | int  |       |                   |

### Response

```
[
   0 // result status code
]
```
