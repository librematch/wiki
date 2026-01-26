# Information

The proxy forwards our requests and takes over authentication.

For the authenticated endpoints we should keep in mind:

- use a separate Steam account (or maybe even this Xbox stuff with a subscription for all 4 games for that (cheaper?))
- generally limit our access to the auth endpoints to a minimum (only what is really needed)

1. even rate-limit our requests

- mimic in-game requests as close as possible

We will need a running instance of a Steam Client for each game. To circumvent limitations (as only holding one login to steam per account on a certain moment in time is needed) we use a proxy to forward our requests on behalf of a certain session.

*Usage*

Base URL: **https://rlink.api.tools.uber.space/relic**

You need to get an *API_KEY* for the proxy from the team members.

Then you can make calls to the proxy e.g. for endpoint `/game/news/getNews` call:

```
https://proxy.api.tools.uber.space/relic/game/news/getNews
```

You need to supply a header with the *API_KEY* e.g. `API_KEY=...`

All query parameters that you add to the request will be forwarded to the Relic Link API on your behalf.

##### Insomnia

[Insomnia](https://insomnia.rest/) is a API design platform.

We have created some to use with their client.
