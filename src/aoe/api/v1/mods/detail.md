# [POST] /api/v1/Mods/Detail/

**AUTHENTICATION**

## Request

```
POST /api/v1/Mods/Detail/ HTTP/1.1
Host: api.ageofempires.com
Accept-Encoding: identity
Accept: application/json
Authorization: Steam1.0 <TOKEN>
Content-Type: application/json
Content-Length: 24

{"game":2,"modid":14788}
```

| parameter | type | value | comments |
| --------- | ---- | ----- | -------- |
| game      | int  | 2     |          |
| modid     | int  | 14788 |          |

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
