# [POST] /game/item/updateItemAttributes

**AUTHENTICATION**

## AoE4

### Request

```
POST /game/item/updateItemAttributes HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=8fcf0d772d3c17881a57cd3841278a97;ApplicationGatewayAffinityCORS=8fcf0d772d3c17881a57cd3841278a97;worldsedgelink=1976371368;
Cache-Control: no-store
Content-Length: 236
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

attributeKeys=[["is_new"]]&attributeValues=[["0"]]&callNum=49&connect_id=59izpfd14rbl5go285a3v22lhu33hg&itemInstance_ids=[449911889]&lastCallTime=44733&sessionID=59izpfd14rbl5go285a3v22lhu33hg&xpGains=[0]
```

| parameter        | type          | value                          | comments      |
| ---------------- | ------------- | ------------------------------ | ------------- |
| attributeKeys    | arr[arr[str]] | \[\["is_new"\]\]               |               |
| attributeValues  | arr[arr[str]] | \[\["0"\]\]                    |               |
| callNum          | int           | 49                             |               |
| connect_id       | str           | 59izpfd14rbl5go285a3v22lhu33hg |               |
| itemInstance_ids | arr[int]      | [449911889]                    |               |
| lastCallTime     | int           | 44733                          |               |
| sessionID        | str           | 59izpfd14rbl5go285a3v22lhu33hg | is connect_id |
| xpGains          | arr[int]      | [0]                            |               |

### Response

```
[
    0,
    [
        [
            0,
            [
                0
            ]
        ]
    ],
    [
        [
            449911889,
            4,
            454344,
            233334, // self profile_id
            1,
            0,
            "{\"att\":{\"is_new\":{\"val\":\"0\"}}}",
            1666823722,
            0,
            -1,
            35,
            -1
        ]
    ]
]
```
