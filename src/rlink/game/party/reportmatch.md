# [POST] /game/party/reportMatch

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/party/reportMatch HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 1265
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
Expect: 100-continue

callNum=123&checkSums=[0,0]&connect_id=ccc&countersZip=zip&itemUpdates=upd&lastCallTime=111&match_id=555&profile_ids=[1,1]&race_ids=[1,2,3]&results=[0,1]&sessionID=zzz&simplayerIDs=[1,7]&teamIDs=[0,1]&xpGained=[2,20]
```

| parameter    | type       | value   | comments |
| ------------ | ---------- | ------- | -------- |
| callNum      | int        | 123     |          |
| checkSums    | array[int] | [0,0]   |          |
| connect_id   | str        | ccc     |          |
| countersZip  | ?          | zip     |          |
| itemUpdates  | ?          | upd     |          |
| lastCallTime | timestamp  | 111     |          |
| match_id     | int        | 555     |          |
| profile_ids  | array[int] | [1,1]   |          |
| race_ids     | array[int] | [1,2,3] |          |
| results      | array[int] | [0,1]   |          |
| sessionID    | str        | zzz     |          |
| simplayerIDs | array[int] | [1,7]   |          |
| teamIDs      | array[int] | [0,1]   |          |
| xpGained     | array[int] | [2,20]  |          |

### Response

```
[
    0, // result status code
    [],
    [
        186444398,
        "https://rl0aoelivemk2blob.blob.core.windows.net/cloudfiles/436432/aoelive_/age2/replay/windows/4.0.0/0/M_186444398_8b31ed6602350cce7ee1736393cab532712c579e545fdd41995117491b1ae319.gz",
        "rl0aoelivemk2blob.blob.core.windows.net",
        "/cloudfiles/436432/aoelive_/age2/replay/windows/4.0.0/0/M_186444398_8b31ed6602350cce7ee1736393cab532712c579e545fdd41995117491b1ae319.gz",
        0,
        "sig=WND8xzRAWkcTItdgU06jbannF1BSfIH%2BaXnF1kx65CA%3D&se=2022-10-22T01%3A06%3A51Z&sv=2019-02-02&sp=cw&sr=b"
    ],
    [
        -1,
        "",
        "",
        "",
        0,
        ""
    ],
    null,
    [],
    [],
    [],
    [],
    [],
    [],
    0,
    null,
    [],
    [],
    []
]
```
