# [GET] /community/external/proxysteamuserrequest

[Example request](https://aoe-api.worldsedgelink.com/community/external/proxysteamuserrequest?title=age2&profileNames=%5B%22%2Fsteam%2F76561197984749679%22%5D&request=%2FISteamUser%2FGetPlayerSummaries%2Fv0002%2F)

## Request

| parameter     | type       | value                                        | comments |
| ------------- | ---------- | -------------------------------------------- | -------- |
| profile_names | array[str] | e.g. ["/steam/<steam_id>"]                   |          |
| request       | str        | e.g. "/ISteamUser/GetPlayerSummaries/v0002/" |          |

## Response

### AoE2:DE

```
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
          "loccountrycode": "DE"           // country
        }
      ]
    }
  }
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
        "avatars": {
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
        },
        "steamResults": {
            "type": "object",
            "properties": {
                "response": {
                    "type": "object",
                    "properties": {
                        "players": {
                            "type": "array",
                            "items": {
                                "type": "object",
                                "properties": {
                                    "steamid": {
                                        "type": "string"
                                    },
                                    "communityvisibilitystate": {
                                        "type": "integer"
                                    },
                                    "profilestate": {
                                        "type": "integer"
                                    },
                                    "personaname": {
                                        "type": "string"
                                    },
                                    "commentpermission": {
                                        "type": "integer"
                                    },
                                    "profileurl": {
                                        "type": "string"
                                    },
                                    "avatar": {
                                        "type": "string"
                                    },
                                    "avatarmedium": {
                                        "type": "string"
                                    },
                                    "avatarfull": {
                                        "type": "string"
                                    },
                                    "avatarhash": {
                                        "type": "string"
                                    },
                                    "personastate": {
                                        "type": "integer"
                                    },
                                    "realname": {
                                        "type": "string"
                                    },
                                    "primaryclanid": {
                                        "type": "string"
                                    },
                                    "timecreated": {
                                        "type": "integer"
                                    },
                                    "personastateflags": {
                                        "type": "integer"
                                    },
                                    "loccountrycode": {
                                        "type": "string"
                                    }
                                },
                                "required": [
                                    "avatar",
                                    "avatarfull",
                                    "avatarhash",
                                    "avatarmedium",
                                    "commentpermission",
                                    "communityvisibilitystate",
                                    "loccountrycode",
                                    "personaname",
                                    "personastate",
                                    "personastateflags",
                                    "primaryclanid",
                                    "profilestate",
                                    "profileurl",
                                    "realname",
                                    "steamid",
                                    "timecreated"
                                ]
                            }
                        }
                    },
                    "required": [
                        "players"
                    ]
                }
            },
            "required": [
                "response"
            ]
        }
    },
    "required": [
        "avatars",
        "result",
        "steamResults"
    ]
}
```
