# [GET] /community/item/getInventoryByProfileIDs

[Example request](https://aoe-api.worldsedgelink.com/community/item/getInventoryByProfileIDs?title=age2&profileids=[196240])

## Request

| parameter  | type     | value                  | comments |
| ---------- | -------- | ---------------------- | -------- |
| title      | str/enum | age1, age2, age3, age4 |          |
| profileids | arr[int] | [196240]               |          |

## Response

### AoE2:DE

```
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
        "itemInstancesByProfileID": {
            "type": "array",
            "items": {
                "type": "object",
                "properties": {
                    "\"196240\"": {
                        "type": "array"
                    }
                },
                "required": [
                    "\"196240\""
                ]
            }
        }
    },
    "required": [
        "itemInstancesByProfileID",
        "result"
    ]
}
```
