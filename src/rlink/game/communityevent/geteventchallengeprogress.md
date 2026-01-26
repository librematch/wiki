# [GET] /game/CommunityEvent/getEventChallengeProgress

**AUTHENTICATION**

## AoE4

### Request

```
GET /game/CommunityEvent/getEventChallengeProgress?callNum=220&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&event_id=22&lastCallTime=2935574&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| callNum      | int       | 123   |          |
| connect_id   |           |       |          |
| event_id     | int       | 22    |          |
| lastCallTime | timestamp |       |          |
| sessionID    | str       |       |          |

### Response

```
[
    0, // result status code
    [
        [
            16273087,
            1525309,
            0,
            0,
            1669708740,
            null,
            22,
            1666716600
        ],
        [
            16273088,
            1525311,
            0,
            0,
            1669708740,
            null,
            22,
            1666716600
        ],
        [
            16273089,
            1525313,
            0,
            0,
            1669708740,
            null,
            22,
            1666716600
        ],
        [
            16273090,
            1525315,
            0,
            0,
            1669708740,
            null,
            22,
            1666716600
        ],
        [
            16273091,
            1525329,
            0,
            0,
            1669708740,
            null,
            22,
            1666716600
        ],
        [
            16273092,
            1525331,
            0,
            0,
            1669708740,
            null,
            22,
            1666716600
        ]
    ]
]
```
