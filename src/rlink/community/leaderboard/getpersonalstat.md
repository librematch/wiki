# [GET] /community/leaderboard/GetPersonalStat

[Example request](https://aoe-api.worldsedgelink.com/community/leaderboard/GetPersonalStat?title=age2&profile_names=[%22/steam/76561197984749679%22])

## Request

| parameter     | type       | value                      | comments |
| ------------- | ---------- | -------------------------- | -------- |
| title         | str/enum   | age1, age2, age3, age4     |          |
| profile_names | array[str] | e.g. ["/steam/<steam_id>"] |          |
| aliases       | array[str] | [BlackRock]                |          |

## Response

### AoE2:DE

```
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
    },
    {
      "statgroup_id": 200,
      "leaderboard_id": 1,
      "wins": 44,
      "losses": 13,
      "streak": 2,
      "disputes": 0,
      "drops": 0,
      "rank": -1,
      "ranktotal": 62,
      "ranklevel": 0,
      "rating": 2044,
      "regionrank": -1,
      "regionranktotal": 24,
      "lastmatchdate": 1620397322
    },
    {
      "statgroup_id": 200,
      "leaderboard_id": 2,
      "wins": 7,
      "losses": 2,
      "streak": 3,
      "disputes": 0,
      "drops": 0,
      "rank": -1,
      "ranktotal": -1,
      "ranklevel": -1,
      "rating": 2049,
      "regionrank": -1,
      "regionranktotal": -1,
      "lastmatchdate": 1591803253
    },
    {
      "statgroup_id": 200,
      "leaderboard_id": 13,
      "wins": 146,
      "losses": 63,
      "streak": -1,
      "disputes": 0,
      "drops": 0,
      "rank": 6,
      "ranktotal": 2662,
      "ranklevel": 1,
      "rating": 1925,
      "regionrank": 2,
      "regionranktotal": 1046,
      "lastmatchdate": 1664824305
    },
    {
      "statgroup_id": 200,
      "leaderboard_id": 14,
      "wins": 1,
      "losses": 0,
      "streak": 1,
      "disputes": 0,
      "drops": 1,
      "rank": -1,
      "ranktotal": -1,
      "ranklevel": -1,
      "rating": 1039,
      "regionrank": -1,
      "regionranktotal": -1,
      "lastmatchdate": 1656025212
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
        "statGroups": {
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
                    "type": {
                        "type": "integer"
                    },
                    "members": {
                        "type": "array",
                        "items": {
                            "type": "object",
                            "properties": {
                                "profile_id": {
                                    "type": "integer"
                                },
                                "name": {
                                    "type": "string"
                                },
                                "alias": {
                                    "type": "string"
                                },
                                "personal_statgroup_id": {
                                    "type": "integer"
                                },
                                "xp": {
                                    "type": "integer"
                                },
                                "level": {
                                    "type": "integer"
                                },
                                "leaderboardregion_id": {
                                    "type": "integer"
                                },
                                "country": {
                                    "type": "string"
                                }
                            },
                            "required": [
                                "alias",
                                "country",
                                "leaderboardregion_id",
                                "level",
                                "name",
                                "personal_statgroup_id",
                                "profile_id",
                                "xp"
                            ]
                        }
                    }
                },
                "required": [
                    "id",
                    "members",
                    "name",
                    "type"
                ]
            }
        },
        "leaderboardStats": {
            "type": "array",
            "items": {
                "type": "object",
                "properties": {
                    "statgroup_id": {
                        "type": "integer"
                    },
                    "leaderboard_id": {
                        "type": "integer"
                    },
                    "wins": {
                        "type": "integer"
                    },
                    "losses": {
                        "type": "integer"
                    },
                    "streak": {
                        "type": "integer"
                    },
                    "disputes": {
                        "type": "integer"
                    },
                    "drops": {
                        "type": "integer"
                    },
                    "rank": {
                        "type": "integer"
                    },
                    "ranktotal": {
                        "type": "integer"
                    },
                    "ranklevel": {
                        "type": "integer"
                    },
                    "rating": {
                        "type": "integer"
                    },
                    "regionrank": {
                        "type": "integer"
                    },
                    "regionranktotal": {
                        "type": "integer"
                    },
                    "lastmatchdate": {
                        "type": "integer"
                    }
                },
                "required": [
                    "disputes",
                    "drops",
                    "lastmatchdate",
                    "leaderboard_id",
                    "losses",
                    "rank",
                    "ranklevel",
                    "ranktotal",
                    "rating",
                    "regionrank",
                    "regionranktotal",
                    "statgroup_id",
                    "streak",
                    "wins"
                ]
            }
        }
    },
    "required": [
        "leaderboardStats",
        "result",
        "statGroups"
    ]
}
```
