# [POST] /game/item/signItems

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/item/signItems HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 127
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store

callNum=123&connect_id=ccc&crc=888&lastCallTime=111&sessionID=zzz
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| callNum      | int       | 123   |          |
| connect_id   |           |       |          |
| crc          | int       | 888   |          |
| lastCallTime | timestamp |       |          |
| sessionID    | str       |       |          |

### Response

```
[
    0, // result status code
    "kIZljYcuEnBkLRNBimBbsnUgCKNRVAim+ZhvQ6uyBnfIwjjXX2P9ZxWlExJEVePgzFzO9dNioZUkKOLjtyeWyfvTojyyxMAIZVP9jUKoB73U6aAsozt+JFbcztFhs6IRezW/lhqtkVrZQwYD3ex4y8suVZRnUouZUXo103b/jyqpha0YvlsWGuuqP/6GBthZU9qsJqHT+YbhAu40bDLvwq9fVksqbdaoBJOmc2dGPrSZFguFJSNmmLcOTQQkIZc/sBaSaTpNFk57zafVz4qe9HAGRxHdF1pfDDsIzEq2Glp65f3yrNFQDLZtshfgGItlIDFa/i6D+qw3TA5FfARgyw=="
]
```

## AoE4

### Request

```
POST /game/item/signItems HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 127
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache

callNum=34&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&crc=3611078805&lastCallTime=17363&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| callNum      | int       | 123   |          |
| connect_id   |           |       |          |
| crc          | int       | 888   |          |
| lastCallTime | timestamp |       |          |
| sessionID    | str       |       |          |

### Response

```
[
    0, // result status code
    "Gv20EHYdVJtMQMzFWmLCja2JdJpgV+/fsN31PYFG5mpYpmbCxihWLET0mAbBpLSFP3TOayG9943zTLtW1K/M95CPyVbQZsaFJOWgqN3310esgCeSirxNCfvM76g94BSeJDI5nD+TxGE0gF1diez2M5VU8PRYlHAyLrF2lHvvtwLXBu807AaaiA22nwShh11uA8MzL7LOI3aVIbSnLj16ywCLKnrEANQe8JTKttuMUFvF2f596hY+mZHxNIw2IjREHo2OgNt6vKvv9l6Jpi6beSXr3Dalhu6oj0oRotXkeCPUp08Q6P1knu3CwnwOtJPs7+PCEUIQUM1XR41mOq0Dgw=="
]
```
