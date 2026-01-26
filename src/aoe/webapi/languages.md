# /webapi/Languages (Missing parameters)

Parameters

[Example request](https://api.ageofempires.com/webapi/Languages?gameId=aoe)

## Request

```
GET /webapi/Languages?gameId=age1 HTTP/2
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
    "language": "English US",
    "utf8Language": "English"
  },
  {
    "language": "Spanish MX",
    "utf8Language": "Español Mexicano"
  },
  {
    "language": "Spanish ES",
    "utf8Language": "Español"
  },
  {
    "language": "Portuguese BR",
    "utf8Language": "Português Brasil"
  },
  {
    "language": "French",
    "utf8Language": "Français"
  },
  {
    "language": "German",
    "utf8Language": "Deutsch"
  },
  {
    "language": "Italian",
    "utf8Language": "Italiano"
  },
  {
    "language": "Hindi",
    "utf8Language": "हिंदी"
  },
  {
    "language": "Japanese",
    "utf8Language": "日本語"
  },
  {
    "language": "Korean",
    "utf8Language": "한국어"
  },
  {
    "language": "Russian",
    "utf8Language": "Русский"
  },
  {
    "language": "Vietnamese ",
    "utf8Language": "Tiếng Việt"
  },
  {
    "language": "Chinese Simplified",
    "utf8Language": "简体中文"
  },
  {
    "language": "Chinese Traditional",
    "utf8Language": "繁體中文"
  }
]
```
