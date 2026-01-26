# [GET] /game/item/getLevelRewardsTableJson

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/item/getLevelRewardsTableJson?callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz&signature=sss HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| callNum      | int       | 123   |          |
| connect_id   |           |       |          |
| lastCallTime | timestamp |       |          |
| sessionID    | str       |       |          |
| signature    | str       |       |          |

### Response

```
RESPONSE_TEMPLATE
```

## AoE4

### Request

```
GET /game/item/getLevelRewardsTableJson?callNum=216&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=2933258&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&signature=fXXM4SDq55MySPTT1KNG2I2l%2BjrHSKlXuakKPXfxrRowBDmE6zNji4qI9GkjciECpSrDrsPBMxuLij1iCapwM420bekwi8TQXimm%2BVHDU%2BkL02HiaKyHt5gdftJgYA2z0BwcpGozWtq21lGC%2FQo7%2BHD83F%2Bj1mgUQRFhXnVJRHwDFRT%2Bz5cvjxBU05SI0VTxZ7SOZl9LPK5TJ2YaC7KxEfjD7ZBkVzIbuhgD1rzTXEb%2Bav%2Bl3Q%2B3JXe9GBzSKWZ0VPDBrAhywanO1B0F%2Bq%2BkA1semppZC4fVeMONEoj8NrO%2FWZDkiZZwuVhx%2FHebF6iiBsUUlfeSqRJP2QyD%2Bg6Xwg%3D%3D HTTP/1.1
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
| lastCallTime | timestamp |       |          |
| sessionID    | str       |       |          |
| signature    | str       |       |          |

### Response

```
{
    "result": 0,
    "dataSignature": "fXXM4SDq55MySPTT1KNG2I2l+jrHSKlXuakKPXfxrRowBDmE6zNji4qI9GkjciECpSrDrsPBMxuLij1iCapwM420bekwi8TQXimm+VHDU+kL02HiaKyHt5gdftJgYA2z0BwcpGozWtq21lGC/Qo7+HD83F+j1mgUQRFhXnVJRHwDFRT+z5cvjxBU05SI0VTxZ7SOZl9LPK5TJ2YaC7KxEfjD7ZBkVzIbuhgD1rzTXEb+av+l3Q+3JXe9GBzSKWZ0VPDBrAhywanO1B0F+q+kA1semppZC4fVeMONEoj8NrO/WZDkiZZwuVhx/HebF6iiBsUUlfeSqRJP2QyD+g6Xwg=="
}
```
