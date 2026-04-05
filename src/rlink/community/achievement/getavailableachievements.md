# [GET] /community/achievement/getAvailableAchievements

[Example request](https://aoe-api.worldsedgelink.com/community/achievement/getAvailableAchievements?title=age2)

Retrieves the full list of available achievement definitions for
the specified title.

## Request

| parameter | type     | value                  | comments |
| --------- | -------- | ---------------------- | -------- |
| title     | str/enum | age1, age2, age3, age4 |          |

## Response

### AoE2:DE

The response contains an `achievementDefs` array with every
achievement definition registered for the title.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "achievementDefs": [
        {
            "id": 1,
            "name": "ACHIEVEMENT_ETERNAL_GRATITUDE",
            "name_locstringid": -1,
            "description_locstringid": -1,
            "icon": "",
            "timemodified": 1665011141,
            "deleted": 0,
            "itembundle_id": -1
        },
        {
            "id": 2,
            "name": "AZTEC_VICTORY",
            "name_locstringid": -1,
            "description_locstringid": -1,
            "icon": "",
            "timemodified": 1665011141,
            "deleted": 0,
            "itembundle_id": -1
        },
        {
            "id": 3,
            "name": "BERBERS_VICTORY",
            "name_locstringid": -1,
            "description_locstringid": -1,
            "icon": "",
            "timemodified": 1665011141,
            "deleted": 0,
            "itembundle_id": -1
        }
        // ... more achievement definitions
    ]
}
```

| field                   | type   | description                                 |
| ----------------------- | ------ | ------------------------------------------- |
| id                      | int    | Achievement definition ID                   |
| name                    | string | Internal achievement name                   |
| name_locstringid        | int    | Localization string ID for name (-1 = none) |
| description_locstringid | int    | Localization string ID for description      |
| icon                    | string | Icon asset reference                        |
| timemodified            | int    | Unix timestamp of last modification         |
| deleted                 | int    | Deletion flag (0 = active)                  |
| itembundle_id           | int    | Associated item bundle (-1 = none)          |
