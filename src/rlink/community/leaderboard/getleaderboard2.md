# [GET] /community/leaderboard/getLeaderBoard2

[Example request](https://aoe-api.worldsedgelink.com/community/leaderboard/getLeaderBoard2?leaderboard_id=3&platform=PC_STEAM&title=age2&sortBy=1&start=1&count=200)

Returns a paginated slice of a leaderboard, including player profile
information and ranking statistics.

## Request

| parameter      | type     | value                  | comments                                            |
| -------------- | -------- | ---------------------- | --------------------------------------------------- |
| leaderboard_id | int      | 3                      | Leaderboard to query (see GetAvailableLeaderboards) |
| platform       | str/enum | PC_STEAM               | Platform filter                                     |
| title          | str/enum | age1, age2, age3, age4 | Game title                                          |
| sortBy         | int      | 1                      | `0` = sort by wins, `1` = sort by rating            |
| start          | int      | 1                      | Starting rank position (1-based)                    |
| count          | int      | 200                    | Number of entries to return                         |

## Response

### AoE2:DE

The response pairs `statGroups` (player profiles) with
`leaderboardStats` (ranking data). Each stat group entry
corresponds to a leaderboard stat entry via `statgroup_id`.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "statGroups": [
        {
            "id": 4120710,
            "name": "",
            "type": 1,
            "members": [
                {
                    "profile_id": 5123311,
                    "name": "/steam/76561199142950174",
                    "alias": "[MoA]Beicola",
                    "personal_statgroup_id": 4120710,
                    "xp": 407,
                    "level": 1,
                    "leaderboardregion_id": 4,
                    "country": "br"
                }
            ]
        },
        {
            "id": 6153140,
            "name": "",
            "type": 1,
            "members": [
                {
                    "profile_id": 10960083,
                    "name": "/steam/76561199385029768",
                    "alias": "Moonlight",
                    "personal_statgroup_id": 6153140,
                    "xp": 235,
                    "level": 1,
                    "leaderboardregion_id": 0,
                    "country": "it"
                }
            ]
        }
        // ... additional stat groups
    ],
    "leaderboardStats": [
        {
            "statgroup_id": 527797,
            "leaderboard_id": 3,
            "wins": 1427,
            "losses": 851,
            "streak": 2,
            "disputes": 0,
            "drops": 10,
            "rank": 1,
            "ranktotal": 39023,
            "ranklevel": 1,
            "rating": 2646,
            "regionrank": -1,
            "regionranktotal": -1,
            "lastmatchdate": 1666299350
        },
        {
            "statgroup_id": 1492,
            "leaderboard_id": 3,
            "wins": 1696,
            "losses": 873,
            "streak": 3,
            "disputes": 0,
            "drops": 10,
            "rank": 2,
            "ranktotal": 39023,
            "ranklevel": 1,
            "rating": 2617,
            "regionrank": -1,
            "regionranktotal": -1,
            "lastmatchdate": 1666113105
        }
        // ... additional leaderboard stats
    ],
    "rankTotal": 39023
}
```

#### `statGroups[].members[]` fields

| field                 | type   | description                                           |
| --------------------- | ------ | ----------------------------------------------------- |
| profile_id            | int    | Unique player profile identifier                      |
| name                  | string | Platform-specific identity (e.g. `/steam/<steam_id>`) |
| alias                 | string | Player display name                                   |
| personal_statgroup_id | int    | The player's personal stat group ID                   |
| xp                    | int    | Experience points                                     |
| level                 | int    | Player level                                          |
| leaderboardregion_id  | int    | Region ID (see GetAvailableLeaderboards)              |
| country               | string | ISO 3166-1 alpha-2 country code                       |

#### `leaderboardStats[]` fields

| field           | type | description                                                  |
| --------------- | ---- | ------------------------------------------------------------ |
| statgroup_id    | int  | References a `statGroups` entry by `id`                      |
| leaderboard_id  | int  | Leaderboard this stat belongs to                             |
| wins            | int  | Total wins                                                   |
| losses          | int  | Total losses                                                 |
| streak          | int  | Current win/loss streak (positive = wins, negative = losses) |
| disputes        | int  | Number of disputed matches                                   |
| drops           | int  | Number of disconnects                                        |
| rank            | int  | Current rank position (`-1` = unranked)                      |
| ranktotal       | int  | Total number of ranked players on this leaderboard           |
| ranklevel       | int  | Rank tier/level                                              |
| rating          | int  | Elo rating                                                   |
| regionrank      | int  | Rank within the player's region (`-1` = unranked)            |
| regionranktotal | int  | Total ranked players in the region (`-1` = unavailable)      |
| lastmatchdate   | int  | Unix timestamp of the last match played                      |

> **Note:** The `rankTotal` top-level field reflects the total
> number of ranked players on the queried leaderboard.
