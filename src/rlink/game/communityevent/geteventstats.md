# [GET] /game/CommunityEvent/getEventStats

**AUTHENTICATION**

## AoE4

### Request

```
GET /game/CommunityEvent/getEventStats?callNum=310&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&event_id=31&group_type=1&lastCallTime=3084269&member_id=11190194&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type      | value    | comments |
| ------------ | --------- | -------- | -------- |
| callNum      | int       | 123      |          |
| connect_id   |           |          |          |
| event_id     | int       | 31       |          |
| group_type   | int       | 1        |          |
| lastCallTime | timestamp |          |          |
| member_id    | int       | 11190194 |          |
| sessionID    | str       |          |          |

### Response

```
[
    0, // result status code
    [
        "4097972"
    ],
    [
        [
            19321,
            11190194,
            "/steam/76561198827722196",
            "{\"sharedHistory\":0}",
            "Pikaboo",
            "",
            4097972,
            235234,
            126,
            2,
            null,
            "76561198827722196",
            3,
            []
        ]
    ],
    [],
    []
]
```
