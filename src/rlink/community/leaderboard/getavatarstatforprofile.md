# [GET] /community/leaderboard/GetAvatarStatForProfile

[Example request](https://aoe-api.worldsedgelink.com/community/leaderboard/GetAvatarStatForProfile?title=age2&profile_names=[%22/steam/76561197984749679%22])

Returns avatar stat values for one or more player profiles. Avatar
stats track various in-game statistics and achievement progress
used for avatar/icon unlocks.

## Request

| parameter     | type       | value                      | comments |
| ------------- | ---------- | -------------------------- | -------- |
| title         | str/enum   | age1, age2, age3, age4     |          |
| profile_names | array[str] | e.g. ["/steam/<steam_id>"] |          |

## Response

### AoE2:DE

Each entry in `avatarStatsForProfile` represents one tracked
statistic for the requested player. A typical response contains
100+ entries covering all stat IDs the player has recorded
values for.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "avatarStatsForProfile": [
        {
            "profile_id": 196240,
            "avatarstat_id": 1,
            "value": 1845,
            "lastupdated": 1664821730
        },
        {
            "profile_id": 196240,
            "avatarstat_id": 2,
            "value": 2257,
            "lastupdated": 1664824306
        },
        {
            "profile_id": 196240,
            "avatarstat_id": 3,
            "value": 102,
            "lastupdated": 1664543322
        }
        // ... typically 100+ entries per profile
    ]
}
```

#### `avatarStatsForProfile[]` fields

| field         | type | description                                                        |
| ------------- | ---- | ------------------------------------------------------------------ |
| profile_id    | int  | Player profile identifier                                          |
| avatarstat_id | int  | Game-internal stat tracking ID (determines which stat is recorded) |
| value         | int  | Current accumulated value for this stat                            |
| lastupdated   | int  | Unix timestamp of the last time this stat was updated              |

> **Note:** The `avatarstat_id` values correspond to game-internal
> stat tracking IDs. Low IDs (1-37) typically map to per-civilization
> win counts, while higher ranges cover cumulative stats like total
> kills, resources gathered, and event/challenge completions.
