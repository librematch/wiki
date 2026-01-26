# [GET] /game/advertisement/findAdvertisements

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/advertisement/findAdvertisements?appBinaryChecksum=8888&callNum=123&connect_id=ccc&dataChecksum=-888&lastCallTime=111&matchType_id=0&modDLLChecksum=0&modDLLFile=INVALID&modName=INVALID&modVersion=INVALID&profile_ids=[1,1]&race_ids=[1,2,3]&sessionID=zzz&statGroup_ids=[4,5,6]&versionFlags=0 HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter         | type       | value     | comments    |
| ----------------- | ---------- | --------- | ----------- |
| appBinaryChecksum | int        | 8888      |             |
| callNum           | int        | 123       |             |
| connect_id        | str        | ccc       |             |
| dataChecksum      | int        | -888      | is negative |
| lastCallTime      | timestamp  | 111       |             |
| matchType_id      | int        | 0         |             |
| modDLLChecksum    | str        | 0         |             |
| modDLLFile        |            |           | INVALID     |
| modName           |            |           | INVALID     |
| modVersion        |            |           | INVALID     |
| profile_ids       | array[int] | [412,567] |             |
| race_ids          | array[int] | [1,2]     |             |
| sessionID         | str        | zzz       |             |
| statGroup_ids     | array[int] | [12,34]   |             |
| versionFlags      | int        | 0         |             |

### Response

```
[
    0,
    [
        [
            144146175, // match_id
            109775240944275349,
            "0",
            8593884,
            0,
            "Come if you dare buahahahahaaaa!", // name
            "Come if you dare buahahahahaaaa!",
            1,
            "my map",
            // zlib compressed settings 
            "eNpFUsFuwyAM/Zd+QZMmSD3skBRaRRqgTKRrdiybIpFt6WFTCl8/g03H6cnG9nvP3rxMfQOvlG7xzQqIN0w2FAu33zZCPgft5Ip5wa5YU2l+qzHWMdlTjVnWNiI+rto1IkJtGqiRERYQu0agjGT68n6y4q278vb1fDkbe9gLI/qdnT/LwWz32HsEPkOqBY47SXyVAW5pzlRCzyPOGdmzETiTW/aBnHba2QJ7TVlbocLiiWepv+dUo1ysSTxr0Jti0kQ/xgjvoO2uTE+a+syrUmb5kT1hHjFy1Hy50wzoN+CM0DBFvGI/9Nd67cSKWIDXA3kothA/Io+BQe0JMXhiuoL+gD5BXCemUd9dQ+9DytsQe0veUM/usRfpBCPeHrwtyRsvozeJSwfzx7WdUp/IxSv6D5p9/q9c1tEBl5F87arsoQoD8EoeeuAFtTQ/2LyPnXK3Gutmr78qysO+JsqHvO+hzHpVvDvM1/JxD7bK9SrM+QYK2AXpn1bI473ALf/fy+OGK9BPfwfYW/e0+QNAfvCc",
            0,
            8,
            // zlib compressed player data
            "eNrVkl1vgjAUhvdbeo0LRVFnshvUOsxALbQoyy6q1IB8yJD5tey/T2p0M5kXi8mMV+e0503Pe55TqEgvHyDN5tMg4noynd8HHmjU1YdyvV6RwCJneTBP9BZoQAnknMVFKktgyiaHwu6UsQk/pkn4zJc8Op4Mlk98e5MKRal4Joh5n2coYzE3LKELFpgzbyO6FD3fF+I65jlrsZyBBtDDroYJ0gYEVQZUxLZDukXUbIKWRRzYmsnixcqG2DVk+Ma2CHlyoXV7LEqHpuPPxs5aocSrsA4d0iSy6ZZmTuQnltChHm6H0A5xZoRq1bJpj+x7NSlNhzjBGhEesNu39EfwKf3Grl6uKfIJO+WbHbw2O8cT7LDdPcyinZ09hPvZUbihCXWddroazVBzAqPRuLOeMWUNndBzzLaZFPwxQuqOPTaJ+jYqR32KKBJ7oe4Tjf2AECr2ZQRn2JXgCbbSjz+nnHArKgdw+/wicvI5cn91Wb4Jl5V/cgkvcqnehMvqTbisXcnl690XTfP9rg==",
            0,
            [
                [
                    144146175,
                    8583720,
                    -1,
                    5445306,
                    -1,
                    1,
                    "/10.0.11.4"
                ],
                [
                    144146175,
                    8593884,
                    -1,
                    5445586,
                    -1,
                    -1,
                    "/10.0.11.4"
                ]
            ],
            0,
            512,
            1,
            0,
            1,
            0,
            null,
            "westeurope", // server
            null
        ],
    /// ...
    ],
    []
]
```

## AoE4

### Request

```
GET /game/advertisement/findAdvertisements?appBinaryChecksum=24916&callNum=293&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&dataChecksum=-638535971&lastCallTime=3052353&matchType_id=0&modDLLChecksum=0&modDLLFile=INVALID&modName=INVALID&modVersion=INVALID&profile_ids=%5B234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%2C234634%5D&race_ids=%5B106553%2C129267%2C131384%2C133008%2C134522%2C136150%2C137266%2C182910%2C186603%2C186624%2C187558%2C187855%2C195982%2C199703%2C205592%2C205674%2C221744%2C2039321%2C2058393%5D&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&statGroup_ids=%5B4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%2C4275156%5D&versionFlags=0 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter         | type       | value     | comments    |
| ----------------- | ---------- | --------- | ----------- |
| appBinaryChecksum | int        | 8888      |             |
| callNum           | int        | 123       |             |
| connect_id        | str        | ccc       |             |
| dataChecksum      | int        | -888      | is negative |
| lastCallTime      | timestamp  | 111       |             |
| matchType_id      | int        | 0         |             |
| modDLLChecksum    | str        | 0         |             |
| modDLLFile        |            |           | INVALID     |
| modName           |            |           | INVALID     |
| modVersion        |            |           | INVALID     |
| profile_ids       | array[int] | [412,567] |             |
| race_ids          | array[int] | [1,2]     |             |
| sessionID         | str        | zzz       |             |
| statGroup_ids     | array[int] | [12,34]   |             |
| versionFlags      | int        | 0         |             |

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
        ],
        [
            50863834,
            0,
            "{\"templateName\":\"GameSession\",\"name\":\"cef65084-3bb6-41d1-b59a-e8e63177206a\",\"scid\":\"00000000-0000-0000-0000-00007d18f66e\"}",
            7041975,
            0,
            " 4 v 4 MAX RS a los putazos",
            " 4 v 4 MAX RS a los putazos",
            1,
            "generated_map",
            "eNqtUttu2kAQ7aegea3b+LJrGyQebEJTkhIIoDZqharFXl/q28o2AYL4986uMf2B7oM1c+ZyZs74DAUTm5PgMDI0OKTlEz+hSYbEGA4NhMI0UqGmZXXb9FkLIe1f4L1MfdDA8+YevjFsNajLEEbUNAzLJjrVIK+CDEa6BvsUA6ZuEUoty9GQuA0SRQdw9SZRjCmujXR51SoPohg7fyX48T9Kkv/ie+Nxz7n0H2Y4GNzJd7ji4pkVKAn4OQuywZeq5k0LaheWp+88nN8yJMpOvJZybFXpAy/X73JT0zSJ1UPf2Knat6ifZViu26N+WiFk21S/Qeur0HoPrKSgN2/xVitdzlD8DlnL5AiXW23Ay9sxWZ5Xh+mxXWbNP3/FRe8XVdid8SzNJS4qdzgDq4PZPbZ9Ea/WZDX/QadFmB2SWfKYHstOIEz5zmvM+eNM1jzzDfEzeX20Yudps7tbxJ2I2HMpm38yia0T1yWurdsOdahuDXGAS5eyUbuJ/U5xUkqJgcVpc8+FijSSB1UsO7mNz/Q48PJ8sOJNta8D3sBli61ENCvfunOI6Jm3nYltdnH38zUcq1JWBnzDWdEpECScKakvH/4CgBnjoA==",
            0,
            16,
            "eNrVlN2PmkAQwPu38Ow1LMh5XHIPoreIUTz5hqYPuwuGjwWNIopN//cu6HkXm0vTNG3DA2F3Zpj5zQcDhN6Xb9xmu14lNNKK1fpzEnKPA74P5IHU43YlKpN1oY25R9DjygjlzZHvcStEXhXstkUkam3EviQIzb3IZlEV0Yu2yOaoJLFVb1qzu8ZXkkcv0RZuUR7NzdYu2RkRCuv23ATe79pjHpVojErEPXJRPS09ge4NAZaBqd3PR4cEO/IGFwHFhVGRgpqBC7PoTXfAKpQCb3orr31XyrAArFCFdQiVigiUR66819L1cTZicUSd970pk0mFrcon5BkbLPSTRcKf9QKoAqjEvlC+kEmjk05auhlo+VXe3LHn8TsmW2FXzmwVpogPdr4bMt36cOPnZItGHE6c9juWa0xyfWqMtHuNwoM71sd2BjzddspALUX0TNdmTvu4IPKLqe20ouE1AKnPORLhWIXs25n1zOIbe8zOc7N/mI+H7FFkz2zrECNHoaTQK5zDHctRYlyJllx09rHyXaMKvWWySJf1wlpKekrY225z8gX5hF2H1Ui/rcGKqJD1xbB8IabMps3j0r+MxeDnacYvLF9kb3CutyER1WZxFPl8V2JWe96eTDfYhXXTOy15qGb1QxWeePnCePBdug+hThnLPlB/ZWfUyOVZD7VWPxMvtXvjtYO25x/6SVg9isBRmB8QkyK78TW9sBvUd4GC1eOGzVnazKqWOZbPQ2VpXX2x/gJp6bL81Gb2zn1/7UujczylIDnMAm+eLGgZnucF1tijDs4p3/TaBef5ClR5gUXDvMz1JsqbWg5bHfJ0JtepnUNWI7nEE2oF7pH6jDMYXf+Jte/pI6zKKRKczLHD8XVGRWXne5SSjM2JKgOSNHMF5eHw6Yn73vt5gTR/+LvdcfdueYCPlgf/9/bG7zIKHWAUO8DY7wCj1AHG+w4wDjrA+PBPGMEfMcodYAR8FyBBFyCFLkCKXYDsdwFS+i+QXz/9AIYibU0=",
            0,
            [
                [
                    50863834,
                    7041975,
                    88816,
                    252032,
                    134522,
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
            "eastus",
            "USA (E)"
        ],
        [
            50864865,
            109775243868444193,
            "{\"templateName\":\"GameSession\",\"name\":\"3a8e2f7a-05b9-406a-a45e-aa81d8634a47\",\"scid\":\"00000000-0000-0000-0000-00007d18f66e\"}",
            801954,
            0,
            "4 vs 4 Original",
            "4 vs 4 Original",
            1,
            "generated_map",
            "eNqtUt1OwjAU9lHMuXWJW1cWRsLFUIJEBUTuDDF166Ch25qtgINw43N44SOQ+FbEh7Dt2HwBe9Gc7zs9f9/pHhIiZqWg0HEs2LL0npbKxD52fN9RVMRi4yokyWUBHdu8Ggttv0Dw1A/AgqA6XZhbkKcRdJDnOa7dchG2gGfhysStmfbYLm752FMpEyLDpakHcEY38UI9aXuqHs+kQRAvVOo7rK7ela7yLzjoduuak95gqBqDa322Z16MSKI0gZ+P4+Xp++t0/AQzCeFsR6PHxq9ZUtJcqzE3gQOaPu/0nAgh7NbUAymztVRKonYLNWyPZYpq29i2m9izzk5NTLWejXu8yY0qe0heIyKJbuHQxIY0bXZJOM+2/Xc5WRV/eEpFjZMsqra41+aEhCszg0om4mG6qWYT8YjKymTF7dui2mNBA84ZSUM6oySp0oVLSsz/OFz8Auy/suY=",
            0,
            16,
            "eNrtmW2PqjgUx/ez+HruprSCdpL7YnAuCFEcUR43+4IChoeCZkBHvNnvvgWdUWeH3N1kkxkTXkF72tM/p+fXI8jBuz9+9jbP61VMQyVfrX+Pg979EHCY79/1itIr43WuPPbuubteGXpZfQvueivPfzWw1rPnh80YiKEwqNt5Ogl3IT1Z83TqlX60rDbNsG+1rzgLn8Jn6dnLwumiGRcXeugFVXNfL7wtmtssLL1Hr/R6972wUksb0q0OpdJdKMJ09BITE29I7lKS6zs/pwvXktKwti0a2wuRJd611XP/cU7lWHxKILcMZKkKJHHnQwo8C2+VZL2fjNg6SAOOrbI+PjdkfPBsfUNgP57F4GiH3M6VxMiB5ZM/rm38QUk2AyV766/bxLZBwfpWxMKpIUuJB9zCsQJmW7+883MwkB4FY/M476g/8kyR+rm2I5lUMA08mxcr8clm7HeOpe8Cex7Pknk1W855LfHZ1WjWdCA+EMtkz6C917jyZYnFTV86MKJsjKqPFOEU35StAaZJCmZLB7Erd4yHzvuywdYR8bEtRiw2wBirG2JJVR1bJR7uJtVwFxwAPml8cSy6DSSNMi1bV/7VOL3yLMBirDT2CfLx00IpLvQabrMnrX5iFo/cNUXmh4v8PH3nSz1p16ljcSKR9xuWB0mdS0pqLh0gifPlm6/Izzh+brHnk+vcuN6X2mbaYu5nUura03hGy+C4n1JFbGqSjAK/UgSLO+6/K+MZQfrilHebMKtj+dDYPFtj/Ro1MonFCJdkTJeutacO0+mO3nJ27djaiMg48aCZmkbw+JZDSCwcm1I/ZXkiY86P2ZwxeOj9dfdPtjmuPwDcQLiiG53p5lrpBgLPoy9C96iF7kVH97+ge68dlEo7HLMvGNOXJt5jcEna3M9oyWLUaFr+KPV5KolPSxBf0Q/NhK2b/mqcWZ8SDWX7iWGol5S9ks/ioG9a/UA1cuWAXp02KY1mP06+8qP2QDYjYkgFIzYimUZrX7qpJXPj0ldDqOhktI755iN6fTlgOcQ0XRDMtJWhaW7ZnMs9TAngd4GksvX0HbGocJm7PqeyvTdfqS9CU6NENhOmMz3nSBT5QC0I1J5dSzd1MH07GXx5H4WWWc0hLggyKzYHruYP3z8kG0JhyCH+Cuz+GWzYBjYECCPIdWR3dbur259et+2Wuo0EOBAguKKbP9ON2unmh4zvju6O7o7uz6Z7spTww8P3j+u3gIZo+I5w4Ux4v6vfHeEd4V+9fqOW+o0Rxki4/qg2ONPNt752oz4PYQd3B3cH96fDnbd9VAM8RHh4TffwTLfQSjfGA9D9OO/o7uj+dLq1tldvrs/3EYJXcOMz3IP20j2AgtDB3cHdwf2l37xrAi/Y/nbxZ/ewDW7wf3LNXXH9XzXiG9DIgVsQyd2CSHgLItEtiOzfgkj+U0T++dvfb6nxlg==",
            0,
            [
                [
                    50864865,
                    801954,
                    1080,
                    84343,
                    129267,
                    0,
                    "/10.0.11.19"
                ],
                [
                    50864865,
                    1454332,
                    87959,
                    2767016,
                    137266,
                    7,
                    "/10.0.11.19"
                ],
                [
                    50864865,
                    2268135,
                    2356,
                    2299729,
                    2039321,
                    2,
                    "/10.0.11.19"
                ],
                [
                    50864865,
                    3627620,
                    8671,
                    715777,
                    2058393,
                    3,
                    "/10.0.11.19"
                ],
                [
                    50864865,
                    6383820,
                    -1,
                    562606,
                    2039321,
                    4,
                    "/10.0.11.19"
                ],
                [
                    50864865,
                    9399364,
                    14116,
                    2961962,
                    134522,
                    5,
                    "/10.0.11.19"
                ],
                [
                    50864865,
                    10523984,
                    6724,
                    3577231,
                    199703,
                    6,
                    "/10.0.11.19"
                ],
                [
                    50864865,
                    11470176,
                    11735,
                    4267851,
                    106553,
                    1,
                    "/10.0.11.19"
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
        ],
        [
            50864987,
            109775243868517347,
            "0",
            8457833,
            0,
            "1v1 noob",
            "1v1 noob",
            1,
            "generated_map",
            "eNqtUt1OwjAU9lHMuXWJ+1NWEi42RSQqIHJniKlbBw1d22wFHIQX8jV8MduOzRewF835vvPX850eocByUUsCfc+BPeVPpNZmiEIPIU9TGc2tq1K4VBX0XRs1lcZ+h/g1TsCB2J7hAJYOlDyDftAL/B7yPeQ7wES6sXlbqj2+G4Q3CIXI0Z1Vurb9AM7oLl/pkOhW92NCWQT5Std+DPWVXJk2/4LjwaDtOUtGY/0wuDZnf+blBBdaE3gQ5c+3uuSClgTsLJjRA8leugjD4pqURo+lTR0R/nbQovkocMOWeca12CrNBl4QRS2bUKGpyA1dt0s9C+21xNwI2rmnu9LKcoTiI8MKmxecutyU8G6ZmDGxH36p2ab6w3MiW1yIrFnj0ZgznG7sCLqYzMd814wm8wlRjUmr+89Vs8iKxIxRzFOyILhoyqVrgu0HOV38AoUwsWo=",
            0,
            16,
            "eNrVlduOmzAQhvssXGcrG5ZsWGkvlqxMiBKyIZyrXtiGiIMhKCEkpOq715A03aaqqqpqK65sz2/PfB7PyFAcfPgklNvNOmGRXqw375NQeBzdyw8jSRoIuwpXyabQX4RHOBCqCOftFAyENaZfBb7aYhq1UxHII0mRWkORzaI6Yhe5yOa4orHVlN2+u9ZZkkev0RZtcR7NV92+ZGdGOGy6eRt5v+umeVThF1xh4VGImmnliWxviqgKVvpwPj4kxFFKUgSMFGZNC7YKXJRF37QD0ZAceNNbe+O7ckZEaIUaakKk1lRkALvKXk83x9mYx5EM4HtTbpMLW1NO2DNLIt4niwScdRHWAVJjX6xe6aTV5JOelg96frW3a+J5YMdta+Iqma2hFINg57sh1zaHGz8nWzLjcOKcz606zhg7KqOFUZMc7TiDzM8lenLR7GPtu2YdestkkS6bhbWUjZTy0e5i+qJyIq7D72DcMq6phnjeTMsXY8b3TM2xPrzkN+MxwDzNwMLyJT7Ccz5MmWo2j6Mq57Ua89wAezItiYuaNrd6MqpnzagOT0C5MB58l+1DZDDOsg+0X+0zG+wCnmO902cSVV5X+u4Nrx10b/JTPwnPRxE4KvcDY1pkN76mF3aT+S5UiXYseR2kbS3pmWP5AKlL6+orpjmUly6/n9bWxvfv0mqOpxY0R1ngzZMFq8Lze6KGeMwhOQO00YcuPL9/oCkLIpmrS92VUd7m8rnTsGdwu8HsHPEcKRWZMCtwj8znnMH4WrMb3zPGRFNSLDqZY4cv1xqS1J3vMUYzXieaAmmiD2cWUp6fn56Ez4MfO7ztwDfNffemu+HPuhv8vb7+XUbxnzDCP2KUesB43wNGuQeMwx4wPvSAcdQDRqUHjBD0ARL2AbIPXw3sw18D+/DZwP/z23x89wW4/03K",
            0,
            [
                [
                    50864987,
                    8457833,
                    7542,
                    2192196,
                    2058393,
                    0,
                    "/10.0.11.23"
                ],
                [
                    50864987,
                    8553693,
                    62425,
                    2271075,
                    131384,
                    1,
                    "/10.0.11.23"
                ]
            ],
            0,
            512,
            0,
            300,
            0,
            0,
            null,
            "brazilsouth",
            "Brazil"
        ],
        [
            50864915,
            0,
            "{\"templateName\":\"GameSession\",\"name\":\"39676d23-823e-4153-9ed7-59f6aadddde3\",\"scid\":\"00000000-0000-0000-0000-00007d18f66e\"}",
            10203850,
            0,
            "unnamed_session",
            "unnamed_session",
            1,
            "generated_map",
            "eNqtUttugkAQ7bfMa0kqchMTHqA11rRVa31rTDOFRTcusIFVi8Z/716E/kD3gcw5s2dm5wwXKJCvW05gbFtwouULaWXohq4dhrakMprrVCOwFg2MB/rWgqv4E+L3SQIWxOZEsLGgLjMYO8ORF/i261vAqnSvZQcqE8OB43qh78uKBYp0p9sB3NBjvpVXRlLVsEpoBPlWVn525Se5V03+BcdR1PVcJtOZfBg8qHO68XyOhbQEYiaQgh4CGT2T7K1PKRZbUisfNlozJeXHWZoVjjwzn2Jesa0OQrKB4/hexya0UlQQhG4vvRncK1fKyEGHFsda+3GB4itDgeoF116bkrJfIjJWnSY/Yrlv/vCK8A4XVWbWd1HhEtO9HkEW4/msPJrReD4nwoS0efremg02JGaMYpmSNcHClEt3BPWPcb37BezfrfY=",
            0,
            16,
            "eNrtVV1vmzAU3W/JczvZUJJQqQ8llQlRQhrC97QH2xDxYQhKCAmZ9t9nSJa2mapp0qQNqU/Y95h7j4/v0YXCzZdvvWKzXsUs1PLV+nMc9O4hEIA4lMBNb1viMl7n2hMP3vTKEGfNkgMrTH8CfLfBNGyWApCGoiw2gTydhlXIznCeznBJI7Mu2nO3TbI4C5/DDdrgLJwt23Px1ghxULfrpvJu2y6zsMRPuMS9+15YT0pXYDtDQKW/1Pqz0T4mtlyQ3GckNyqas6XvoDR8wfZERZLvTq7jtedIKRGgGaioDpBSUYEB7Mg7LVkfpiNeR9SB5054TMotVT5i1yiIcBfPY3DCBVj5SIk8oXym4waTjlpSDLTsEm/2xHXBlsdWxJFTS0UJBv7WcwKOrfdXeY6WaETB2D79t2x5RthWGM31imRoyzlI/L9Yi8+Ydag8x6gCdxHPk0U9NxeSnlD+tdqaniAfiWPzO+jXHFdURVw3w/SEiPEzE2Ok9c/6prwGmCUpmJueyL/wpIchUdXidRT5tFcirg2wxpOCOKhutNXiYTWth1VwBPKZ495z2C5AOuNcdr76u3NGjR3ANdZafCpS+XmpbV/xtfz2Td7NE3M9ct9WeB4Y0Ty9yjU5czeY50CFqIeC90HS9JKW2qYHkLIwL7kimkFp4fD7qU1vvH2XBrNdJacZSn13Fs9ZGZzeE9XEZTbJGKC11nfg6f19VZ4T0Vie+64Is0bLxxbDrs7jOrMyxDWSSzJmpu8cmMd5+qNLz649Vx8RVU6wYKe2FTxdekhUtp7LGE15n6gypLHWn5pIfnx8eOh9v/nV4kM4AP3B8I3DhReHw/cdzv0twA+Hfzj8w+H/tcMbB74y9+2r+S28527wN30N3/j6TzmKHeB41wGOUgc49jvAcdABjsMOcJQ7wBGCLpCEXSDZhVEDuzBrYBeGDfw30+brpx+vJGY+",
            0,
            [
                [
                    50864915,
                    8170678,
                    11121,
                    1864338,
                    2039321,
                    1,
                    "/10.0.11.19"
                ],
                [
                    50864915,
                    10203850,
                    88173,
                    3419884,
                    2058393,
                    0,
                    "/10.0.11.19"
                ]
            ],
            0,
            512,
            0,
            300,
            0,
            0,
            null,
            "brazilsouth",
            "Brazil"
        ],
        [
            50864628,
            109775243868280745,
            "{\"templateName\":\"GameSession\",\"name\":\"c1e11e45-57cb-4e04-8dcb-74b84178a21b\",\"scid\":\"00000000-0000-0000-0000-00007d18f66e\"}",
            11034775,
            0,
            "3vs3 Max Lv45 No R a t s",
            "3vs3 Max Lv45 No R a t s",
            1,
            "generated_map",
            "eNqtUdFugjAU3bfc15GMSmFg4gNuxplt6pxvi1kqFGws0NCqY8Z/X1sEf2A8lHtO772n99wzFESsG0FhiBw4sfKVNjrEEUZRhDSVssxeSUVqJbushTDxF8QfcQyO/cXxZAQbB+oy1VkRwhh5OPAd4FWyh6HrwIHpm4HrYT/0kedoZZXsrB7AFT1luU4JA63HK2URZLnu/YL1Mb43Mv+C49Go01yOpzP9MHgw3+nKizkptCcwpVtW51IQKcGOQjj7pel7n2BY0tDa2LGxlVNafv4aCx5DD3XMG2mqg9LsIPQHXseOWaWpIPDdsC+9+dwSK+On26HFsbaunKH4Toki5gWXvjahZb9Lwnl1mvyo5V7e8IqKDhdV2m7xbMIlSfZ2BN1MZLPy2I4msjlVbcjk8zZv9yhpzDkjZULXlBRtu2RHienmXu7+AEwzsK4=",
            0,
            16,
            "eNrtl1uPmkAUx/tZfHabuTgo+7a4ATErrijXpg8zA0ZkQLMiu9j0u3dAu7fWNJs23dr4YBjOmTnz48z5HwSi9qcvrfXdap6I2Mznq49J1LqEEOBOt0varU1Bi2SVm9fS2G4VMc3qIWi35pR/d8i7O8rjeogA6WEV14Y8vYnLWBzceTqiBV/MqnUz76IOlmTxbXyn39EsHk2becnGjmlUNeN65+2mGWZxQa9pQVuXrbgaFj4SWxvpRTg1lVH/PmGuumZ5KFhulzwX09DT0/jJd88MnYT+8LW9CjySMgRnkaFXka6VHAlAPXVrLlcPN325D7ZA4A+ljeSOoe6ob68Z6iTjBOz9CJahri0CVNzyQe0jO3O57prZo72+Z74PNtI2Z56aOoa+pCDcBF4kfav7V3F2DrYX0cDdr5s2nAvqaoLnVskyfSMZiFyXmMnB5zyUgWeXkT9JxstJNZ5NiLXk8uo0ewZI3THPlc9gvWacc0OXebNnAVoIOWdo903lkN9U7gFGyxSMZwGWV7jPh0244ch9NHV/ry1kboAzGK6Zp1d1bs2kV95UvTLaAfXAeB94YhvplpAs29D41Ty7oh6QOTYb/w3m6u3U3DzjdcLmTI7GSWQ+8tDVZBy44Hn6KtbwwG6LwIMaMx7Wsg6WdS2Zqa5NHPmbPcZa8AySiSefz6hr4+W51D7X13Ke6Wnoj5KxKKL9eeoV84XLMgF4ZSoe3J9/aKhjhu3poe7WcVbn8qrxUd+Sdks4mS5zpBZsIGah9yACyRn2H2t2FfhWnxnqkiI3dZ3o+rGGsLYJfCF4KuvEUCFP5JocXLW+tn+UN+mSDsQv1Y2e1A2PqRsChZCzuM/iPov73cVtHRV3RyUIKy/EjZ/EjY6KG0Pc65zFfRb3Wdzv/uYeHBF3rb5nur549p8cv9db+62gneMdqIsU5S+DKirGBIMXtN0nWHL8S0d+5yD4j/fL6blfnvvlT/ul/V/1S//t/VI5pmzwJzUNf6tVdk+AsXcCjOoJMEJwCpDwFCDRKUDiU4DsnAIkeRfIzx++AdMOlKc=",
            0,
            [
                [
                    50864628,
                    5495236,
                    11074,
                    3842521,
                    129267,
                    2,
                    "/10.0.11.15"
                ],
                [
                    50864628,
                    5754135,
                    57615,
                    3888989,
                    106553,
                    1,
                    "/10.0.11.15"
                ],
                [
                    50864628,
                    6933530,
                    7189,
                    314942,
                    106553,
                    5,
                    "/10.0.11.15"
                ],
                [
                    50864628,
                    11034775,
                    10349,
                    3891719,
                    2058393,
                    0,
                    "/10.0.11.15"
                ]
            ],
            0,
            512,
            0,
            300,
            0,
            0,
            null,
            "westeurope",
            "Europe (W)"
        ],
        [
            50865024,
            109775243868518488,
            "0",
            3798905,
            0,
            "noobs no rush 15 min ",
            "noobs no rush 15 min ",
            1,
            "generated_map",
            "eNqtU1uvmkAQ7k9p9rU0XWC5mfiA1XOKerxVa5oT06ywKnWBFVAPGv97ZxcvaZP2qftA5v7NfDOcUULFtBIMNXQNHeO0xyoQiUd0z9PBFMUr5SpKmpfFLWoopPyK/LHvIw356nWaaKGhPI1QgxiWKysYWEM8C7eoAcI+Bo+BTWJj7DkaIJfhRuEhdNU+r9YQ4tqAx7NSaWi1htpfCHxaHyTMf9H9ZvOGOWo9B9AY+iTf8WoXA5oAJ2hEebYvGFJjUB6fWPRyd0orrVguqViorGeWfj0BSZ7jmvrN0qdVti8VdbWhFWegOaap43vWg97aMJE03t3DQ67IOKPkR0RLKsEv99yQpfcVUs6zY+etHG2Lhz5h4qYnWVQv7yzFEQ2l/fWMaB4GbSibHYzxU7u7m3SGyXybLOO35bxdswUh31gOMRXfzKJub9ojx6c5twzD282CK3NQcySLfzRgzcR1iWtj27EcC5seNHCpQ6ZqNrFfKkzP9FwTkuOizYTyFBLH1FBaE00wfi8yASM/Gg0n1mkQvAzy2TwjBk8CRz/4498b1fvBruvE7twNfhZB/7tfruN0/UejBFs2NmzdkIfpyLP9W59wt7r+rz5v13JZQL5YBemhvhKxGrCyFiF3ua5/h4L5nMc0DdmU0aReT7hhVG4HX979Ao3JDFQ=",
            0,
            16,
            "eNrVlF1vq0YQhvtbuPapliUkIVIv4tiLQYYYzJepesECFh8LRgZjcNX/3gGSk6McHVVV1VZcWOzOwMwz74yHx4tff+eq8+mYslgpj6ef04h7Eh6kRwmJC65ugiY9lcqKe+IXXBMHxXBEC+4YhO8OuJ2DMB6OGAmSgPnBUObbuI3Zm7vMtaAJE6uvxve+DMHSIt7FZ3IOiljbj++ltRkHUT+eh8yXejwWcROsgibgnri4VxsPs4uJSePvlXvt5ZpSR6po6TNamm1Ysr3vkjz+8F2pTETfUz/b+4Mr5hTzViSTPiLLNsQMBa50UbJTt32BPIKODp4KNrG0ZekWeGZF8V36mqLJj/nWJ8vkgJtduBl84k3Jqgel+Gof7tTzUA22I3Wl3JZJFiC/PrgR+E7XT3FutmAm0cYZv4Nak7DQVfNFuVcKCWuMyOa66uzc2VEnOlNXrWJZ9cz1WtrtlVopB16TD/upxhB3bQTfbq015DcvFM7a/u6qrZ7ht5S2mzqF+rK9bUBNamZnzr2VM90qVcfBj0grumZvhV2UE3NnoRRYb6AVijwtfc2eh3w1FYx3PXJaXMG+vkzxn69HZ6r74DID9L+BPgmVGRp6oKTKu0+jmORUcBDogbQsR6/WQYAnP2mjQ194Fskss4Tl2J+hvnEOhGUCvUE21k++y7OxjrIe58GHWvWVIuqrHOs3eO7HnqPYW7JB9+N0v0L+C/S+D1w+CcscalHabf/YboVw0hQYQ5nAfJmW7+otLcy/es8OC9ZAjnT095Lwpt1XXkd2eqjnh3EOBcl97BhDHOiP+DnWGzuCeW4Mt6sDl1wO2B56SECLpWGvP2J5ahPbJA3croKcbNDO5dGHz3GuvqAmvjzNnDfFhrnjRccVq2gDvWZNNPXCbK1CQnZBLr4sNYFXsY8ZZjewZ76jJqBRS91OtLFTg2bAaUzzAjkDmdyMomth1plPnI3Rf/c/XdFhbj1lnKuj8fwL98fi+w01bJBvltOXb7YT/6PthP69vfR3GfEMGIUZMN7NgFGcAeP9f8LI/yPGhxkwPs6AUZoBI4/mAMnPARLPAVKYA+TdHCDF/wXyt5/+BEMej4U=",
            0,
            [
                [
                    50865024,
                    3798905,
                    67358,
                    61431,
                    2039321,
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
            "westeurope",
            "Europe (W)"
        ],
        [
            50769515,
            109775243815120963,
            "{\"templateName\":\"GameSession\",\"name\":\"b22cd39a-71b3-4a80-93a1-58e2ba53f87e\",\"scid\":\"00000000-0000-0000-0000-00007d18f66e\"}",
            11478923,
            0,
            "èæºå¤æå·²æ´æ°è¯ç¨Qç¾¤485069332",
            "èæºå¤æå·²æ´æ°è¯ç¨Qç¾¤485069332",
            1,
            "generated_map",
            "eNqtUt1OwjAU9lnOrSR2ZRkbCRebEiQqIHJniKlbBw3d1mwFHMT38B28kSueSKNvYdux+QL2ojnf1/P7ne4hIWJWCgpdqwVblt7QUpm2Z1ueZykqYrF5KiTJZQFdZLzGQtuP4N/3A2iBX50ezFuQpxF0PWy7joM6yptn4cqErZl6wKiNOi5yVMaEyHBpygGc0GW8UC6uo8rxTBoE8UJlvrbVFZzrIv+C/V6vrjkJBkPVGFzosz3xYkQSJQn8vL99Hg5fx8P3xxHMLISzHY3uGg/NkpLmWo65CR3Q9GGnJ8UY2+2auiVltpZKyjZC2KvZgGWKslzXwk3sSWirJqZaUFSj8SY3uuwheYqIJLqF1yY2pGmzTMJ5tu2/yMmq+MNTKmqcZFG1xr02JyRcmRlUMhEP0001m4hHVFYmK66eF9UmC+pzzkga0hklSZUuXFJiPsjr2S/05bUb",
            0,
            16,
            "eNrtl12PokgUhve3eO1sikJUJpmLxh4QotgiFB+bvaAKDB8FGkEUN/vft0Db0d5xJ5OZTK+JVxR1ilMPp877BjjY/eOvznqzWsY0VPPl6vc46HzkuN5gKEK+2ylKv4xXufrMJrudMvSzZgi6naVPXgPsbuOTsBlCwIs85JqJPJ2EVUhP4Tyd+iWJzHrdrvvQJIuz8CXcyBs/C6eLdl1cGKEf1O242XlbtMMsLP1nv/Q7HzthrZUOpFsDyqW3UPvT0S7GSFzj3KM4NyqS04Vny2n4JbbDiix4jvZ2vnZtIcWQMwNFrgNZqgikwLfFrZqs9pMR24fXgetobE7ILUU8+I6xxrAXz2JwjEOu8mQpcmH5QsZNTDioyXqgZuf55h47DijY3BLbYmopcuIDr3DtgMVWuzd5DhZvRMEYHZ9btJyRjyRKcr3CmVwwBoE9F6vxKWbtK9c2qsCZx7NkXs/MuaAnhF2tdk8XigdsI/YO+lvGJVFkVjfDdGFE2RrNGKn9U31TtgeYJimYmS7PrtyxHoZAFIvtI4nHeylitQHWWFtjW66b2qrxsJrUwyo4APHEuHNtug1knTKWrad8a51R+zZgNVbb+IQn4stCLS54La89k5t5YlaP3EMSy8NFJE/f5NJO7AZ1bU7Cyn7N+iBpeklNkekCWZqb51wRyThhbrP3U5reuD6XJoYcKSeZnHrONJ7RMjiep1xjhyKcUUBqtW9zx/P3FHGGeWNx6rt1mDW1fGpjvqOzeZ1amcxqJJZ4TE3P3lOXcXqjc8+uXEcfYUVMfIhSZAXP5x7ipcJ1KCUp6xNF5Eis9iemLD49ffrU+bv7b4k3CrwQ94cLdXPvpu6vkjZmJPR617wQDL4Aw1vAHBRhf/Bwo4cbPdzop7rR4te5EX9T3DzHD3u/2Iz+A7R3G3QA+/3/D6hwExT0BYG/AuV+DBQ+7PJ97HKvH9RaPxzlHIzprq33GFxa15xktGQ1apnMz6UxT2XpxQTxlZ1ClLB902+tQ43ttra1n1iWdmlbr1bK6mCsb+aBWuQpAb2y75RGs8+nXPmRPVBQhC25YBYY4UynTS4D6cncuszVWp7kZrSp+fprdkiUgPUQY7qwRMZWhght2TOXZ5hiIFSBrLH9jArbtH/Zu4TT2NmjVxstQqRTrKCEcabnXoRRRIBWYKhvPNtABpierZYo+yi0UT2HYoF5VLNnyqkDnr5X1P3vsMmHqB/fQI9voDv6BhrcFjcPwPAh7oe4H+K+V3EPb4kb/MxfBu6HfhnEO2DkwD1AcvcACe8Bkr8HyN49QArvAvnnb/8ABn2u6A==",
            0,
            [
                [
                    50769515,
                    11475441,
                    -1,
                    4270589,
                    2039321,
                    2,
                    "/10.0.11.21"
                ],
                [
                    50769515,
                    11478923,
                    -1,
                    4271949,
                    2039321,
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
            "westeurope",
            "Europe (W)"
        ],
        [
            50864750,
            109775243868346664,
            "{\"templateName\":\"GameSession\",\"name\":\"e68a0d67-6da2-4869-bc42-f8bc3f63fbc2\",\"scid\":\"00000000-0000-0000-0000-00007d18f66e\"}",
            5419669,
            0,
            "7 vs 1 Mega A.I",
            "7 vs 1 Mega A.I",
            1,
            "deep pit 7v1",
            "eNqtU0tu2zAQ7VEMrlrEhSmJFCUDWSi1609iy7EDp24QFLREy6r1YS35Dy+767bnaIEuih4oPUdHUpwgQZJVtaBmhjNvHh+HOxRyebGRAlVxGa386FRsUFUzqaFoVMVaGbn+BFWVMkpSPk+T3IQ0W2b2FbKs8xYqw68OlnWMrstoHrmQpTNiEIaJXkZB7Mxy+IUPOwBKqIkx4IQ8daZ5Q4RuvXcTD1IMqEqCOM09NPEsy2oSWE6OYLH+i28dHx969k4aLSCGKtm3uo3LLg9BFOQKIUvST0tsqaD8LDzwt8Lt3GVkUb4R80yP67y0IaLBFlWJahJTZ6pJD9EzvokX6VM7J378VHhwL3oR6Gfi4oNnL+e5RDsUfnJ5yjM2+7taR0TFzUI1D4J4VV+nvVly7/eFPPhh7BZXusvMHney+NUO8bnTqgFsR2kYfSNN2jjcDieaGLTXjXahFaQMxRxyTqWx1PSB5P0vi4B1vSM+bPq3egJmLwN/q+maohLTpAqFs8KKKRDYFykX+dnkYpz3ZIpuECj2k5qQ+U6S9YGZjArlb35/vfn18+/3bzc//rzuCI+XrNYbEOCetuGo8TRd2Z/rdq056muX20u37T2kbYadijPyt3zMsTm0Rx+9pNZ4RJsRhTDNxIypmgr0Vc18jrWCTcVQX6L9YKQesB2fVd53FRrPfNLtjvpiWrftR2wv2+tpz03IYN0JP1C1eb6uDGfWI5FVomNiGMTQsc4oo/h5upRShl9iq2CMS71YLgKe+nGE9teAIyetaFnMvpx0RVqYgDH2ipeeCCsIfB454kLwsJgxZyp4NmJ4/+ofISpOGQ==",
            0,
            16,
            "eNrtmFtzokgUx/ez+JzZahoxYarmQRO5OILKpbls7QMNWFwaZAOiuLXffRs0mmTiTs091ubBArqb0/8+l5+nYODVH3/3ivvVMiahnC9Xv8dB7z3XZ/jBgL/qlZVXxatcvuu9Z656Vehl7S246i09/2GCPt17ftit4flrwLbPeToN65AcZvNU8So/MpqiW/autRVn4Ty8F+69LFT0bl1caqEXNN19u/G67G6zsPLuvMrrve+FzaSyIVlrUKhcXR4ot5sYI77AuUtwrtV+TnTXEtLwNLfBosC59uT5eONYXIohYwSi0ATCqPYhAZ7Fr+VktZne0n1YFTj2hI5xuSnyO8/WCgz78SxxSjljltjiU1MUEg/wm0AkNc6VeJaX8XGcpc+kCpZ6t1+FobZwLPVey7aR284lw6d2WLXVAgK7e+9azoTGAWRM9cQzcaJMgTtTDFR7MAVGyrlmhlaayc/dHeDleBP7rBYFEtod9O+wyAN6Xyl0f1fkSnq/nSbDjXJHfxIoqS8jP1Mn2q08kFOw1XaRPpO0nZ6MqpC4mQKRoeeRpOc+P9flUs5bf2iM3+x96MNtHdB3p8aYnkNbY3qv6P29/bsRP5XKmPov0c1FPIvlvrOb1J6ksQYsBANosoXkHWIL2x0X+dwAcav5eP7WN7laYrZ9F2zpXIqzDR0fr/f2h5slAp3/HIssaHx3GHIRFgloYyzH8sOcgqGQYha1vgBKkoKZ4bD0ynQxhiqNO0No/BKDHXXxb8/X5Rk7imjsgQnVlWsxpDtHG1+aby49q3onc+pdCtUdve5jDEJ7RFr/H2K+ofuvaW41nsVEfp62fqinzU09ZQ8+pRp9UaD5qxmupdY40z63zvQzUrU50c03PHvw3VEvElFDz3PWjpMJqQvRorVD48M9t3XQDmi9VAtrW3qWsHagSW1NRgtToL/xyZY9qUJTiD1rW9A9Ses7iwGnOYQ2LjuJXLHNywLbe9s07xgOWVwRSPsa2cdCq42MB2YmrF2Rrzy7IMdahGRHxxMXTSLqoxpbW86EqKQ+ozoXx1ryRGG3yLa1AyviCkhaNJ9w4A63eWvL9B3ED4cfPvT+ufoUgDfsNby+eQpAeAIgcxaALMPe9C8egNv/BOC+IKkOpnaFUUSdPfeldo5rg0zBdRzfB90Gz4Dplo4V7E7BPa03jxAr8BNAJVFs3PKikYwZDKtCHXMzC02IN0ZzA34PQE1UxfT7ZhIBH6w22C4sN1GJCYq+Bgr2qwClb59BXGkwjEAA+L8ouMe6QHSFCQYIah+/DuLMoXCEwqRF70N+7bSFKHWFHz/MGSJPC5BngpehlWBWrVwaW+f5H9kRYGriiahyzfYcXXyXXld0i2ZmLDg18enV7GIcSGTT5aUEHkPrLGweg4sWdEJzKP3cOiRNCtxB/qaDW3Dw3UmvRvycnuecHdgCKSBma8cSmvC5rXyvPRBRhE2hpH8qFDpqC6N4D0BhdLIlNNgmIycjZVsfrv0YaN0c8sWA1pr2EhzX9J3HYEwx4OpAeIAcGTyucZ+Z0BpB+qFuyxCpBIsooTrTUy1FkQ8mJYbqvWtpSAOnRsMXt1FooWYBeZq3qOnyygbDFwHIUJLdAIZ7QkD2REB4loBgwHGvvQXUv7UF9N9awLcW8K0FvPgWUD3fAl7zzIDhnwKwfwIge9EAfD0tYKPunB8FQWpbPgOR4dk2zTAEaSbI/UBSPyoiM0CZs3OR+jEcBx+D7wHaJEqUjF8FUjD3UjTXxpFrJqodkiDVsxdAS9urM3ts3lrBX9cKakhN/hetYEuqRwx89+hDYP8cBMGP49+XauQuQOPgAjRen//m0ecgfCKU/Tah8BV+9B3+jI7/DeI/G+IWea0Q334FxLfLxfDDlxb2zU+BD/NN8OEvQCMDLkEkcwki4SWIZC9BZP8SRHK/ROSfv/0LsIU6cg==",
            0,
            [
                [
                    50864750,
                    5419669,
                    88379,
                    4008180,
                    199703,
                    0,
                    "/10.0.11.14"
                ],
                [
                    50864750,
                    7916195,
                    67931,
                    1548009,
                    106553,
                    3,
                    "/10.0.11.14"
                ],
                [
                    50864750,
                    8372789,
                    86611,
                    2098624,
                    131384,
                    1,
                    "/10.0.11.14"
                ],
                [
                    50864750,
                    11318015,
                    84434,
                    4181255,
                    106553,
                    2,
                    "/10.0.11.14"
                ]
            ],
            0,
            512,
            1,
            300,
            0,
            0,
            null,
            "eastus",
            "USA (E)"
        ],
        [
            50864708,
            109775243868323497,
            "0",
            8222997,
            0,
            "unnamed_session",
            "unnamed_session",
            1,
            "generated_map",
            "eNqtUttuwjAM3bf4dZXW0DJSJB5gmxjauIjxNqHJa9MS0TZVG2AF8e9zUtr9wPzQ+hzHdnycC2RYbOpCwJA5cJL5m6jJ9QOfBQEjKpKxDVUaS13B0LWnloXxP2FMBo79kY1g60CZR5QwcBnvD1jfgVSFe5t2kBTouZ7f59zzHGqsw51tB3BDT3FCR/gjtUuVtgjihCq/+vSZ3Jsm/4LHo1HbczWZzuhi8GDsdOOLBWYkCcxFgmvMI5WBnQRTeRbRvIsbFmtRGjG2NnEq8o8zCRAMuMda5h1rddDEctf3ectOpCKKcc56XepN5S5zbdR0W7Q8llaUC2RfEWo0N7h2uaHIu01imqrTy49e7as/vBZFizMVNTu8GHeF4d6OQMWKeJYfm9GKeCF048rq+Ttp1liJcZpKzEOxEZg15cKdQPs6rne/fmqvuw==",
            0,
            16,
            "eNrtlV2PmkAUhvtbuLYNDIvKJnuxuBnEKK7Id9OLmQHDx4BEEcWm/70DWnfXdNM0Tbol3Stmzjuc83DmvEEAvc9fuWKzXsU01PLV+lMccLdDAIAsD3rctkRlvM61B+4W9LgyRFmz5HvcCpEfAtttEAmbpcD3JUls9nk6DauQntU8naGSRGZdtMc+CixXnIWP4QZuUBbOlu25eGuEKKjbdVN4t22XWViiB1Qi7pYL60npArozACz9pdafjfYxtuUC5z7FuVGRnC59B6bhk7bHKpR8d3Idrz1HSjEQzECFdQCVigDKI0feacn6MB2xOqLOe+6ExaTcUuUjco0Cg5t4HvMnHQiVD5XIA+UjGTeadNSSYqBll3izx67Lb1lshR05tVSYIN7fek7AtPX+Ks/REo0oGNun95YtZ4RshZJcr3AGt4xBYu/FWnzWrEPlOUYVuIt4nizqubmQ9ISwp9XW9IB8xI7NvkG/ZlwRFbK+GaYHIsrOTIyR1j/3N2U1+FmS8nPTE9lTOPXDkIhqsTqKfNorEesNb40nBXZg3fRWi4fVtB5WwZGXz4x7z6G7AOqUsex89VfnjBo5POux1upTkciPS237jNfy2zt5NU/M+pH7tsLyCBHJ06tckzO7QT1HULB6KNgcJM0saaltejxUFuYlV0QyQVo47PvUZjZe3kuj2a6SkwymvjuL57QMTvcJa+xSG2eUJ7XWd4TT/fuqPMeisTzPXRFmTS/vWw25Oovr1Mog65Fc4jE1fedAPcbpjy4zu/ZcfYRVOUHATm0reLjMkKhsPZdSkrI5UWWBxFp/akL5/v7ujvvW+5nBJVEciC8MLj4ZXOi0wZfvBn83+H9u8MaBz7zdGvJsbvBW5v5dUPE1UP7fYbz5K4zCHzFKHWDsd4Bx0AHGYQcY5Q4wCnwXIIUuQIIuQIpdgOzCz0Z4m7/Nlw/fAQK3ZsY=",
            0,
            [
                [
                    50864708,
                    8222997,
                    56753,
                    1926614,
                    133008,
                    0,
                    "/10.0.11.11"
                ],
                [
                    50864708,
                    8253373,
                    31428,
                    1962586,
                    106553,
                    1,
                    "/10.0.11.11"
                ]
            ],
            0,
            512,
            0,
            300,
            0,
            0,
            null,
            "westus2",
            "USA (W)"
        ],
        [
            50865033,
            109775243868519420,
            "0",
            9191380,
            0,
            "4v4-350 pop-35 min-lvl 100+",
            "4v4-350 pop-35 min-lvl 100+",
            1,
            "mountain pass walls",
            "eNqtU9tu2kAQ7aegfa0rfFnbGCkPa+5KCBCgVRpF1cZejItvtRcMQfx7ZnchKFLap86DNZczM2dmx0eU0mJxKBhq6xqq4+yWHVAbG7rhYh27LQ2F8Qq1DQ1VnJa8kirAJoXQnxCZ9XwyI0JukIZIFPiEjIhQCURAOhEh3ZoQv1aIGemAtwcoX6L0sUCcRSKkPA786EYl3Fy9StCzhsosRG1Ldx3Ls7DpaijJg40cYhtDxNQt7OiGZWkwIA/WciyEzlZnFQGk5cBUSc6lhVaCxRDDx/8qmvwXm0jusufUH4yAGGoKqc/+4p6msHqU5tuM0zhrFLSqGjVNkgrJkWgSv7Jw/A4UXnpgpVj+s6wwYNn8FZ7M9LDnuKZnX7x39JBv+WcRP84/c8+vL6wcD2LH+sWa7Eq5qSNKf4WUU8Hm9J4bsEydEWQD/bzu7fl0U13tB1Zc7DQP1f0chTqlgfA/HREtg1FXbCMa9n/26+Vi6Wzm97tFyZx0qK4BIN9ZCZgx/hPlYbEh5gHvg9/1bDjh3nmtUHMqin+zHMswsefZhg2zwle3gcBJQRZytmL7Invato0xJMdVlxUyUok+cD+Z2jwJdzQLWNgYgN2YM87jLKpgA1fe/ddsO1k2d/vlfOU9GhOnah46s4+8b188ipOHvZfbozzt5tPxYHkXfeTtYgO7lqe7rmmZwN+0vL/Sbtkt61+0x5fLmsrLivm68UOe1+kZCharUbZTZ1Ws7hlXKhR7idS/VDGSJLEYfMFoqp4vWDMqXk8/fXkDtiM7jw==",
            0,
            16,
            "eNrVlN+PozYQx/u35HmvwhB21yvdw5IshCghG4ffVR9sQxSCIWghJOTU/71jktu9XnWqqqqteEAMHjPz8czXg9S7X76MqrfDNhOpXW4PP2fJ6AkjjLRH5W5UN7TJDqU9HT2hu1GT0kKa4NhS/tUBX2+Up9JUFQ1rKpILZb5I21Tc3GW+pA3fuV3V7/skg2VF+pq+mW+0SJebfl9Wk5QmXW/LzMe6N4u0oVPa0NHTKO3mTaiKI1HNJt7Y98vJKWM+rlgZC1aSlpdiEwdmnn74Tswy9Ticf7/eRYGeMxW5iWV2iWm0XBUKDfDR3h9Oiwnk0RwlCuewppeehS80JBVTx9lqv6ztAm1ZgHPPMvdUwafEEi0rl9mqrLP3dQ2+RZNsN32+hqlkHQXOGynOu1j69s9/jKM5kkVJwv6/B7swu0gRL8CTkbI6Jh72F1o89n2nWPn52b3El4Umpp6rYDs7ZVwju2TmX278F2ZhBexmCfljS6/BPi/2z6flFJ6ZUkMtd7xw5mRi3wNHuXmJKSkT3zc9lSJnlQjSxW7cbCyOXzd2bZeyHgTx7lpDrp7bBP5duC9wDnJkYC8342v8qYHD67l31DcEL52WFWYNNdTleSRv7/PObRSQNgnXUI91t3LXurPn8Pb62kQqvrDAhx44r3wm66/D+aoH6eOWCX0nbqTuBOzpz3HTRw45lOU+V1ZupMEbXftJdG55kMfA129jB71VvNm8YoHZSW3Y2WO76B7b5HKtqdRPFIhjYjoCWI6x9Vf7SEcDJVtldu9faLfaffB6ca+pH8bJoB5l7BsQB+14mX8Xa35jJyIKkMGscwU63su7YOemsfbgcd9jQX+Rvg7gfJbUttRGxb72Rfr80Ch5YebxVXNJH1s1OxYKnxVCkb0OkNLzxxZeMY1sbvemSgvvXcM0dGDdEV5hQo1A6zPhxsFZRMAZT97v3CEKnQnock9VP/e9ZPpx14w6CoXgOejEwohnUlcmfn7+/Hn0292fJ5ScIN8Mp0/fTCf0o+mk/Htz6e8yqgNg1AbAOB4Aoz4AxvsBMD4MgPHxP2FE/4gRD4ARKUOAREOAVIcAqQ0BcjwESP1/gfz1p98B4EKPHA==",
            0,
            [
                [
                    50865033,
                    9191380,
                    1328,
                    2797840,
                    2039321,
                    0,
                    "/10.0.11.16"
                ]
            ],
            0,
            512,
            0,
            300,
            0,
            0,
            null,
            "westus2",
            "USA (W)"
        ]
    ],
    []
]
```
