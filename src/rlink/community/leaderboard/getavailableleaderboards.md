# [GET] /community/leaderboard/GetAvailableLeaderboards

[Example request](https://aoe-api.worldsedgelink.com/community/leaderboard/GetAvailableLeaderboards?title=age2)

Returns the available leaderboard definitions, match types, races
(civilizations), and leaderboard regions for a given title.

## Request

| parameter | type     | value                  | comments |
| --------- | -------- | ---------------------- | -------- |
| title     | str/enum | age1, age2, age3, age4 |          |

## Response

### AoE2:DE

The response contains lookup tables that map leaderboard IDs to their
match types, plus all known civilizations and regions.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "leaderboards": [
        {
            "id": 1,
            "name": "SOLO_DM_RANKED",
            "isranked": 1,
            "leaderboardmap": [
                {
                    "matchtype_id": 2,
                    "statgroup_type": 1,
                    "race_id": -1
                },
                {
                    "matchtype_id": 60,
                    "statgroup_type": 1,
                    "race_id": -1
                }
            ]
        },
        {
            "id": 2,
            "name": "TEAM_DM_RANKED",
            "isranked": 1,
            "leaderboardmap": [
                {
                    "matchtype_id": 3,
                    "statgroup_type": 1,
                    "race_id": -1
                },
                {
                    "matchtype_id": 4,
                    "statgroup_type": 1,
                    "race_id": -1
                },
                {
                    "matchtype_id": 5,
                    "statgroup_type": 1,
                    "race_id": -1
                },
                {
                    "matchtype_id": 61,
                    "statgroup_type": 1,
                    "race_id": -1
                }
            ]
        },
        {
            "id": 3,
            "name": "SOLO_RM_RANKED",
            "isranked": 1,
            "leaderboardmap": [
                {
                    "matchtype_id": 6,
                    "statgroup_type": 1,
                    "race_id": -1
                }
            ]
        }
        // ... additional leaderboards (ids 4, 5, 13, 14, etc.)
    ],
    "matchTypes": [
        {
            "id": 2,
            "name": "1V1",
            "locstringid": -1
        },
        {
            "id": 3,
            "name": "2V2",
            "locstringid": -1
        },
        {
            "id": 4,
            "name": "3V3",
            "locstringid": -1
        }
        // ... additional match types (4V4, FFA, CUSTOM_DM_*, etc.)
    ],
    "races": [
        {
            "id": 0,
            "name": "Aztec",
            "faction_id": 0,
            "locstringid": -1
        },
        {
            "id": 1,
            "name": "Berbers",
            "faction_id": 0,
            "locstringid": -1
        },
        {
            "id": 2,
            "name": "Britons",
            "faction_id": 0,
            "locstringid": -1
        }
        // ... additional civilizations (42 total in AoE2:DE)
    ],
    "factions": [],
    "leaderboardRegions": [
        {
            "id": 0,
            "name": "Europe",
            "locstringid": -1
        },
        {
            "id": 1,
            "name": "Middle East",
            "locstringid": -1
        },
        {
            "id": 2,
            "name": "Asia",
            "locstringid": -1
        },
        {
            "id": 3,
            "name": "North America",
            "locstringid": -1
        },
        {
            "id": 4,
            "name": "South America",
            "locstringid": -1
        },
        {
            "id": 5,
            "name": "Oceania",
            "locstringid": -1
        },
        {
            "id": 6,
            "name": "Africa",
            "locstringid": -1
        },
        {
            "id": 7,
            "name": "Unknown",
            "locstringid": -1
        }
    ]
}
```

#### `leaderboards[]` fields

| field                           | type   | description                                                          |
| ------------------------------- | ------ | -------------------------------------------------------------------- |
| id                              | int    | Unique leaderboard identifier                                        |
| name                            | string | Internal leaderboard name (e.g. `SOLO_RM_RANKED`)                    |
| isranked                        | int    | Whether the leaderboard is ranked (`1` = yes, `0` = no)              |
| leaderboardmap                  | array  | List of match type / stat group / race mappings for this leaderboard |
| leaderboardmap[].matchtype_id   | int    | References a `matchTypes` entry by `id`                              |
| leaderboardmap[].statgroup_type | int    | Stat group type (`1` = individual)                                   |
| leaderboardmap[].race_id        | int    | Race filter (`-1` = any race)                                        |

#### `matchTypes[]` fields

| field       | type   | description                                   |
| ----------- | ------ | --------------------------------------------- |
| id          | int    | Unique match type identifier                  |
| name        | string | Display name (e.g. `1V1`, `2V2`, `FFA`)       |
| locstringid | int    | Localization string ID (`-1` = not localized) |

#### `races[]` fields

| field       | type   | description                                   |
| ----------- | ------ | --------------------------------------------- |
| id          | int    | Unique civilization identifier                |
| name        | string | Civilization name (e.g. `Aztec`, `Britons`)   |
| faction_id  | int    | Faction grouping (`0` for all AoE2:DE civs)   |
| locstringid | int    | Localization string ID (`-1` = not localized) |

#### `leaderboardRegions[]` fields

| field       | type   | description                                   |
| ----------- | ------ | --------------------------------------------- |
| id          | int    | Unique region identifier                      |
| name        | string | Region name (e.g. `Europe`, `Asia`)           |
| locstringid | int    | Localization string ID (`-1` = not localized) |

> **Note:** The `factions` array is always empty for AoE2:DE.
