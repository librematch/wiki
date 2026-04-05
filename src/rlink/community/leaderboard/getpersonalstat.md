# [GET] /community/leaderboard/GetPersonalStat

[Example request](https://aoe-api.worldsedgelink.com/community/leaderboard/GetPersonalStat?title=age2&profile_names=[%22/steam/76561197984749679%22])

Returns a player's profile information and their ranking statistics
across all leaderboards they have participated in.

## Request

| parameter     | type       | value                      | comments |
| ------------- | ---------- | -------------------------- | -------- |
| title         | str/enum   | age1, age2, age3, age4     |          |
| profile_names | array[str] | e.g. ["/steam/<steam_id>"] |          |
| aliases       | array[str] | [BlackRock]                |          |

## Response

### AoE2:DE

The response pairs `statGroups` (player profile) with
`leaderboardStats` (one entry per leaderboard the player has
played on).

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "statGroups": [
        {
            "id": 200,
            "name": "",
            "type": 1,
            "members": [
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
    ],
    "leaderboardStats": [
        {
            "statgroup_id": 200,
            "leaderboard_id": 3,
            "wins": 910,
            "losses": 477,
            "streak": 5,
            "disputes": 0,
            "drops": 4,
            "rank": 3,
            "ranktotal": 39023,
            "ranklevel": 1,
            "rating": 2602,
            "regionrank": 3,
            "regionranktotal": 15933,
            "lastmatchdate": 1664555924
        },
        {
            "statgroup_id": 200,
            "leaderboard_id": 4,
            "wins": 119,
            "losses": 35,
            "streak": -1,
            "disputes": 0,
            "drops": 10,
            "rank": -1,
            "ranktotal": 62599,
            "ranklevel": 0,
            "rating": 1443,
            "regionrank": -1,
            "regionranktotal": 25154,
            "lastmatchdate": 1661468788
        }
        // ... one entry per leaderboard the player has participated in
    ]
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
| statgroup_id    | int  | References the `statGroups` entry by `id`                    |
| leaderboard_id  | int  | Leaderboard this stat belongs to                             |
| wins            | int  | Total wins                                                   |
| losses          | int  | Total losses                                                 |
| streak          | int  | Current win/loss streak (positive = wins, negative = losses) |
| disputes        | int  | Number of disputed matches                                   |
| drops           | int  | Number of disconnects                                        |
| rank            | int  | Current rank position (`-1` = unranked)                      |
| ranktotal       | int  | Total number of ranked players on this leaderboard           |
| ranklevel       | int  | Rank tier/level (`0` = unranked, `1` = ranked)               |
| rating          | int  | Elo rating                                                   |
| regionrank      | int  | Rank within the player's region (`-1` = unranked)            |
| regionranktotal | int  | Total ranked players in the region (`-1` = unavailable)      |
| lastmatchdate   | int  | Unix timestamp of the last match played                      |
