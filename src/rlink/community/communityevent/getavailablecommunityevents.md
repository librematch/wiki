# [GET] /community/CommunityEvent/getAvailableCommunityEvents

[Example request](https://aoe-api.worldsedgelink.com/community/CommunityEvent/getAvailableCommunityEvents?title=age2)

## Request

| parameter | type     | value                  | comments |
| --------- | -------- | ---------------------- | -------- |
| title     | str/enum | age1, age2, age3, age4 |          |

## Response

### AoE2:DE

Returns currently active or recently ended community events
(e.g. sponsored tournaments with special leaderboards). The
array is empty when no events are active.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "communityEvents": [
        {
            "id": 57,
            "name": "Red Bull Wololo: Londinium",
            "start": 1767372900,
            "end": 1768755600,
            "expiryTime": 1777651200,
            "scheduledstarttime": 1767372900,
            "scheduledendtime": 1768755600,
            "scheduledexpirytime": 1777651200,
            "actualstarttime": 1767372910,
            "actualendtime": 1768755675,
            "customdata": "{\"ClientData\":{\"MatchTypeOverride\":[{\"current\":26,\"override\":124,\"leaderboard\":29,\"gamemode\":13,\"victoryType\":7,\"leaderboard-string\":\"IDS_MATCHMAKING_RED_BULL\",\"leaderboard-warning-string\":\"IDS_LEADERBOARD_RANKED_WARNING_RED_BULL_WOLOLO\",\"match-type-name\":[\"RBW_LONDINIUM\",\"IDS_MATCHMAKING_SPONSORED_TOURNAMENT\"],\"crossplay\":true,\"console\":false},{\"current\":86,\"override\":125,\"leaderboard\":30,\"gamemode\":13,\"victoryType\":7,\"leaderboard-string\":\"IDS_MATCHMAKING_RED_BULL_CO\",\"leaderboard-warning-string\":\"IDS_LEADERBOARD_RANKED_WARNING_RED_BULL_WOLOLO\",\"match-type-name\":[\"RBW_LONDINIUM\",\"IDS_MATCHMAKING_SPONSORED_TOURNAMENT\"],\"crossplay\":false,\"console\":true}],\"TournamentMode\":true}}",
            "eventstate": 2
        }
    ],
    "leaderboards": [],
    "leaderboardMaps": [],
    "rankLevels": []
}
```

| field              | type   | description                                            |
| ------------------ | ------ | ------------------------------------------------------ |
| id                 | int    | Event ID                                               |
| name               | string | Display name of the event                              |
| start              | int    | Unix timestamp for event start                         |
| end                | int    | Unix timestamp for event end                           |
| expiryTime         | int    | Unix timestamp when event data expires                 |
| scheduledstarttime | int    | Originally scheduled start time                        |
| scheduledendtime   | int    | Originally scheduled end time                          |
| actualstarttime    | int    | Actual start time (may differ from scheduled)          |
| actualendtime      | int    | Actual end time                                        |
| customdata         | string | JSON-encoded client config (match type overrides, etc) |
| eventstate         | int    | Event state (2 = ended)                                |
