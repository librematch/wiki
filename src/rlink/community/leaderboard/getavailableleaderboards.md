# [GET] /community/leaderboard/GetAvailableLeaderboards (Definitions, Translations)

[Example request](https://aoe-api.worldsedgelink.com/community/leaderboard/GetAvailableLeaderboards?title=age2)

## Request

| parameter | type     | value                  | comments |
| --------- | -------- | ---------------------- | -------- |
| title     | str/enum | age1, age2, age3, age4 |          |

## Response

### AoE2:DE

```
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
    },
    {
      "id": 4,
      "name": "TEAM_RM_RANKED",
      "isranked": 1,
      "leaderboardmap": [
        {
          "matchtype_id": 7,
          "statgroup_type": 1,
          "race_id": -1
        },
        {
          "matchtype_id": 8,
          "statgroup_type": 1,
          "race_id": -1
        },
        {
          "matchtype_id": 9,
          "statgroup_type": 1,
          "race_id": -1
        }
      ]
    },
    {
      "id": 5,
      "name": "SOLO_BR_RANKED",
      "isranked": 1,
      "leaderboardmap": [
        {
          "matchtype_id": 10,
          "statgroup_type": 1,
          "race_id": -1
        }
      ]
    },
    {
      "id": 13,
      "name": "SOLO_EW_RANKED",
      "isranked": 1,
      "leaderboardmap": [
        {
          "matchtype_id": 26,
          "statgroup_type": 1,
          "race_id": -1
        }
      ]
    },
    {
      "id": 14,
      "name": "TEAM_EW_RANKED",
      "isranked": 1,
      "leaderboardmap": [
        {
          "matchtype_id": 27,
          "statgroup_type": 1,
          "race_id": -1
        },
        {
          "matchtype_id": 28,
          "statgroup_type": 1,
          "race_id": -1
        },
        {
          "matchtype_id": 29,
          "statgroup_type": 1,
          "race_id": -1
        }
      ]
    }
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
    },
    {
      "id": 5,
      "name": "4V4",
      "locstringid": -1
    },
    {
      "id": 6,
      "name": "1V1",
      "locstringid": -1
    },
    {
      "id": 7,
      "name": "2V2",
      "locstringid": -1
    },
    {
      "id": 8,
      "name": "3V3",
      "locstringid": -1
    },
    {
      "id": 9,
      "name": "4V4",
      "locstringid": -1
    },
    {
      "id": 10,
      "name": "FFA",
      "locstringid": -1
    },
    {
      "id": 26,
      "name": "1V1",
      "locstringid": -1
    },
    {
      "id": 27,
      "name": "2V2",
      "locstringid": -1
    },
    {
      "id": 28,
      "name": "3V3",
      "locstringid": -1
    },
    {
      "id": 29,
      "name": "4V4",
      "locstringid": -1
    },
    {
      "id": 60,
      "name": "CUSTOM_DM_1v1",
      "locstringid": -1
    },
    {
      "id": 61,
      "name": "CUSTOM_DM_TEAM",
      "locstringid": -1
    }
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
    },
    {
      "id": 3,
      "name": "Bulgarians",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 4,
      "name": "Burmese",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 5,
      "name": "Byzantines",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 6,
      "name": "Celts",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 7,
      "name": "Chinese",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 8,
      "name": "Cumans",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 9,
      "name": "Ethiopians",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 10,
      "name": "Franks",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 11,
      "name": "Goths",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 12,
      "name": "Huns",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 13,
      "name": "Incas",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 14,
      "name": "Hindustanis",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 15,
      "name": "Italians",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 16,
      "name": "Japanese",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 17,
      "name": "Khmer",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 18,
      "name": "Koreans",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 19,
      "name": "Lithuanians",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 20,
      "name": "Magyars",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 21,
      "name": "Malay",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 22,
      "name": "Malians",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 23,
      "name": "Mayans",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 24,
      "name": "Mongols",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 25,
      "name": "Persians",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 26,
      "name": "Portuguese",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 27,
      "name": "Saracens",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 28,
      "name": "Slavs",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 29,
      "name": "Spanish",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 30,
      "name": "Tatars",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 31,
      "name": "Teutons",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 32,
      "name": "Turks",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 33,
      "name": "Vietnamese",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 34,
      "name": "Vikings",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 35,
      "name": "Burgundians",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 36,
      "name": "Sicilians",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 37,
      "name": "Poles",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 38,
      "name": "Bohemians",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 39,
      "name": "Bengalis",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 40,
      "name": "Dravidians",
      "faction_id": 0,
      "locstringid": -1
    },
    {
      "id": 41,
      "name": "Gurjaras",
      "faction_id": 0,
      "locstringid": -1
    }
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

```
{
    "$schema": "http://json-schema.org/schema#",
    "type": "object",
    "properties": {
        "result": {
            "type": "object",
            "properties": {
                "code": {
                    "type": "integer"
                },
                "message": {
                    "type": "string"
                }
            },
            "required": [
                "code",
                "message"
            ]
        },
        "leaderboards": {
            "type": "array",
            "items": {
                "type": "object",
                "properties": {
                    "id": {
                        "type": "integer"
                    },
                    "name": {
                        "type": "string"
                    },
                    "isranked": {
                        "type": "integer"
                    },
                    "leaderboardmap": {
                        "type": "array",
                        "items": {
                            "type": "object",
                            "properties": {
                                "matchtype_id": {
                                    "type": "integer"
                                },
                                "statgroup_type": {
                                    "type": "integer"
                                },
                                "race_id": {
                                    "type": "integer"
                                }
                            },
                            "required": [
                                "matchtype_id",
                                "race_id",
                                "statgroup_type"
                            ]
                        }
                    }
                },
                "required": [
                    "id",
                    "isranked",
                    "leaderboardmap",
                    "name"
                ]
            }
        },
        "matchTypes": {
            "type": "array",
            "items": {
                "type": "object",
                "properties": {
                    "id": {
                        "type": "integer"
                    },
                    "name": {
                        "type": "string"
                    },
                    "locstringid": {
                        "type": "integer"
                    }
                },
                "required": [
                    "id",
                    "locstringid",
                    "name"
                ]
            }
        },
        "races": {
            "type": "array",
            "items": {
                "type": "object",
                "properties": {
                    "id": {
                        "type": "integer"
                    },
                    "name": {
                        "type": "string"
                    },
                    "faction_id": {
                        "type": "integer"
                    },
                    "locstringid": {
                        "type": "integer"
                    }
                },
                "required": [
                    "faction_id",
                    "id",
                    "locstringid",
                    "name"
                ]
            }
        },
        "factions": {
            "type": "array"
        },
        "leaderboardRegions": {
            "type": "array",
            "items": {
                "type": "object",
                "properties": {
                    "id": {
                        "type": "integer"
                    },
                    "name": {
                        "type": "string"
                    },
                    "locstringid": {
                        "type": "integer"
                    }
                },
                "required": [
                    "id",
                    "locstringid",
                    "name"
                ]
            }
        }
    },
    "required": [
        "factions",
        "leaderboardRegions",
        "leaderboards",
        "matchTypes",
        "races",
        "result"
    ]
}
```
