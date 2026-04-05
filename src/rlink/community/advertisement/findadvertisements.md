# [GET] /community/advertisement/findAdvertisements

[Example request](https://aoe-api.worldsedgelink.com/community/advertisement/findAdvertisements?title=age2)

Returns a list of currently advertised (open/waiting) matches
for the specified title, along with avatar information for
the players in those matches.

## Request

| Parameter | Type     | Value                  | Comments |
| --------- | -------- | ---------------------- | -------- |
| title     | str/enum | age1, age2, age3, age4 |          |

## Response

### AoE2:DE

The response contains a `matches` array with active lobbies
and an `avatars` array with player profile information for
all participants.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "matches": [
        {
            "id": 186581479,
            "steamlobbyid": 109775243596890080,
            "xboxsessionid": "0",
            "host_profile_id": 8863869,
            "state": 0,
            "description": "[Rematch] ",
            "visible": 1,
            "mapname": "my map",
            "options": "eNo9Us1ugzAMfpc+AYESaYce...",
            "passwordprotected": 0,
            "maxplayers": 8,
            "slotinfo": "eNrVkF1PwjAUhv0tvR6GMjYn...",
            "matchtype_id": 0,
            "matchmembers": [
                {
                    "match_id": 186581479,
                    "profile_id": 8863869,
                    "ranking": -1,
                    "statgroup_id": 5331726,
                    "race_id": -1,
                    "teamid": -1
                }
            ],
            "observernum": 0,
            "observermax": 512,
            "isobservable": 1,
            "observerdelay": 120,
            "hasobserverpassword": 1,
            "servicetype": 0,
            "relayserver_region": "westeurope"
        }
    ],
    "avatars": [
        {
            "profile_id": 8863869,
            "name": "/steam/76561198025231211",
            "alias": "PlayerName",
            "personal_statgroup_id": 5331726,
            "xp": 483,
            "level": 1,
            "leaderboardregion_id": 0,
            "country": "gb"
        }
    ]
}
```

#### Match fields

| Field               | Type   | Description                                                    |
| ------------------- | ------ | -------------------------------------------------------------- |
| id                  | int    | Unique match/lobby identifier                                  |
| steamlobbyid        | int    | Steam lobby ID for the match                                   |
| xboxsessionid       | string | Xbox session ID (`"0"` when not applicable)                    |
| host_profile_id     | int    | Profile ID of the lobby host                                   |
| state               | int    | Match state (`0` = waiting/open)                               |
| description         | string | Lobby name set by the host                                     |
| visible             | int    | Whether the lobby is publicly visible                          |
| mapname             | string | Map name for the match                                         |
| options             | string | Encoded match options (see note below)                         |
| passwordprotected   | int    | Whether a password is required to join (`0` = no, `1` = yes)   |
| maxplayers          | int    | Maximum number of player slots                                 |
| slotinfo            | string | Encoded slot configuration (see note below)                    |
| matchtype_id        | int    | Match type identifier                                          |
| matchmembers        | array  | List of players currently in the lobby                         |
| observernum         | int    | Current number of observers                                    |
| observermax         | int    | Maximum number of observers allowed                            |
| isobservable        | int    | Whether observers can join (`0` = no, `1` = yes)               |
| observerdelay       | int    | Observer delay in seconds                                      |
| hasobserverpassword | int    | Whether observers need a password (`0` = no, `1` = yes)        |
| servicetype         | int    | Service type identifier                                        |
| relayserver_region  | string | Azure region of the relay server (e.g. `westeurope`, `eastus`) |

#### Matchmember fields

| Field        | Type | Description                                          |
| ------------ | ---- | ---------------------------------------------------- |
| match_id     | int  | ID of the match this member belongs to               |
| profile_id   | int  | Player's profile ID                                  |
| ranking      | int  | Player's ranking (`-1` if unranked)                  |
| statgroup_id | int  | Player's stat group ID                               |
| race_id      | int  | Chosen civilization/race (`-1` if random or not set) |
| teamid       | int  | Team assignment (`-1` if not assigned)               |

#### Avatar fields

| Field                 | Type   | Description                                    |
| --------------------- | ------ | ---------------------------------------------- |
| profile_id            | int    | Player's profile ID                            |
| name                  | string | Platform identifier (e.g. `/steam/<steam_id>`) |
| alias                 | string | Player's display name                          |
| personal_statgroup_id | int    | Player's personal stat group ID                |
| xp                    | int    | Experience points                              |
| level                 | int    | Player level                                   |
| leaderboardregion_id  | int    | Leaderboard region identifier                  |
| country               | string | Two-letter country code                        |

> **Note:** The `options` and `slotinfo` fields may be
> zlib-compressed. Also check if there is a Base64 encoding
> on it -- sometimes it is even **two times** Base64
> encoded.
