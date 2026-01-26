# [POST] /game/party/createOrReportSinglePlayer

**AUTHENTICATION**

## AoE4

### Request

```
POST /game/party/createOrReportSinglePlayer HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 2535
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Expect: 100-continue

appbincrc=24916&callNum=58&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&countersZip="H4sIAAAAAAAACouOBQApu0wNAgAAAA=="&createMatchKey=1&datacrc=-638535971&isComplete=0&itemUpdates=[]&lastCallTime=210521&mapname=ang_chp1_hastings&matchKey=&matchTypeID=17&moddllcrc=0&moddllfile=INVALID&modname=INVALID&modversion=INVALID&options=eNqtUstO4zAUnW+52wnCTZ2nxCKdVqWCoR2oYBCqKjdxEkPiWElKKVX/fa6dtLNhiReW7/E593HsA5RMLfeKQ0gs2Al5w/cQDn0H15BSCxKRQmhb0LSsbhsIB4Y1V/r8AlF0dQUrC2qZQEgHtm17lBDfgqKK30zKrcAbhD1CPMezA5s6gc5bsjbOTTGAPvqVZkj1XSxWVK2JIM2iKLqmuI1+4hZ9S6yb7msuRtMZNgiXeu16XN2xEg0BJrN1nKvBOmdNK2TWgBmMFeKTJ7/PNI2yPa+1Iyujn3L58ImG2AENXBzaOaG3bF9t269uRqL6Cn74b3sH3GunySmav9fGpwOU64S1THdzPGtjLrunRb9ZUVS7yUe7eGuM3sT3XJ3iskq6Rz3o44LFGn85AKvj2RjTjm+d6uZy/ppNnrxc+s/CS8jTH2MYUh55jRzXnu6u64mcpH+p+zraPNaB3PRmY86FTn5hU5dQ36e+S1z8EQ4ZBjjesaMsTS9quzE1USeaMVcGbHSJC/RB9q4fVyhS6Uy+d1SV3vH2rNpk3fdreFQUgsmYLzkru1njnDNj6vHHP5f2390=&race_ids=[]&results=[]&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&slotInfo=eNrtVltvo0YU7m/xc7aCwSRLpH0wdgZj2Thg7lUfGMDiMmAaMDau+t97BpzEmzRdrdqXSH5AzJwznDmX7/tsHt389ueoetptUxqr5Xb3axqN7pEwvhXGN6O6CZp0V6qz0T1/M2rioGBL7ma0DcJnB+yegjBmS4T4u/GY7ct8GbcxPXvLfBU0YWJ2VX/sC4uVFvFj/ISfgiJebfpzaW3EQdT1a3bxvu6XRdwEs6AJRvejuFs0LqJ7A+HG36i3q+khJbZUkdKnpDTasKQb38F5/Oo7EAWLvrt4tW96e+c5Yk4Qb0YK7iIstyGiXOBIezXbHZdTuEfQOM9dgE0sLUU6Ba5RETRO1yk3+BHf+lhOPNQ8hnPmE09qVt2pxYud7YnrcjXYtsSRckvBWcD5tedE4Nsd3sQ5WYKRRHO7/w5qTcJCWxhT9VbNjZXmSMslJ/3hc7aroWS/xrTSkH6w+QfpcaPWasnyNfiwG2oP0bGN4Nul+QD3G3syZfbxYTWbwCNL7tCHJLBlGpZaSwpcQ40i5JWq6dlnHVvPMdrI1dN1pndrUxe1LIS31dfkIelEHBt6pL3twTZUMMzFMD2UUDjT13GeXw53cKss59amJ8CbH/ptiKFiwT2yNOzlBHrPWfNFRRzcsdmp6dd22X1toxMnnXM8eA7dR1ijkMveV350zugCh4MZqr1/KYRD717ztfx+5h/GSaEfpW/LEIdPwjJ/E2txzt2gnsPLRDlWgLOMYVXNsaxb8JgvsWC+vKg7UJ/CsDfM/XkuzGe7chkWOPfdVbqmTTTgBXfEpTYpKMdm7fADvnxFWhPB2JxxXcUF6+VD7wtcDewatQoMPZIaMqem7xypB3n60xeu7DxXmxJFygJk57YVzV4wKsi151Ia5oATReLDlOFqIU0m376N/rp5rx+M4Rfa8eVCPPgPxYMTb+++Fw/038QD/f/iMf0c4vFv5PYVu/Bcu46wlAFIGTFKkg4kgPWKIJwTweb+kaRIg1p5Gik0MwW5r5mBsO/tM2GRtvMdnm4sEI2y7nvMQKbNVFGb5Ug7wXvIj4tdmbJatptLkn5Eru+ICgBmdRk/OmeFBW1Y3b2/k4RHk0svBcZW7A7q+TCOxwiIbJ3FgZmKb2Odc+cAI43uHGsQj72HgHzpQrYY4a2H11juooktnAbOsYI76SWBe59tH3xhkcCM3ouBI1bR/FIIjNYsJO6Z1IFb0Rf8IXoCe+bbiwR61BLnKFrIrqFnkCcT88kgDAo+6QWIPGqoj+253r3D/oywHxJXZdjttvrkpwmPfuLfwpXwV8J/asLrV8LfC1fCXwl/JfxnJvzvv/wNG4ZmsA==&teamIDs=[]&versionFlags=0&xpGained=[]
```

| parameter      | type       | value             | comments |
| -------------- | ---------- | ----------------- | -------- |
| appbincrc      | int        | 24916             |          |
| callNum        | int        | 123               |          |
| connect_id     | str        | ccc               |          |
| countersZip    | ?          | zip               |          |
| createMatchKey | int        | 1                 |          |
| datacrc        | int        | -4514551          |          |
| isComplete     | int        | 0                 |          |
| itemUpdates    | arr[]      | []                |          |
| lastCallTime   | timestamp  | 111               |          |
| mapname        | str        | ang_chp1_hastings |          |
| matchKey       | ?          |                   |          |
| matchTypeID    | int        | 17                |          |
| moddllcrc      | int        | 0                 |          |
| moddllfile     | ?          | INVALID           |          |
| modname        | ?          | INVALID           |          |
| modversion     | ?          | INVALID           |          |
| options        | str        |                   |          |
| race_ids       | array[int] | [1,2,3]           |          |
| results        | arr[]      | []                |          |
| sessionID      | str        | zzz               |          |
| slotInfo       | str        |                   |          |
| teamIDs        | array[int] | [0,1]             |          |
| versionFlags   | int        | 0                 |          |
| xpGained       | array[int] | []                |          |

### Response

```
[
    0, // result status code
    86651938,
    "54d65072140dcc75321b5da5ea4c80cd",
    [
        6,
        233334, // self profile_id
        "/steam/76561197333337299", // self steam_id
        "",
        "TTLv2", // self steam_name
        "",
        4275156,
        0,
        1,
        0,
        null,
        "76561197333337299", // self steam_id64
        3,
        []
    ],
    [],
    [],
    [],
    null,
    0,
    0,
    [],
    [
        [
            449911690,
            0,
            451960,
            233334, // self profile_id
            1,
            0,
            "",
            1666823722,
            5,
            -1,
            3,
            -1
        ]
    ],
    null,
    [
        -1,
        "",
        "",
        "",
        0,
        ""
    ],
    [
        -1,
        "",
        "",
        "",
        0,
        ""
    ],
    [],
    [],
    [],
    [],
    [],
    [],
    []
]
```
