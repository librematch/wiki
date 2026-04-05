# [GET] /community/item/getInventoryByProfileIDs

[Example request](https://aoe-api.worldsedgelink.com/community/item/getInventoryByProfileIDs?title=age2&profileids=[196240])

## Request

| parameter  | type       | value                  | comments |
| ---------- | ---------- | ---------------------- | -------- |
| title      | str/enum   | age1, age2, age3, age4 |          |
| profileids | array[int] | e.g. [196240]          |          |

## Response

### AoE2:DE

Returns item inventories grouped by profile ID. The community
endpoint appears to always return empty inventory arrays --
for actual item data, use the authenticated
[/game/item/getInventoryByProfileIDs](../../game/item/getinventorybyprofileids.md)
endpoint instead.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "itemInstancesByProfileID": [
        {
            "\"196240\"": []
        }
    ]
}
```

> **Note:** The profile ID key in the response is
> double-quoted as a string (e.g. `"\"196240\""`). The
> inventory array is consistently empty on the community
> endpoint.
