# [GET] /community/leaderboard/getLeaderBoard2

[Example request](https://aoe-api.worldsedgelink.com/community/leaderboard/getLeaderBoard2?leaderboard_id=3&platform=PC_STEAM&title=age2&sortBy=1&start=1&count=200)

## Request

| parameter                              | type     | value                  | comments |
| -------------------------------------- | -------- | ---------------------- | -------- |
| leaderboard_id                         | int      | 3                      |          |
| platform                               | str/enum | PC_STEAM               |          |
| title                                  | str/enum | age1, age2, age3, age4 |          |
| sortBy                                 | int      | 1                      | ```      |
| sortBy=0                               |          |                        |          |
| `:= sorts by absolute number of wins,` |          |                        |          |
| sortBy=1                               |          |                        |          |

```:= sorts by rating |
| start | int | 1 |  |
| count | int | 200 |  |

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
"id": 4120710,
"name": "",
"type": 1,
"members": [
{
"profile_id": 5123311,
"name": "/steam/76561199142950174",
"alias": "[MoA]Beiçola",
"personal_statgroup_id": 4120710,
"xp": 407,
"level": 1,
"leaderboardregion_id": 4,
"country": "br"
}
]
},
{
"id": 6153140,
"name": "",
"type": 1,
"members": [
{
"profile_id": 10960083,
"name": "/steam/76561199385029768",
"alias": "Moonlight",
"personal_statgroup_id": 6153140,
"xp": 235,
"level": 1,
"leaderboardregion_id": 0,
"country": "it"
}
]
},
{
"id": 4961990,
"name": "",
"type": 1,
"members": [
{
"profile_id": 6440047,
"name": "/steam/76561198067238361",
"alias": "CL.Blackheart",
"personal_statgroup_id": 4961990,
"xp": 890,
"level": 1,
"leaderboardregion_id": 0,
"country": "de"
}
]
},
{
"id": 3381111,
"name": "",
"type": 1,
"members": [
{
"profile_id": 4012008,
"name": "/steam/76561198294644972",
"alias": "chaos_2_win",
"personal_statgroup_id": 3381111,
"xp": 2718,
"level": 2,
"leaderboardregion_id": 0,
"country": "de"
}
]
},
{
"id": 6263359,
"name": "",
"type": 1,
"members": [
{
"profile_id": 11383502,
"name": "/steam/76561199405610404",
"alias": "给那个",
"personal_statgroup_id": 6263359,
"xp": 13,
"level": 1,
"leaderboardregion_id": 5,
"country": "au"
}
]
},
{
"id": 10777,
"name": "",
"type": 1,
"members": [
{
"profile_id": 215963,
"name": "/steam/76561197960609427",
"alias": "[o.p.]fatman",
"personal_statgroup_id": 10777,
"xp": 2160,
"level": 2,
"leaderboardregion_id": 0,
"country": "de"
}
]
},
],
"leaderboardStats": [
{
"statgroup_id": 527797,
"leaderboard_id": 3,
"wins": 1427,
"losses": 851,
"streak": 2,
"disputes": 0,
"drops": 10,
"rank": 1,
"ranktotal": 39023,
"ranklevel": 1,
"rating": 2646,
"regionrank": -1,
"regionranktotal": -1,
"lastmatchdate": 1666299350
},
{
"statgroup_id": 1492,
"leaderboard_id": 3,
"wins": 1696,
"losses": 873,
"streak": 3,
"disputes": 0,
"drops": 10,
"rank": 2,
"ranktotal": 39023,
"ranklevel": 1,
"rating": 2617,
"regionrank": -1,
"regionranktotal": -1,
"lastmatchdate": 1666113105
},
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
"regionrank": -1,
"regionranktotal": -1,
"lastmatchdate": 1664555924
},
{
"statgroup_id": 173507,
"leaderboard_id": 3,
"wins": 2154,
"losses": 973,
"streak": 3,
"disputes": 0,
"drops": 40,
"rank": 4,
"ranktotal": 39023,
"ranklevel": 1,
"rating": 2594,
"regionrank": -1,
"regionranktotal": -1,
"lastmatchdate": 1665298806
},
{
"statgroup_id": 1137,
"leaderboard_id": 3,
"wins": 999,
"losses": 378,
"streak": 3,
"disputes": 0,
"drops": 8,
"rank": 5,
"ranktotal": 39023,
"ranklevel": 1,
"rating": 2591,
"regionrank": -1,
"regionranktotal": -1,
"lastmatchdate": 1665956337
},
{
"statgroup_id": 297,
"leaderboard_id": 3,
"wins": 2161,
"losses": 947,
"streak": 8,
"disputes": 0,
"drops": 17,
"rank": 6,
"ranktotal": 39023,
"ranklevel": 1,
"rating": 2587,
"regionrank": -1,
"regionranktotal": -1,
"lastmatchdate": 1665145236
},
{
"statgroup_id": 273,
"leaderboard_id": 3,
"wins": 1170,
"losses": 685,
"streak": 2,
"disputes": 0,
"drops": 18,
"rank": 7,
"ranktotal": 39023,
"ranklevel": 1,
"rating": 2585,
"regionrank": -1,
"regionranktotal": -1,
"lastmatchdate": 1665861387
},
{
"statgroup_id": 1855428,
"leaderboard_id": 3,
"wins": 1254,
"losses": 927,
"streak": 2,
"disputes": 0,
"drops": 12,
"rank": 8,
"ranktotal": 39023,
"ranklevel": 1,
"rating": 2584,
"regionrank": -1,
"regionranktotal": -1,
"lastmatchdate": 1666289097
},
{
"statgroup_id": 55127,
"leaderboard_id": 3,
"wins": 2541,
"losses": 1039,
"streak": 5,
"disputes": 0,
"drops": 90,
"rank": 9,
"ranktotal": 39023,
"ranklevel": 1,
"rating": 2583,
"regionrank": -1,
"regionranktotal": -1,
"lastmatchdate": 1666217850
},
{
"statgroup_id": 5840698,
"leaderboard_id": 3,
"wins": 192,
"losses": 65,
"streak": 4,
"disputes": 0,
"drops": 3,
"rank": 10,
"ranktotal": 39023,
"ranklevel": 1,
"rating": 2571,
"regionrank": -1,
"regionranktotal": -1,
"lastmatchdate": 1665838700
},
{
"statgroup_id": 6835,
"leaderboard_id": 3,
"wins": 589,
"losses": 262,
"streak": 10,
"disputes": 0,
"drops": 6,
"rank": 11,
"ranktotal": 39023,
"ranklevel": 1,
"rating": 2565,
"regionrank": -1,
"regionranktotal": -1,
"lastmatchdate": 1664756820
},
],
"rankTotal": 39023
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
},
"rankTotal": {
"type": "integer"
}
},
"required": [
"leaderboardStats",
"rankTotal",
"result",
"statGroups"
]
}

```
```
