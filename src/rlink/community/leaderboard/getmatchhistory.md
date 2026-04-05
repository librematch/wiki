# [GET] /community/leaderboard/getMatchHistory

[Example request](https://aoe-api.worldsedgelink.com/community/leaderboard/getMatchHistory?matchIDs=[468097482]&title=age2)

Retrieves match details by match ID. More efficient than fetching
a player's full recent match history when you already know the
match ID(s).

## Request

| parameter | type       | value                  | comments               |
| --------- | ---------- | ---------------------- | ---------------------- |
| title     | str/enum   | age1, age2, age3, age4 |                        |
| matchIDs  | array[int] | e.g. [468097482]       | max batch size unknown |

## Response

### AoE2:DE

The response includes `matchHistory` (array of match objects),
and `profiles` (array of player profiles referenced in the
matches).

Each match object contains the same fields as in
[getRecentMatchHistory](./getrecentmatchhistory.md), plus
additional `matchhistorymember` entries with ELO rating changes
and a `gamemod_id` field.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "matchHistory": [
        {
            "id": 468097482,
            "creator_profile_id": 8793414,
            "mapname": "Arabia.rms",
            "maxplayers": 2,
            "matchtype_id": 6,
            "options": "...",
            "slotinfo": "...",
            "description": "AUTOMATCH",
            "startgametime": 1775375467,
            "completiontime": 1775377115,
            "observertotal": 8,
            "matchhistoryreportresults": [
                {
                    "matchhistory_id": 468097482,
                    "profile_id": 8793414,
                    "resulttype": 0,
                    "teamid": 0,
                    "civilization_id": 27,
                    "xpgained": 1,
                    "counters": "{}",
                    "matchstartdate": 1775375467
                },
                {
                    "matchhistory_id": 468097482,
                    "profile_id": 271202,
                    "resulttype": 1,
                    "teamid": 1,
                    "civilization_id": 59,
                    "xpgained": 1,
                    "counters": "{}",
                    "matchstartdate": 1775375467
                }
            ],
            "matchhistoryitems": [],
            "matchurls": [
                {
                    "profile_id": 8793414,
                    "url": "https://rl0aoelivemk2blob...",
                    "size": 788341,
                    "datatype": 0
                }
            ],
            "matchhistorymember": [
                {
                    "matchhistory_id": 468097482,
                    "profile_id": 8793414,
                    "civilization_id": 27,
                    "statgroup_id": 5316808,
                    "teamid": 0,
                    "wins": 4318,
                    "losses": 3429,
                    "streak": -3,
                    "arbitration": 1,
                    "outcome": 0,
                    "oldrating": 2728,
                    "newrating": 2720,
                    "reporttype": 1
                },
                {
                    "matchhistory_id": 468097482,
                    "profile_id": 271202,
                    "civilization_id": 59,
                    "statgroup_id": 80031,
                    "teamid": 1,
                    "wins": 1785,
                    "losses": 717,
                    "streak": 16,
                    "arbitration": 1,
                    "outcome": 1,
                    "oldrating": 2915,
                    "newrating": 2923,
                    "reporttype": 1
                }
            ],
            "gamemod_id": 1768
        }
    ],
    "profiles": [
        {
            "profile_id": 271202,
            "name": "/steam/76561198000635167",
            "alias": "Oni.Vinchester",
            "personal_statgroup_id": 80031,
            "xp": 10290,
            "level": 3,
            "leaderboardregion_id": 0,
            "country": "ru",
            "clanlist_name": ""
        },
        {
            "profile_id": 8793414,
            "name": "/steam/76561198136932885",
            "alias": "Oni.Lewis",
            "personal_statgroup_id": 5316808,
            "xp": 12017,
            "level": 4,
            "leaderboardregion_id": 0,
            "country": "gb",
            "clanlist_name": ""
        }
    ]
}
```

> **Note:** The top-level key is `matchHistory` (not
> `matchHistoryStats` as in `getRecentMatchHistory`). The
> `matchhistorymember` array includes ELO rating data
> (`oldrating`, `newrating`) and win/loss/streak stats.
