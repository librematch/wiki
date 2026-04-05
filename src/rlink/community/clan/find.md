# [GET] /community/clan/find

[Example request](https://aoe-api.worldsedgelink.com/community/clan/find?title=age2&joinPolicies=[0,1,2]&name=GL&tags=[]&start=0&count=100)

Searches for clans by name, tags, and join policy. Returns a
paginated list of matching clans.

## Request

| parameter    | type     | value                  | comments                          |
| ------------ | -------- | ---------------------- | --------------------------------- |
| title        | str/enum | age1, age2, age3, age4 | Game title                        |
| joinPolicies | arr[int] | [0,1,2]                | Filter by join policy             |
| name         | str      | "GL"                   | Clan name substring to search for |
| tags         | arr[str] | []                     | Filter by tags                    |
| start        | int      | 0                      | Pagination offset                 |
| count        | int      | 100                    | Number of results to return       |

## Response

### AoE2:DE

Returns a `clans` array containing clan objects that match
the search criteria. The example below is trimmed to 2 entries;
a real response may contain up to `count` results.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "clans": [
        {
            "id": 9221,
            "name": "SME",
            "fullname": "Swiss_Martial_Eagle",
            "description": "",
            "tags": "",
            "icon": "",
            "membercount": 4,
            "joinpolicy": 0,
            "metadata": "",
            "messageoftheday": "",
            "statgroup_id": 458620
        },
        {
            "id": 8254,
            "name": "GTwn",
            "fullname": "Glendorians",
            "description": "",
            "tags": "",
            "icon": "",
            "membercount": 1,
            "joinpolicy": 1,
            "metadata": "",
            "messageoftheday": "",
            "statgroup_id": 414313
        }
    ]
}
```

| field           | type   | description                                         |
| --------------- | ------ | --------------------------------------------------- |
| id              | int    | Unique clan identifier                              |
| name            | string | Short clan tag (max 5 characters)                   |
| fullname        | string | Full display name of the clan                       |
| description     | string | Clan description text                               |
| tags            | string | Comma-separated tags                                |
| icon            | string | Clan icon identifier (e.g. `"CR-001"`)              |
| membercount     | int    | Current number of members                           |
| joinpolicy      | int    | Join policy (`0` = open, `1` = invite/request only) |
| metadata        | string | Additional metadata (JSON string)                   |
| messageoftheday | string | Clan message of the day                             |
| statgroup_id    | int    | Associated stat group identifier                    |
