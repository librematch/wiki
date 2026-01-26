# /textmoderation

## Request

```
POST /textmoderation HTTP/1.1
Host: api.ageofempires.com
Accept-Encoding: identity
Accept:: application/json
Authorization: Steam1.0 CAEQ/ZzT4AsYBSBXKoABmNR5nKEvxOZpR3jXLBTeWT+SQfBPWnM786lvM3NsQNLaQvIGgur5Ub9nLriapKcxJpikWBq+svb22WVYeAhISj0ZwgVodLjNFeZmIA3aQFWywiPaKC53vC3bXYTg7nSIVc92Fet34xPSkIqf7asqoFbbw4Y80arguEAnOn4AvUI=
Content-Type: application/json
Content-Length: 124

{
   "conversationId":"0",
   "includeResponse":true,
   "language":"en-US",
   "textContent":"Test's Game",
   "textType":"SanitisationInput"
}
```

## Response

### AoE2:DE

```
{
   "filterResult":"Allow",
   "familyFriendlyResult":"Allow",
   "mediumResult":"Allow",
   "matureResult":"Allow",
   "maturePlusResult":"Allow",
   "moderatedText":"Test\u0027s Game"
}
```
