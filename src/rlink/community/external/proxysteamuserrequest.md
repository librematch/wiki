# [GET] /community/external/proxysteamuserrequest

[Example request](https://aoe-api.worldsedgelink.com/community/external/proxysteamuserrequest?title=age2&profileNames=%5B%22%2Fsteam%2F76561197984749679%22%5D&request=%2FISteamUser%2FGetPlayerSummaries%2Fv0002%2F)

Proxies a request to the Steam Web API through the game server.
The `request` parameter specifies the Steam API path to call
(e.g. `/ISteamUser/GetPlayerSummaries/v0002/`). The response
includes both the game's avatar data and the raw Steam API
result.

## Request

| parameter     | type       | value                                        | comments                             |
| ------------- | ---------- | -------------------------------------------- | ------------------------------------ |
| title         | str/enum   | age1, age2, age3, age4                       | Game title                           |
| profile_names | array[str] | e.g. ["/steam/<steam_id>"]                   | Steam profile identifiers to look up |
| request       | str        | e.g. "/ISteamUser/GetPlayerSummaries/v0002/" | Steam Web API path to proxy          |

## Response

### AoE2:DE

Returns an `avatars` array with the game's player data and
a `steamResults` object containing the raw Steam API response.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "avatars": [
        {
            "profile_id": 209525,
            "name": "/steam/76561197995781128",
            "alias": "aoe2companion.com",
            "personal_statgroup_id": 2818,
            "xp": 416,
            "level": 1,
            "leaderboardregion_id": 0,
            "country": "de"
        }
    ],
    "steamResults": {
        "response": {
            "players": [
                {
                    "steamid": "76561197995781128",
                    "communityvisibilitystate": 3,
                    "profilestate": 1,
                    "personaname": "aoe2companion.com",
                    "commentpermission": 1,
                    "profileurl": "https://steamcommunity.com/profiles/76561197995781128/",
                    "avatar": "https://steamcdn-a.akamaihd.net/steamcommunity/public/images/avatars/15/15b212855bc63aa40651d31a5239a9285751cf56.jpg",
                    "avatarmedium": "https://steamcdn-a.akamaihd.net/steamcommunity/public/images/avatars/15/15b212855bc63aa40651d31a5239a9285751cf56_medium.jpg",
                    "avatarfull": "https://steamcdn-a.akamaihd.net/steamcommunity/public/images/avatars/15/15b212855bc63aa40651d31a5239a9285751cf56_full.jpg",
                    "avatarhash": "15b212855bc63aa40651d31a5239a9285751cf56",
                    "personastate": 0,
                    "realname": "Baal",
                    "primaryclanid": "103582791434874752",
                    "timecreated": 1200164646,
                    "personastateflags": 0,
                    "loccountrycode": "DE"
                }
            ]
        }
    }
}
```

#### Avatar fields

| field                 | type   | description                              |
| --------------------- | ------ | ---------------------------------------- |
| profile_id            | int    | Unique player profile identifier         |
| name                  | string | Platform identifier (e.g. `/steam/<id>`) |
| alias                 | string | Player display name                      |
| personal_statgroup_id | int    | Player's personal stat group identifier  |
| xp                    | int    | Experience points                        |
| level                 | int    | Player level                             |
| leaderboardregion_id  | int    | Leaderboard region identifier            |
| country               | string | Two-letter country code                  |

#### Steam player fields (`steamResults.response.players[]`)

| field                    | type   | description                                |
| ------------------------ | ------ | ------------------------------------------ |
| steamid                  | string | 64-bit Steam ID                            |
| communityvisibilitystate | int    | Profile visibility (`3` = public)          |
| profilestate             | int    | Profile configuration state                |
| personaname              | string | Steam display name                         |
| commentpermission        | int    | Whether comments are allowed (`0`/`1`)     |
| profileurl               | string | Full URL to the Steam profile              |
| avatar                   | string | URL to small avatar image (32x32)          |
| avatarmedium             | string | URL to medium avatar image (64x64)         |
| avatarfull               | string | URL to full avatar image (184x184)         |
| avatarhash               | string | Avatar image hash                          |
| personastate             | int    | Online status (`0` = offline)              |
| realname                 | string | Real name set on profile                   |
| primaryclanid            | string | Primary Steam group ID                     |
| timecreated              | int    | Unix timestamp of account creation         |
| personastateflags        | int    | Bitfield for persona state flags           |
| loccountrycode           | string | Two-letter country code from Steam profile |

> **Note:** The `request` parameter accepts any valid Steam Web
> API path. The game server adds its own Steam API key and
> forwards the request, so no client-side key is needed.
