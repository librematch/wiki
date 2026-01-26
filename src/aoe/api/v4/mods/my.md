# [POST] /api/v4/Mods/My/

**AUTHENTICATION**

## Request

### AoE4

```
POST /api/v4/Mods/My/ HTTP/1.1
Host: api.ageofempires.com
Accept-Encoding: identity
Accept: application/json
Authorization: Steam1.0 CAEQ8r/r2AwYBSBLKoABBvLEPiLC/jFgMWrApLt1wEVq/gNVsjg/mrmECUAQM5669cvmj8SxWM9wLNBzjZCyVJqlocVi/4hIU7il2ToQoiiLOiWuURy2ebX/AEcd8jS/iqMGZW6qIdoT9eumDueQOyKw4cH26mSVc3/bLRi2sf0vThM2dkt3eQ4Mnfr5xQs=
Content-Length: 83
Content-Type: application/json

{
    "q": "",
    "filter": 0,
    "sort": "",
    "order": "",
    "start": 1,
    "count": 20000,
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
| start     | int  | 1     |          |
| count     | int  | 20000 |          |
| game      | int  | 4     |          |
| modid     | int  | 0     |          |

## Response

### AoE2:DE

```
{
   "modId":14788,
   "gameTitleId":2,
   "gameTitleName":"Age of Empires II DE",
   "modName":"[GreatestTech] Gunpowder Tracer FX",
   "description":"<p>Gunpowder projectile shots will have thin smoke trails.</p>",
   "modDescription":"<p>Gunpowder projectile shots will have thin smoke trails.</p>",
   "changeList":"",
   "verifiedVersion":null,
   "modTypeId":12,
   "clientId":null,
   "modType":"Graphics",
   "modTags":[
      "12",
      "24",
      "25"
   ],
   "modTagIds":null,
   "modTagNames":[
      "Graphics",
      "Official",
      "Event"
   ],
   "metaData":{
      "modId":14788,
      "gameTitleId":null,
      "gameTitleName":null,
      "modName":"[GreatestTech] Gunpowder Tracer FX",
      "description":"<p>Gunpowder projectile shots will have thin smoke trails.</p>",
      "modDescription":"<p>Gunpowder projectile shots will have thin smoke trails.</p>",
      "changeList":null,
      "verifiedVersion":null,
      "modTypeId":null,
      "clientId":null,
      "modType":"Graphics",
      "modTags":[
         "12",
         "24",
         "25"
      ],
      "modTagIds":null,
      "modTagNames":[
         "Graphics",
         "Official",
         "Event"
      ],
      "metaData":null,
      "modStatusId":null,
      "modStatus":"Published",
      "modStatusMessage":null,
      "modVisibility":"Unlisted",
      "creatorId":null,
      "creatorName":"AoE Official",
      "creatorAvatarUrl":"https://images-eds-ssl.xboxlive.com/image?url=wHwbXKif8cus8csoZ03RW8ke8ralOdP9BGd4wzwl0MJ9z6QzuGwZjtvbE7sSsMVW.yovsDdui0TKE6WR.4_G12uLRBxuIvCnWAqCxdnHpyhcb0trk6v4voWKTlVqnrmoBvD0REWNWMHYDaEaY6h4q23at4q0mjQwBHt.ikWVbw0-&format=png",
      "isOwner":false,
      "isLoggedOn":true,
      "allowDiscussion":false,
      "discourseUrl":null,
      "createDate":"2020-04-29T15:26:20.85",
      "lastUpdate":"2020-04-29T15:26:20.85",
      "updateAvailable":false,
      "modFileSize":915274.0,
      "modDiskSize":929333.0,
      "popular":0,
      "downloads":80761,
      "installs":62181,
      "likes":119,
      "userLiked":false,
      "ratings":null,
      "currentRating":0.0,
      "userDownloaded":false,
      "userInstalled":false,
      "userFlagged":false,
      "userRating":null,
      "userReview":null,
      "positiveRatings":0,
      "totalRatings":0,
      "thumbnail":null,
      "fileUrl":null,
      "imageUrls":null
   },
   "modStatusId":2,
   "modStatus":"Published",
   "modStatusMessage":"",
   "modVisibility":null,
   "creatorId":null,
   "creatorName":null,
   "creatorAvatarUrl":null,
   "isOwner":null,
   "isLoggedOn":false,
   "allowDiscussion":false,
   "discourseUrl":null,
   "createDate":null,
   "lastUpdate":null,
   "updateAvailable":null,
   "modFileSize":null,
   "modDiskSize":null,
   "popular":0,
   "downloads":null,
   "installs":null,
   "likes":null,
   "userLiked":null,
   "ratings":null,
   "currentRating":0.0,
   "userDownloaded":null,
   "userInstalled":null,
   "userFlagged":null,
   "userRating":null,
   "userReview":null,
   "positiveRatings":0,
   "totalRatings":0,
   "thumbnail":null,
   "fileUrl":null,
   "imageUrls":[
      {
         "imageId":"e2f3e683-19ba-4f1b-b9c3-49aea7150139",
         "displayIndex":0,
         "imageName":"https://xforgeassets002.xboxlive.com/pf-title-aa0bae460e9fd6e4-5f5b4/e2f3e683-19ba-4f1b-b9c3-49aea7150139/modImage_0.jpg?width=1280&height=720",
         "imageThumbnail":"https://xforgeassets002.xboxlive.com/pf-title-aa0bae460e9fd6e4-5f5b4/e2f3e683-19ba-4f1b-b9c3-49aea7150139/modImage_0.jpg?width=400&height=225",
         "imageFileSize":null
      }
   ]
}
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
            "modId": 97570,
            "gameTitleId": 4,
            "gameTitleName": null,
            "modName": "PheniX Rise and Curry",
            "description": "PheniX Rise and Curry \r\nGold and Stone rises again :) \r\nWolfs are more mad 400 PoP \r\nMore Wood Better Fields",
            "modDescription": "PheniX Rise and Curry \r\nGold and Stone rises again :) \r\nWolfs are more mad 400 PoP \r\nMore Wood Better Fields",
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
            "creatorId": 9910532,
            "creatorName": "Freddy",
            "creatorAvatarUrl": "https://avatars.akamai.steamstatic.com/7eb86a98d34da786dc134603a248c7169791a9fa.jpg",
            "isOwner": false,
            "isLoggedOn": false,
            "allowDiscussion": false,
            "discourseUrl": null,
            "createDate": "2022-08-27T20:31:05.057",
            "lastUpdate": "2022-10-26T21:00:25.847",
            "updateAvailable": false,
            "modFileSize": 3360497.0,
            "modDiskSize": null,
            "popular": 14,
            "downloads": 18,
            "installs": null,
            "likes": 0,
            "userLiked": false,
            "ratings": {
                "leastFavorableReview": null,
                "mostFavorableReview": null,
                "rating": {
                    "average": 3.0,
                    "count1Star": null,
                    "count2Star": null,
                    "count3Star": null,
                    "count4Star": null,
                    "count5Star": null,
                    "totalCount": 1
                },
                "reviewsCount": 0
            },
            "currentRating": 3.0,
            "userDownloaded": false,
            "userInstalled": false,
            "userFlagged": false,
            "userRating": null,
            "userReview": null,
            "positiveRatings": 0,
            "totalRatings": 1,
            "thumbnail": "https://cdn.ageofempires.com/aoe-mods/4/97570/e1ba0efd.jpeg",
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
