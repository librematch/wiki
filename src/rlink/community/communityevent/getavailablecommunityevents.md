# [GET] /community/CommunityEvent/getAvailableCommunityEvents

[Example request](https://aoe-api.worldsedgelink.com/community/CommunityEvent/getAvailableCommunityEvents?title=age2)

## Request

| parameter | type     | value                  | comments |
| --------- | -------- | ---------------------- | -------- |
| title     | str/enum | age1, age2, age3, age4 |          |

## Response

### AoE2:DE

```
{
  "result": {
    "code": 0,
    "message": "SUCCESS"
  },
  "communityEvents": []
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
        "communityEvents": {
            "type": "array"
        }
    },
    "required": [
        "communityEvents",
        "result"
    ]
}
```
