# [GET] /community/achievement/getAchievements

[Example request](https://aoe-api.worldsedgelink.com/community/achievement/getAchievements?title=age2&profileids=[196240])

Retrieves the list of achievements earned by one or more players,
identified by profile ID.

## Request

| parameter  | type     | value                  | comments |
| ---------- | -------- | ---------------------- | -------- |
| title      | str/enum | age1, age2, age3, age4 |          |
| profileids | arr[int] | [196240]               |          |

## Response

### AoE2:DE

The response contains a `userAchievementsMap` array. Each element
is an object keyed by the requested profile ID, whose value is an
array of achievement entries the player has earned.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "userAchievementsMap": [
        {
            "196240": [
                {
                    "achievement_id": 83,
                    "achieveddate": 1589903767
                },
                {
                    "achievement_id": 109,
                    "achieveddate": 1604004966
                },
                {
                    "achievement_id": 44,
                    "achieveddate": 1604333155
                }
                // ... more achievements
            ]
        }
    ]
}
```

| field          | type | description                  |
| -------------- | ---- | ---------------------------- |
| achievement_id | int  | Achievement definition ID    |
| achieveddate   | int  | Unix timestamp when achieved |
