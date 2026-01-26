# /webapi/games

[Example request](https://api.ageofempires.com/webapi/Games)

## Request

```
GET /webapi/Games HTTP/2
Host: api.ageofempires.com
User-Agent: <UA>
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8
Accept-Language: en-GB,en;q=0.5
Accept-Encoding: gzip, deflate, br
DNT: 1
Connection: keep-alive
Cookie: MSCC=cid=l8flb3okwccch8klb744k8e2-c1=2-c2=2-c3=2
Upgrade-Insecure-Requests: 1
Sec-Fetch-Dest: document
Sec-Fetch-Mode: navigate
Sec-Fetch-Site: cross-site
Pragma: no-cache
Cache-Control: no-cache
TE: trailers
```

## Response

```
[
   {
      "gameTitleId":1,
      "gameTitleName":"Age of Empires DE",
      "gameVersion":"1.1.1"
   },
   {
      "gameTitleId":2,
      "gameTitleName":"Age of Empires II DE",
      "gameVersion":"1"
   },
   {
      "gameTitleId":3,
      "gameTitleName":"Age of Empires III DE",
      "gameVersion":"1"
   },
   {
      "gameTitleId":4,
      "gameTitleName":"Age of Empires IV",
      "gameVersion":"1"
   },
   {
      "gameTitleId":5,
      "gameTitleName":"Age of Mythology",
      "gameVersion":"1"
   }
]
```
