# [POST] /api/v4/Mods/Installed/

**AUTHENTICATION**

## Request

### AoE4

```
POST /api/v4/Mods/Installed/ HTTP/1.1
Host: api.ageofempires.com
Accept-Encoding: identity
Accept: application/json
Authorization: Steam1.0 CAEQ8r/r2AwYBSBLKoABBvLEPiLC/jFgMWrApLt1wEVq/gNVsjg/mrmECUAQM5669cvmj8SxWM9wLNBzjZCyVJqlocVi/4hIU7il2ToQoiiLOiWuURy2ebX/AEcd8jS/iqMGZW6qIdoT9eumDueQOyKw4cH26mSVc3/bLRi2sf0vThM2dkt3eQ4Mnfr5xQs=
Content-Length: 79
Content-Type: application/json

{
    "q": "",
    "filter": 0,
    "sort": "",
    "order": "",
    "start": 0,
    "count": 0,
    "game": 4,
    "modid": 0
}
```

| parameter | type | value | comments |
| --------- | ---- | ----- | -------- |
| q         | ?    |       |          |
| filter    | int  | 0     |          |
| sort      | ?    |       |          |
| order     | ?    |       |          |
| start     | int  | 0     |          |
| count     | int  | 0     |          |
| game      | int  | 4     |          |
| modid     | int  | 0     |          |

## Response

### AoE2:DE

```
RESPONSE TEMPLATE
```

### AoE4

```
{
    "searchParams": {
        "q": null,
        "creator": null,
        "filter": 0,
        "sort": "lastUpdate",
        "order": "DESC",
        "start": 1,
        "count": 200,
        "game": 4,
        "modid": 0
    },
    "modList": [
        {
            "modId": 112877,
            "gameTitleId": 4,
            "gameTitleName": null,
            "modName": "Mobius Tuning Pack 2",
            "description": "Updated for Malians and Ottomans. \r\n \r\n- Traders contribute 0.2 to population, reduced from 1. \r\n- Increases resource limits from 100,000 to 100,000,000.",
            "modDescription": "Updated for Malians and Ottomans. \r\n \r\n- Traders contribute 0.2 to population, reduced from 1. \r\n- Increases resource limits from 100,000 to 100,000,000.",
            "changeList": null,
            "verifiedVersion": null,
            "modTypeId": 6,
            "clientId": "",
            "modType": "Extension",
            "modTags": null,
            "modTagIds": [
                4
            ],
            "modTagNames": [
                "Tuning Pack"
            ],
            "metaData": null,
            "modStatusId": 2,
            "modStatus": "Published",
            "modStatusMessage": null,
            "modVisibility": "Public",
            "creatorId": 2270778,
            "creatorName": "Mobius6469",
            "creatorAvatarUrl": "https://images-eds-ssl.xboxlive.com/image?url=z951ykn43p4FqWbbFvR2Ec.8vbDhj8G2Xe7JngaTToBrrCmIEEXHC9UNrdJ6P7KI4AAOijCgOA3.jozKovAH9wJVHMk5TchyPp7y7q0530QiLZPdTsSqNSrT34qiEmcl&format=png",
            "isOwner": false,
            "isLoggedOn": false,
            "allowDiscussion": false,
            "discourseUrl": null,
            "createDate": "2022-10-26T21:09:34.173",
            "lastUpdate": "2022-10-26T21:09:34.173",
            "updateAvailable": false,
            "modFileSize": 1635361.0,
            "modDiskSize": null,
            "popular": 3,
            "downloads": 3,
            "installs": null,
            "likes": 0,
            "userLiked": false,
            "ratings": {
                "leastFavorableReview": null,
                "mostFavorableReview": null,
                "rating": {
                    "average": 0.0,
                    "count1Star": null,
                    "count2Star": null,
                    "count3Star": null,
                    "count4Star": null,
                    "count5Star": null,
                    "totalCount": 0
                },
                "reviewsCount": 0
            },
            "currentRating": 0.0,
            "userDownloaded": false,
            "userInstalled": false,
            "userFlagged": false,
            "userRating": null,
            "userReview": null,
            "positiveRatings": 0,
            "totalRatings": 0,
            "thumbnail": "https://cdn.ageofempires.com/aoe-mods/4/112877/64ff210a.jpeg",
            "fileUrl": null,
            "imageUrls": null
        },
        {
            ...
        }
        
    ],
    "totalCount": 3109,
    "isLoggedOn": false
}
```
