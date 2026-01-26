# [GET] /game/advertisement/getAdvertisements

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/advertisement/getAdvertisements?callNum=123&connect_id=ccc&lastCallTime=111&match_ids=[5]&sessionID=zzz HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type       | value     | comments |
| ------------ | ---------- | --------- | -------- |
| callNum      | int        | 123       |          |
| connect_id   |            |           |          |
| lastCallTime | timestamp  |           |          |
| match_ids    | array[int] | [132,123] |          |
| sessionID    | str        |           |          |

### Response

```
[
    0,
    [
        [
            186625757,
            109775243615147302,
            "0",
            2239585,
            0,
            "mitchell.flowers's Game",
            "mitchell.flowers's Game",
            1,
            "my map",
            "eNpFkttuwyAMht+lT9CkCdIuk0KnTAOUilTKLptOkYi6VNoqCk8/g03L1S8b258Pm+PcN/BKaVffOFC8YbIhW7jd2yj5ErSVDv2CnTGm0vxWo61jsqcYs7o2Kj46bRsRpTYNxMgoC7Cdo1BGsmP5cbuY9uu0E17uf53ko5ehrSY+l5ewfcPcI/AMKRYYd5J4lQG2VGcuIecB64zs0wisySf2jUw7bacCc82Zs1Bh9cRZ6p8lxSgbYxJnre2YbNLEeYxRPqC3hzK5pz5zVcqsf7InzaNGRs3XB9WAfAPWCA1TxBXz4Xwnr61wqAXMeqAZii3YD8gxMIh9Rw0zMV1Bf6A/Qawz07i7h4bc++SfQswteUM5u+depBWMuD3MtqS9ww5gNomlg/qja+eUJ7J4Rf+hZ5//K5v76IBlpLl2FdwM9TwAV5qhBy6fZyjDlG9tp2ze5+L1tSI/7MuRP2T/UGZ+9bq7Wj7vYapyvApLvoECdkH9zw78eC9wy6976ZjGvxX0T7sYan093Tf/3iHxvw==",
            0,
            8,
            "eNrt0k9PgzAUAHA/S8/MUBjTLfHCRhUj+1NocTMeKnQZKzBkOLcYv7srZptL9CAe3IFTX997eS/55UFNeXgDWb6YRjG30+niPApBR9P0tnFpKGBZsCJapHYPdKACCs4SGaoKmLJgV9j+chbwfZiKO77i8f7nsCKYeZus7GjIMVHChzxHOUu445Z90RJzFm7KLXLny7JMJ7xgPVYw0AG2uDUxQeaIoObID+VrkfvMJGUOm65a1gbYEtATOHeE0XI9OiACynyXIrGhKZ34VvY6nqNuAOPx0/V6zrQ19EXo961+uu0zMUKGBzHuE+N5rMdDiiiS+RGd3NBkFhFC5TyTu/YVeFe+s2uqels/stMOdvBE7LBH/83OiX6wa8AjtsaXm9OO3GRlB/cZ/0lOPchpp3113d/L6bVcRblmLVdRzqjlKsq1armKche13F7u8ewDHxYYPA==",
            0,
            [
                [
                    186625757,
                    2239585,
                    -1,
                    1990152,
                    -1,
                    -1,
                    "/10.0.11.14"
                ],
                [
                    186625757,
                    2240393,
                    -1,
                    1990856,
                    -1,
                    1,
                    "/10.0.11.14"
                ]
            ],
            0,
            512,
            0,
            0,
            1,
            0,
            null,
            "eastus",
            null
        ]
    ]
]
```

## AoE4

### Request

```
GET /game/advertisement/getAdvertisements?callNum=301&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=3078219&match_ids=%5B50864995%5D&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type       | value     | comments |
| ------------ | ---------- | --------- | -------- |
| callNum      | int        | 123       |          |
| connect_id   |            |           |          |
| lastCallTime | timestamp  |           |          |
| match_ids    | array[int] | [132,123] |          |
| sessionID    | str        |           |          |

### Response

```
[
    0,
    [
        [
            50864995,
            109775243868517791,
            "0",
            11190194,
            0,
            "3v3 random team",
            "3v3 random team",
            1,
            "generated_map",
            "eNqtUc1OwkAQ9lnmahNbKLRLwqGoQaICAjdDzNpuYcO23bQLWAjP4tW7B+PFt1Ffw/2h5QXcw2a+b2a/2flmDwnms5IT6DgWbGl6S0oZush1EHIkFdFYpwqBc1FUVSOu4kcIHoIALAjM6cLcgjyNoNNse40WclyvYQHLwhV0bAvWVGYadtNtIeRLnQSLcKn7ARzRZbyQJX5b9mOZ0AjihZS+ceXVO1dd/gUH3W7Vc9zrD+TH4EKd7ZHnQ5xIT+D74+339f3n8wv0IJjRHYnu67RicUlyZcZcv+uTdLqTNiHPbzoVc4fLbC3U8I5vuxXbo5ks9DwP1dT05LIhJspNu0KjTa492UPyFGGB1Q8O9duQpPUmMWPZ9vpFjFfFCU8Ir3CSRWaHexWOcbjSI0gxHg/SjRmNx0MiTEiLq+eF2WJBAsYoTkMyIzgxcuGSYKVmH87+AHSdsw8=",
            0,
            16,
            "eNrtmFtvozgUx/ez5Dld2eaSeKR5KKlMiXJpCPfVPBhDFIIhUUNoyWi++xqSbZrORKvVaqbNiCfsc8zxn+Pz07GAqPvX187mcb1IeGzki/WfSdT5BCHEAGK529kWtEjWuXEnjN1OEdOsHoJuZ0HZPw4xe6QsrocIKH0JS7UhT0dxGfOjO0/HtGBLq9o0627qYEkWP8SP5JFm8XjerEu2ZkyjqhnXO++2zTCLC3pHC9r51ImrYeEhvjMRKYK5oY4HT0no4E2YBzzMzZLlfB64JI1PvqdQJ0rgDd/aK99V0hBBK9JJFRGtZIgD6uKdsVo/jwZiH2kCfG8obEpu63hPPXMTIjmZJuDgR7AMiLb0UfHA7mufsjdWm56Rvdjreeh5YCtsi9DFqa2TFQXB1ncj4Vs/vYmztyVzGd07h/fmjc4ldTTO8kkZZmQrNCjivcRIjj77ufRds4y8WTJdzaqpNVMmKyaedrOnj/A+dB3xDZO3GhdMJyJvpuWjJRdrhubAUI/5TcUeYLxKwdTyJfGEh3yYCtNtsY+GD3NtKXID7PvhJnRJVefWSPrlqOqX0R7go8Yn3+W7iEy40LIL9H9bZ1bUBSLHRuMfSQw/zI3tK7120JzJxTiJyEceOJqIA5csT9/EGh61m9x3oRbqzxtRB6u6lozUsXxAtJn1EmvJMqjMXPF9el0b5+dS+xxPy1lG0sAbJ1NeRIfzJFXocSfMOGCVobrwcP6BjqehZM6PdbeJszqXt42PehNhn3A7IyJHuAjvuRW4z9wXOoPBS82ufW8yCHW8oshJHTu6e6khSdv6HucsFXWiY8gSQx1ZBN/efv7c+db9HvEeAgAq+IxwdCIcXiIcSlDqyx8c8HkLeAv47w/4OAe3P4QbgT4CqHcGt3SCG12EG6iK0nbvFu4W7o/dvWUA+3Lv/H4unwCXLt/Pxe0cwZbwlvCW8Hdv39KF9o2RLKlIOqNbOdEtX76b95CqtnC3cLdwf+j2XRP4iu2bV7/WlEtwg5/H9X/VqP4SjfB/aexdgcb+FWjEV6ARgmsQCa9BJLoGkdI1iJSvQaTyLiK//PE3wKGsig==",
            0,
            [
                [
                    50864995,
                    2082027,
                    182,
                    317820,
                    106553,
                    2,
                    "/10.0.11.21"
                ],
                [
                    50864995,
                    4018474,
                    83222,
                    3197784,
                    2039321,
                    3,
                    "/10.0.11.21"
                ],
                [
                    50864995,
                    7200159,
                    14052,
                    557957,
                    131384,
                    1,
                    "/10.0.11.21"
                ],
                [
                    50864995,
                    9243623,
                    69314,
                    2840904,
                    137266,
                    4,
                    "/10.0.11.21"
                ],
                [
                    50864995,
                    11190194,
                    1219,
                    4097972,
                    131384,
                    0,
                    "/10.0.11.21"
                ]
            ],
            0,
            512,
            0,
            300,
            0,
            0,
            null,
            "koreacentral",
            "Korea"
        ]
    ]
]
```
