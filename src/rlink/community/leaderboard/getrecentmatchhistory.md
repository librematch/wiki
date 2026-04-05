# [GET] /community/leaderboard/getRecentMatchHistory

[Example request](https://aoe-api.worldsedgelink.com/community/leaderboard/getRecentMatchHistory?title=age2&profile_names=[%22/steam/76561197984749679%22])

Returns the recent match history for one or more players.
You must provide at least one of `profile_names`,
`profile_ids`, or `aliases`.

## Request

| parameter     | type       | value                      | comments                     |
| ------------- | ---------- | -------------------------- | ---------------------------- |
| title         | str/enum   | age1, age2, age3, age4     | Game title                   |
| profile_names | array[str] | e.g. ["/steam/<steam_id>"] | Platform-prefixed player IDs |
| profile_ids   | array[int] | e.g. ["<relic_link_id>"]   | Relic link profile IDs       |
| aliases       | array[str] | e.g. [BlackRock]           | In-game display names        |

## Response

### AoE2:DE

The response contains a `matchHistoryStats` array of match
objects and a `profiles` array with player metadata. Each
match includes a `matchhistoryreportresults` array with
per-player results, and optionally `matchurls` with replay
download links.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "matchHistoryStats": [
        {
            "id": 183556359,
            "creator_profile_id": 199325,
            "mapname": "FrigidLake.rms",
            "maxplayers": 2,
            "matchtype_id": 26,
            "options": "eNpFUtFugzAM/Jd9waAQqY+p...",
            "slotinfo": "eNq9kFFPgzAUhf0tfa5mFDVh...",
            "description": "AUTOMATCH",
            "startgametime": 1664802149,
            "completiontime": 1664802709,
            "observertotal": 4,
            "matchhistoryreportresults": [
                {
                    "matchhistory_id": 183556359,
                    "profile_id": 199325,
                    "resulttype": 0,
                    "teamid": 0,
                    "race_id": 29,
                    "xpgained": 1,
                    "counters": "{}",
                    "matchstartdate": 1664802149
                },
                {
                    "matchhistory_id": 183556359,
                    "profile_id": 196240,
                    "resulttype": 1,
                    "teamid": 1,
                    "race_id": 12,
                    "xpgained": 1,
                    "counters": "{}",
                    "matchstartdate": 1664802149
                }
            ],
            "matchhistorymember": [
                {
                    "matchhistory_id": 183556359,
                    "profile_id": 199325,
                    "race_id": 29,
                    "statgroup_id": 12345,
                    "teamid": 0,
                    "wins": 10,
                    "losses": 5,
                    "streak": 2,
                    "arbitration": 0,
                    "outcome": 0,
                    "oldrating": 1200,
                    "newrating": 1190,
                    "reporttype": 0
                }
            ],
            "matchhistoryitems": [],
            "matchurls": []
        }
    ],
    "profiles": [
        {
            "profile_id": 196240,
            "name": "/steam/76561197984749679",
            "alias": "GL.TheViper",
            "personal_statgroup_id": 200,
            "xp": 3091,
            "level": 2,
            "leaderboardregion_id": 0,
            "country": "de"
        }
    ]
}
```

### Match object fields

| field                     | type   | description                                       |
| ------------------------- | ------ | ------------------------------------------------- |
| id                        | int    | Unique match ID                                   |
| creator_profile_id        | int    | Profile ID of the player who created the lobby    |
| mapname                   | string | Map filename (e.g. `FrigidLake.rms`)              |
| maxplayers                | int    | Maximum number of player slots                    |
| matchtype_id              | int    | Match type identifier (e.g. 26 = 1v1 ranked)      |
| options                   | string | Base64-encoded zlib-compressed match options      |
| slotinfo                  | string | Base64-encoded zlib-compressed slot configuration |
| description               | string | Lobby description (`AUTOMATCH` for ranked)        |
| startgametime             | int    | Match start time (Unix timestamp)                 |
| completiontime            | int    | Match end time (Unix timestamp)                   |
| observertotal             | int    | Number of observers in the match                  |
| matchhistoryreportresults | array  | Per-player result entries (see below)             |
| matchhistorymember        | array  | Per-player rating/ELO data (see below)            |
| matchhistoryitems         | array  | In-game items (typically empty)                   |
| matchurls                 | array  | Replay file download URLs (when available)        |

### `matchhistoryreportresults` entry fields

| field           | type   | description                                       |
| --------------- | ------ | ------------------------------------------------- |
| matchhistory_id | int    | Match ID (same as parent match `id`)              |
| profile_id      | int    | Player's profile ID                               |
| resulttype      | int    | `0` = loss, `1` = win                             |
| teamid          | int    | Team index (0-based)                              |
| race_id         | int    | Civilization ID (see reference tables)            |
| xpgained        | int    | Experience points gained from the match           |
| counters        | string | JSON string of in-game counters (often `"{}"`)    |
| matchstartdate  | int    | Match start time (Unix timestamp, same as parent) |

### `matchhistorymember` entry fields

| field           | type | description                          |
| --------------- | ---- | ------------------------------------ |
| matchhistory_id | int  | Match ID (same as parent match `id`) |
| profile_id      | int  | Player's profile ID                  |
| race_id         | int  | Civilization ID                      |
| statgroup_id    | int  | Player's stat group ID               |
| teamid          | int  | Team index (0-based)                 |
| wins            | int  | Player's total wins in this mode     |
| losses          | int  | Player's total losses in this mode   |
| streak          | int  | Current win/loss streak              |
| arbitration     | int  | Arbitration status                   |
| outcome         | int  | Match outcome for this player        |
| oldrating       | int  | ELO rating before the match          |
| newrating       | int  | ELO rating after the match           |
| reporttype      | int  | Type of result report                |

### `profiles` entry fields

| field                 | type   | description                                     |
| --------------------- | ------ | ----------------------------------------------- |
| profile_id            | int    | Player's profile ID                             |
| name                  | string | Platform-prefixed ID (e.g. `/steam/<steam_id>`) |
| alias                 | string | In-game display name                            |
| personal_statgroup_id | int    | Player's personal stat group ID                 |
| xp                    | int    | Total experience points                         |
| level                 | int    | Player level                                    |
| leaderboardregion_id  | int    | Region ID (`0` = Europe, `2` = Asia, etc.)      |
| country               | string | Two-letter country code                         |

> **Note:** The `options` and `slotinfo` fields contain
> base64-encoded, zlib-compressed data. Decode with base64
> then decompress with zlib to access the underlying
> configuration.
