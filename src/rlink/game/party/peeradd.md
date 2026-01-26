# [POST] /game/party/peerAdd

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/party/peerAdd HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 220
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

callNum=123&connect_id=ccc&lastCallTime=111&match_id=555&profile_ids=[1,1]&race_ids=[1,2,3]&sessionID=zzz&statGroup_ids=[4,5,6]&teamIDs=[0]
```

| parameter     | type       | value               | comments |
| ------------- | ---------- | ------------------- | -------- |
| callNum       | int        | 123                 |          |
| connect_id    |            |                     |          |
| lastCallTime  | timestamp  |                     |          |
| match_id      | int        | 555                 |          |
| profile_ids   | array[int] | [44129481,28941984] |          |
| race_ids      | array[int] | [2,3]               |          |
| sessionID     | str        | zzz                 |          |
| statGroup_ids | array[int] | [1321,12314]        |          |
| teamIDs       | array[int] | [0,1]               |          |

### Response

```
[
   0 // result status code
]
```

## AoE4

### Request

```
POST /game/party/peerAdd HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 225
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=272&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=3025005&match_id=50865084&profile_ids=[233334]&race_ids=[2039321]&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&statGroup_ids=[4275156]&teamIDs=[0]
```

| parameter     | type       | value               | comments |
| ------------- | ---------- | ------------------- | -------- |
| callNum       | int        | 123                 |          |
| connect_id    |            |                     |          |
| lastCallTime  | timestamp  |                     |          |
| match_id      | int        | 555                 |          |
| profile_ids   | array[int] | [44129481,28941984] |          |
| race_ids      | array[int] | [2,3]               |          |
| sessionID     | str        | zzz                 |          |
| statGroup_ids | array[int] | [1321,12314]        |          |
| teamIDs       | array[int] | [0,1]               |          |

### Response

```
[
   0 // result status code
]
```
