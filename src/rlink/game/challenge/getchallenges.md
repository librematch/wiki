# [GET] /game/Challenge/getChallenges

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/Challenge/getChallenges?callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz&signature=sss HTTP/1.1
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
{
    "result": 0,
    "dataSignature": "Q8jVpeRaWqNAyXwg7I/+4elO6TtyZGGRFkgOzBdiuh+h3CTgIHvCODfZZ95GFMSSpkBOwAgW/rx0EOiPXLn1BKyQW1qjmLIJFkCAfy06JoxPGpRXoo6WxRyLhe3xg6YrIm4AVa2sxeAkA9mNfFfFr+feiSNZ/6HBp621flD+f2Y+zHPd3ClPcQGiEvQXy6CCzsfqifr15+zTXZKsrrCmKgnrWQpefBxcaQipsZy063tHmH1DVbq05nC+iiecZJjhe70Pn+hzTBli6AOhAvFjrU7/95JFyWuHsfHu9GjWWAz5XNppOaPs5qChhm4bqr/4hd6pmnD9h4htIDDctdiAJw=="
}
```

## AoE4

### Request

```
GET /game/Challenge/getChallenges?callNum=170&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=1984780&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&signature=IrzFNAXOGFbB0WP3tc21BGDe8Br%2B1hZdG7L%2BONL8HourY0aIjyqbV%2FyrS7Dc6N%2BBqumlqrGFbJl9DDLJ6fdY8rcXNb%2BWQYep6als79ipXFgtS%2FFsy6Ewq6%2F31dfiloQzjdnGCljC%2ByaL%2BbtUL93e62AFOtihFfxD%2F6qcMLtZm4isuEHdUGcCn7MCyB409plnV6Qk5UitKHfx8OLAGBm0%2BF8%2BB6vtJTk0IrfwMWZQwzpx1uULTnLoLyJm6OPirHVqe8qi5Y29ZAw8bUZCdug8F2lX3ltuMFTnmVSSJBEV2WT8dssNiuTPdbTpZ30b6vv8SUAKaumVk4GsxcZHqsWPAA%3D%3D HTTP/1.1
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
[
    0, // result status code
    [],
    [],
    "IrzFNAXOGFbB0WP3tc21BGDe8Br+1hZdG7L+ONL8HourY0aIjyqbV/yrS7Dc6N+BqumlqrGFbJl9DDLJ6fdY8rcXNb+WQYep6als79ipXFgtS/Fsy6Ewq6/31dfiloQzjdnGCljC+yaL+btUL93e62AFOtihFfxD/6qcMLtZm4isuEHdUGcCn7MCyB409plnV6Qk5UitKHfx8OLAGBm0+F8+B6vtJTk0IrfwMWZQwzpx1uULTnLoLyJm6OPirHVqe8qi5Y29ZAw8bUZCdug8F2lX3ltuMFTnmVSSJBEV2WT8dssNiuTPdbTpZ30b6vv8SUAKaumVk4GsxcZHqsWPAA=="
]
```
