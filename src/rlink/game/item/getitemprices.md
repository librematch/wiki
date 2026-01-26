# [GET] /game/item/getItemPrices

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/item/getItemPrices?accountType=3&callNum=123&connect_id=ccc&country=us&currency=usd&lastCallTime=111&saleVersion=-1&sessionID=zzz HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type               | value | comments |
| ------------ | ------------------ | ----- | -------- |
| accountType  | int                | 3     |          |
| callNum      | int                | 123   |          |
| connect_id   |                    |       |          |
| lastCallTime | timestamp          |       |          |
| sessionID    | str                |       |          |
| country      | ISO 3166-1 Alpha-2 | us    |          |
| currency     | ISO 4217           | usd   |          |
| saleVersion  | int                | -1    |          |

### Response

```
RESPONSE_TEMPLATE
```

## AoE4

### Request

```
GET /game/item/getItemPrices?accountType=3&callNum=119&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&country=de&currency=eur&lastCallTime=653353&saleVersion=-1&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type               | value | comments |
| ------------ | ------------------ | ----- | -------- |
| accountType  | int                | 3     |          |
| callNum      | int                | 123   |          |
| connect_id   |                    |       |          |
| lastCallTime | timestamp          |       |          |
| country      | ISO 3166-1 Alpha-2 | us    |          |
| currency     | ISO 4217           | usd   |          |
| saleVersion  | int                | -1    |          |
| sessionID    | str                |       |          |

### Response

```
[
    0, // result status code
    [],
    0,
    []
]
```
