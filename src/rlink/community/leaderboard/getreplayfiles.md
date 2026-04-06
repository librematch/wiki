# [GET] /community/leaderboard/getReplayFiles

[Example request](https://aoe-api.worldsedgelink.com/community/leaderboard/getReplayFiles?matchIDs=[468097482]&title=age2)

Returns signed download URLs for replay files of the requested
matches. Each match returns one replay file per player. The
download links expire after a period (see `expiryUnix`), so
replays should be downloaded and cached promptly.

## Request

| parameter | type       | value                  | comments           |
| --------- | ---------- | ---------------------- | ------------------ |
| title     | str/enum   | age1, age2, age3, age4 |                    |
| matchIDs  | array[int] | e.g. [468097482]       | max batch size ~10 |

## Rate Limits

This endpoint has a stricter rate limit than regular community
endpoints -- reportedly around **120 requests per minute**.
Batch requests on-demand and cache the downloaded replay files
to stay within limits.

## Response

### AoE2:DE

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "expiryUnix": 1775411322,
    "replayFiles": [
        {
            "profile_id": 8793414,
            "matchhistory_id": 468097482,
            "url": "https://rl0aoelivemk2blob.blob.core.windows.net/cloudfiles/.../M_468097482_...gz?sig=...&se=2026-04-05T17%3A48%3A42Z&sv=2019-02-02&sp=r&sr=b",
            "size": 788341,
            "datatype": 0
        },
        {
            "profile_id": 271202,
            "matchhistory_id": 468097482,
            "url": "https://rl0aoelivemk2blob.blob.core.windows.net/cloudfiles/.../M_468097482_...gz?sig=...&se=2026-04-05T17%3A48%3A42Z&sv=2019-02-02&sp=r&sr=b",
            "size": 778066,
            "datatype": 0
        }
    ]
}
```

| field           | type   | description                                                                                                 |
| --------------- | ------ | ----------------------------------------------------------------------------------------------------------- |
| expiryUnix      | int    | Unix timestamp when the signed URLs expire                                                                  |
| profile_id      | int    | Profile ID of the player who uploaded this replay                                                           |
| matchhistory_id | int    | Match ID this replay belongs to                                                                             |
| url             | string | Signed Azure Blob Storage URL (expires at expiryUnix)                                                       |
| size            | int    | File size in bytes; `-1` means the replay was never uploaded and the URL will return a `BlobNotFound` error |
| datatype        | int    | Data type identifier (0 = replay)                                                                           |

> **Note:** The `url` field is a signed Azure Blob Storage URL
> with an expiration timestamp. Download and cache replay files
> rather than storing the URL for later use. One replay file is
> returned per player in the match.

> **Important:** Filter out entries where `size` is `-1` — these
> replays were never uploaded by the player and the download URL
> will return a `BlobNotFound` error. Among the remaining entries,
> prefer the one with the largest `size`, as it is likely the most
> complete recording (i.e. from the player who stayed longest in
> the match).
