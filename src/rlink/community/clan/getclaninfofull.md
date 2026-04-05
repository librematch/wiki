# [GET] /community/clan/getClanInfoFull

[Example request](https://aoe-api.worldsedgelink.com/community/clan/getClanInfoFull?title=age2&name=gli)

Returns full details for a clan including its permissions and
member list with player avatars.

## Request

| parameter | type     | value                  | comments   |
| --------- | -------- | ---------------------- | ---------- |
| title     | str/enum | age1, age2, age3, age4 | Game title |
| name      | str      | gli                    | Clan tag   |

## Response

### AoE2:DE

Returns the clan object with nested `permissions` (one entry
per role rank) and `members` (one entry per clan member).
The members array below is trimmed to 1 entry.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "clan": {
        "id": 52618,
        "name": "gli",
        "fullname": "TheClick",
        "description": "",
        "tags": "",
        "icon": "CR-001",
        "membercount": 4,
        "joinpolicy": 0,
        "metadata": "",
        "messageoftheday": "",
        "statgroup_id": 2254028,
        "permissions": [
            {
                "rank": 1,
                "chat": 1,
                "promote": 1,
                "demote": 1,
                "invite": 1,
                "remove": 1,
                "disband": 1,
                "editinfo": 1,
                "editpermission": 1,
                "name": "Leader",
                "locstringid": -1
            },
            {
                "rank": 2,
                "chat": 1,
                "promote": 1,
                "demote": 1,
                "invite": 1,
                "remove": 1,
                "disband": 0,
                "editinfo": 0,
                "editpermission": 0,
                "name": "Officer",
                "locstringid": -1
            },
            {
                "rank": 3,
                "chat": 1,
                "promote": 0,
                "demote": 0,
                "invite": 0,
                "remove": 0,
                "disband": 0,
                "editinfo": 0,
                "editpermission": 0,
                "name": "Member",
                "locstringid": -1
            }
        ],
        "members": [
            {
                "avatar": {
                    "entityversion": 7676,
                    "profile_id": 2327018,
                    "name": "/steam/76561198300477799",
                    "metadata": "{\"icon\":\"PR7-031\"}",
                    "alias": "Atashwong",
                    "clanlist_name": "gli",
                    "personal_statgroup_id": 2072253,
                    "xp": 276,
                    "level": 1,
                    "leaderboardregion_id": 3,
                    "presence_id": 0,
                    "presenceproperty": []
                },
                "membershipstatus": 1,
                "playerlistpermission_rank": 1
            }
        ]
    }
}
```

#### Clan fields

| field           | type   | description                                         |
| --------------- | ------ | --------------------------------------------------- |
| id              | int    | Unique clan identifier                              |
| name            | string | Short clan tag                                      |
| fullname        | string | Full display name of the clan                       |
| description     | string | Clan description text                               |
| tags            | string | Comma-separated tags                                |
| icon            | string | Clan icon identifier (e.g. `"CR-001"`)              |
| membercount     | int    | Current number of members                           |
| joinpolicy      | int    | Join policy (`0` = open, `1` = invite/request only) |
| metadata        | string | Additional metadata (JSON string)                   |
| messageoftheday | string | Clan message of the day                             |
| statgroup_id    | int    | Associated stat group identifier                    |

#### Permission fields

| field          | type   | description                                           |
| -------------- | ------ | ----------------------------------------------------- |
| rank           | int    | Role rank (`1` = Leader, `2` = Officer, `3` = Member) |
| chat           | int    | Can send chat messages (`0`/`1`)                      |
| promote        | int    | Can promote members (`0`/`1`)                         |
| demote         | int    | Can demote members (`0`/`1`)                          |
| invite         | int    | Can invite players (`0`/`1`)                          |
| remove         | int    | Can remove members (`0`/`1`)                          |
| disband        | int    | Can disband the clan (`0`/`1`)                        |
| editinfo       | int    | Can edit clan info (`0`/`1`)                          |
| editpermission | int    | Can edit role permissions (`0`/`1`)                   |
| name           | string | Display name of the role                              |
| locstringid    | int    | Localization string ID (`-1` if custom)               |

#### Member fields

| field                     | type | description                      |
| ------------------------- | ---- | -------------------------------- |
| membershipstatus          | int  | Membership status (`1` = active) |
| playerlistpermission_rank | int  | Permission rank of this member   |

#### Avatar fields (nested in each member)

| field                 | type   | description                              |
| --------------------- | ------ | ---------------------------------------- |
| entityversion         | int    | Version counter for the entity           |
| profile_id            | int    | Unique player profile identifier         |
| name                  | string | Platform identifier (e.g. `/steam/<id>`) |
| metadata              | string | JSON string with profile metadata        |
| alias                 | string | Player display name                      |
| clanlist_name         | string | Clan tag the player belongs to           |
| personal_statgroup_id | int    | Player's personal stat group identifier  |
| xp                    | int    | Experience points                        |
| level                 | int    | Player level                             |
| leaderboardregion_id  | int    | Leaderboard region identifier            |
| presence_id           | int    | Online presence status                   |
| presenceproperty      | array  | Additional presence properties           |
