# [GET] /game/news/getNews

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/news/getNews?callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz HTTP/1.1
Cookie: ApplicationGatewayAffinity=1;ApplicationGatewayAffinityCORS=2;worldsedgelink=3;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| callNum      | int       | 123   |          |
| connect_id   |           |       |          |
| lastCallTime | timestamp |       |          |
| sessionID    | str       |       |          |

### Response

```
RESPONSE_TEMPLATE
```

## AoE4

### Request

```
GET /game/news/getNews?callNum=10&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=4963&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| callNum      | int       | 123   |          |
| connect_id   |           |       |          |
| lastCallTime | timestamp |       |          |
| sessionID    | str       |       |          |

### Response

```
[
    0,
    [
        [
            80,
            "Hero - Season3Live Anniv. Events",
            "Season Three",
            "Season Three: Anniversary is now live!",
            "Season Three: Anniversary! is here along with a brand new Ranked season, new challenges, and more!\r\n\r\nThe new Ranked Season, along with the all-new Team Ranked runs from **October 26th** through **February 15th**! \r\n\r\nMissed an announcement? Head on over the link below to check out our Broadcast Recap and learn more about all of the exciting 25th Anniversary Events across the Age of Empires franchise.",
            "https://www.ageofempires.com/wp-content/uploads/2022/10/anniversary_trio_1920x1080-1.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"hero\", \"widget\"],\r\n \"url\": \"https://aoe.ms/aoe4-icymi\"\r\n}",
            1666681200,
            1669881600
        ],
        [
            82,
            "Hero - ICYMI - Anniv. Events",
            "Anniversary Event",
            "Runs October 25th - November 28th.",
            "Running from **October 25th through November 28th**, the Anniversary event brings a number of unique challenges for you to complete and exclusive rewards to earn!\r\n\r\nHead on over to the link below more information on all of the 25th Anniversary events across the Age of Empires franchise.\r\n\r\nYou have also received the following items for logging in during this portion of Season Three: Anniversary!\r\n\r\n* 25th Age-aversary! portrait\r\n* 25th Coin portrait\r\n* Chibi Wololo Priest portrait",
            "https://www.ageofempires.com/wp-content/uploads/2022/10/anniversary_trio_1920x1080-1.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"popup\", \"hero\"],\r\n \"url\": \"https://aoe.ms/aoe4-s3-anniv-event\"\r\n}",
            1666681200,
            1669881600
        ],
        [
            83,
            "News + Hero - RB Twitch",
            "Stream Red Bull Wololo: Legacy",
            "Tune in to the official tournament stream",
            "To battle! Red Bull Wololo is back, bringing together the best Age of Empires players from around the world for a battle of the ages. Who will be crowned the ultimate champion of Age of Empires IV? **Red Bull Wololo: Legacy runs from 10/21 to 10/30** - tune in here to catch all the action: [twitch.tv/redbull](https://twitch.tv/redbull).",
            "https://www.ageofempires.com/wp-content/uploads/2022/09/RBWL_CORECT_noweapons_1920x1080-1080x608.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"widget\", \"hero\"],\r\n \"url\": \"https://aoe.ms/rb-wololo\"\r\n}",
            1666335600,
            1667372400
        ],
        [
            78,
            "News - Patch Notes",
            "Season Three Notes",
            "Check out the latest Release Notes for Season Three: Anniversary!",
            "The party is about to get started in _Age of Empires IV_ with Season Three: Anniversary! \r\n\r\nThis Season Three update brings with it a number of reasons to celebrate including the new Ottoman and Malian civilizations, eight new maps, the long-anticipated cheat and taunt systems, and so much more!\r\n\r\nThe celebration kicks off on **October 25th**, with Ranked Seasons (including the new Team Ranked) making their triumphant return shortly afterward on **October 26th**.\r\n\r\nHead on over to the link below to read the complete set of release notes for our Season Three: Anniversary! Update.",
            "https://www.ageofempires.com/wp-content/uploads/2022/10/S3_25Anni_Update_1920x1080.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"widget\"],\r\n \"url\": \"https://aoe.ms/aoe-iv-s3-patch-notes\"\r\n}",
            1666249200,
            1669881600
        ],
        [
            79,
            "News - Taunts FAQ",
            "Taunts & Cheats",
            "Learn how they work with our FAQ",
            "Taunts & Cheats make their debut in _Age of Empires IV_ with our Anniversary update. Head on over to the Taunts & Cheats FAQ page at the link below to learn how to use them in your games.",
            "https://www.ageofempires.com/wp-content/uploads/2021/04/NDA2_1920x1080.png",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"widget\"],\r\n \"url\": \"https://aoe.ms/aoeiv-taunt-faq\"\r\n}",
            1666249200,
            1669881600
        ],
        [
            73,
            "News - Anniv Stream Recap",
            "Stream Recap",
            "Watch the VOD of our latest stream.",
            "Our latest stream saw members of the development team discussing upcoming content in the _Age of Empires IV_ Anniversary Update set to land on **October 25th**. \r\n  \r\nHead on over to the _Age of Empires_ YouTube page using the link below to check it out!",
            "https://www.ageofempires.com/wp-content/uploads/2022/10/anniv_stream.png",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"featured\"],\r\n \"url\": \"https://aoe.ms/aoe-iv-anniv-stream-vod\"\r\n}",
            1666162800,
            1669881600
        ],
        [
            74,
            "News - Wololo Event",
            "Red Bull Wololo: Legacy",
            "Tournament runs Oct. 21 \u2013 30",
            "The latest installment in the Red Bull Wololo tournament series brings together some of the top players of _Age of Empires_, as they battle it out in the picturesque Castle Heidelberg of Germany!  \r\n\r\nAs the biggest tournament to date, Red Bull Wololo: Legacy runs from **October 21st through 30th** and features tournaments across multiple titles including _Age of Empires: Definitive Edition_, _Age of Empires II: Definitive Edition_, and _Age of Empires IV_! \r\n\r\nThe _Age of Empires IV_ portion kicks off on **October 26th**, with semi-finals and finals taking place on **October 30th**! \r\n\r\nHead on over to the Red Bull website below for more information on this exciting event.",
            "https://www.ageofempires.com/wp-content/uploads/2022/09/RBWL_CORECT_noweapons_1920x1080-1080x608.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"widget\", \"featured\"],\r\n \"url\": \"https://aoe.ms/wololo-legacy-details\"\r\n}",
            1665644400,
            1667199600
        ],
        [
            77,
            "News - Ranked Dates",
            "Ranked Games",
            "Ranked returns October 26th - Feb 15th as part of Season Three: Anniversary!",
            "Season Three: Anniversary brings with it the return of ranked gameplay as the new Ranked Season kicks off on **October 26th**!\r\n\r\nPlus, for the first time ever take part in the all-new Team Ranked! \r\n\r\nHead on over the link below to learn more.",
            "https://www.ageofempires.com/wp-content/uploads/2022/10/S3_25Anni_Update_1920x1080.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"popup\", \"widget\"],\r\n\"showAlways\": false,\r\n \"url\": \"https://aoe.ms/aoe-iv-s3-dates\"\r\n}",
            1665644400,
            1676880000
        ],
        [
            69,
            "Mods - New Guides",
            "New Guides Available",
            "New guides on the Content Editor and Mod creation are now available.",
            "With several newly published guides, there's now even more help for those looking to create their own content for _Age of Empires IV_ using the Content Editor (Beta).\r\n\r\n---\r\n\r\n### VillagerLife Prefabs\r\nThese entities will spawn a number of villagers in a designated area that go about pre-set tasks such as gathering resources or wandering, and can be set to either flee from a player, attack, or ignore them. These prefabs can make a map feel more \"alive,\" and open the door to creating lively villages, bustling cities, or towns of bloodthirsty, axe-wielding villagers.\r\n\r\n[View Guide](https://support.ageofempires.com/hc/en-us/articles/5585466092436-VillagerLife-Prefabs)\r\n\r\n---\r\n\r\n### Ultimate Grass Guide\r\nThere are a ton of grass assets available in Age of Empires IV, from field tufts and flowers to wheat crops and scorched patches of dead grass. This guide offers a comprehensive look at the many ways grass can be manipulated and applied to a crafted map or custom scenario.\r\n\r\n[View Guide](https://support.ageofempires.com/hc/en-us/articles/5843509475476-Ultimate-Grass-Guide)\r\n\r\n---\r\n\r\n### Creating Intro/Outro Cameras\r\nOften when beginning or finishing a custom scenario the player is taken on a swooping flyby of the map, setting the stage for the action to come or framing their victory. Now you can make use of these flying cameras as well! This guide covers everything you need to know about creating your own intro and outro camera movements.\r\n\r\n[View Guide](https://support.ageofempires.com/hc/en-us/articles/5893486569364-Creating-Intro-Outro-Cameras)\r\n\r\n---\r\n\r\n### Sculpting Terrain\r\nWhile they share many properties with other heightfield tools, the terrain sculpting capabilities of the Content Editor contain some unique quirks and features. This guide covers how to use all the specialized heightfield brushes and custom settings to sculpt terrain and create the exact effect you want.\r\n\r\n[View Guide](https://support.ageofempires.com/hc/en-us/articles/5264798022548-Sculpting-Terrain)\r\n\r\n---\r\n\r\n### Painting Trees\r\nForests are an integral part of an _Age of Empires IV_ map, as they define the map?s appearance, provide resources, define passable areas, and can even be used to hide units. This guide goes over how to create areas that will spawn specific types of trees.\r\n\r\n[View Guide](https://support.ageofempires.com/hc/en-us/articles/5026862103188-Placing-Trees)\r\n\r\n---\r\n\r\n### Creating Fog of War Areas\r\nSpecific areas on a map can contain customized Fog of War settings that display as either explored, revealed, or unexplored. This guide covers how to define areas of a map where the Fog of War will behave in a specified way.\r\n\r\n[View Guide](https://support.ageofempires.com/hc/en-us/articles/5722455564052-Creating-Fog-of-War-Areas)\r\n\r\n---\r\n\r\n### Player Settings\r\nThere are a number of player controls available for crafted maps and custom scenarios that allow mod creators to control aspects of player slots, team allegiances, faction colours, and AI settings. This guide covers what these player settings are and what effect they have.\r\n\r\n[View Guide](https://support.ageofempires.com/hc/en-us/articles/5502424402324-Adjusting-Player-Settings)",
            "https://www.ageofempires.com/wp-content/uploads/2021/04/NDA2_1920x1080.png",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"ugc\"],\r\n \"url\": \"https://support.ageofempires.com/hc/en-us/sections/360012376652-Age-of-Empires-IV-Mod-Workshop\"\r\n}",
            1664434800,
            1672473600
        ],
        [
            70,
            "Mods - Community Spotlight",
            "Community Mod Spotlight",
            "Check out just a few of the amazing mods created by members of the Age of Empires IV community!",
            "Since the release of the _Age of Empires IV_ Content Editor (Beta) we\u2019ve seen a ton of cool content created by members of the _Age of Empires IV_ community! \r\n\r\nIn the four short months since we launched the [Content Editor (Beta)](https://www.ageofempires.com/news/customize-your-battle-with-the-age-of-empires-iv-content-editor-beta/) back in April, players just like you have been hard at work creating a ton of awesome new maps, tuning packs, and game modes for everyone to enjoy.\r\n\r\nIn fact, there\u2019s so much cool content out there that we thought it was worth sharing them in a Community Mod Spotlight. \r\n\r\n---\r\n\r\n### Castle Blood Automatic\r\n_Created by kzoacn_\r\n![Castle Blood Automatic](https://xforgeassets002.xboxlive.com/pf-title-aa0bae460e9fd6e4-ed603/b2b2f6a6-f538-4754-b81e-195efd30b754/thumbnail.jpeg?width=768&height=432)\r\nThe classic game mode from Age of Empires II has been re-created in Age of Empires IV! Castle Blood Automatic provides all players with a castle that continuously spawns units, creating a free-for-all bloodbath in the center of the map. This mod changes the fundamentals of play and is a great example of a mod bundle containing three parts: a game mode, tuning pack, and crafted map.\r\n\r\n[View Mod](https://www.ageofempires.com/mods/details/55628/)\r\n\r\n---\r\n\r\n### Trojan Sheep\r\n_Created by Kotri_\r\n![Trojan Sheep](https://xforgeassets001.xboxlive.com/pf-title-aa0bae460e9fd6e4-ed603/1c5900f7-0487-479b-9bd5-79f7b438134f/thumbnail.jpeg?width=768&height=432)\r\nAn incredibly unique Tuning Pack adds a new unit to the game; a non-hostile sheep that can explode to cause damage to all units within range. In addition to being absolutely hilarious, this adds an interesting dynamic to play as players must constantly be on the lookout for these stealthy neutral sheep, as their units will not automatically attack them.\r\n\r\n[View Mod](https://www.ageofempires.com/mods/details/55540/)\r\n\r\n---\r\n\r\n### Cauldron\r\n_Created by 'Twister_\r\n![Cauldron](https://xforgeassets001.xboxlive.com/pf-title-aa0bae460e9fd6e4-ed603/33350abb-c2d3-461d-868f-d503f6e7758c/thumbnail.jpeg?width=768&height=432)\r\nA rocky, mountainous map with a small lake in the center teeming with fish. Cauldron provides players an isolated corner to build in while fighting over control of the central lake and it's abundant fishy bounty.\r\n\r\n[View Mod](https://www.ageofempires.com/mods/details/94208/)\r\n\r\n---\r\n\r\n### Four Lakes\r\n_Created by Bidderlyn & Fano_\r\n![Four Lakes](https://xforgeassets001.xboxlive.com/pf-title-aa0bae460e9fd6e4-ed603/13b2daa0-dd34-4398-85e5-56ae360b3661/thumbnail.jpeg?width=768&height=432)\r\nA remake of a classic Age of Empires II map, Four Lakes features a flat plain with lake in each corner. These lakes each hold a bounty of fish, encouraging players to control of as much coastline as they can to get a food advantage over their opponents.\r\n\r\n[View Mod](https://www.ageofempires.com/mods/details/72914/)\r\n\r\n---\r\n\r\n### Basin \r\n_Created by IamAvely_\r\n![Basin](https://xforgeassets001.xboxlive.com/pf-title-aa0bae460e9fd6e4-ed603/21863386-a4df-4a0d-9a32-7946dd12e75c/thumbnail.jpeg?width=768&height=432)\r\nA hilly map covered in forests, the land gives way to a flat plain in the centre. Encouraging \"king of the hill\" style gameplay, Basin provides each player with a sacred site near their start location as they vie for control of the single sacred site in the middle.\r\n\r\n[View Mod](https://www.ageofempires.com/mods/details/94798/)\r\n\r\n---\r\n\r\nOf course, these are just a select few of the thousands of mods already available for _Age of Empires IV_, with more and more being released each and every day! \r\n\r\nWant to see your own content shared here in the future? Learn more about the _Age of Empires_ Content Editor (Beta) at the link below and get creating today!",
            "https://www.ageofempires.com/wp-content/uploads/2022/04/UGC_Banner_v2_1920x1080-3.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"ugc\"],\r\n \"url\": \"https://www.ageofempires.com/news/customize-your-battle-with-the-age-of-empires-iv-content-editor-beta/\"\r\n}",
            1664434800,
            1672473600
        ],
        [
            72,
            "Hero - Anniv. Celebration",
            "AoE Anniversary celebration!",
            "Join us on October 25th for our anniversary broadcast",
            "We\u2019re thrilled to announce that on **October 25th**, we\u2019ll be celebrating 25 years of _Age of Empires_ in a big way. \n\nJoin us live from a special location as we share our Anniversary Broadcast featuring announcements, interviews with the team and some surprises. \n\nOf course, we want to maintain an air of mystery so we won\u2019t tell you exactly what we have garrisoned in our Town Center but we promise, there\u2019ll be something for everyone! **Tune in October 25th, 10am PT** to take part.",
            "https://www.ageofempires.com/wp-content/uploads/2022/09/AgeIV-AnniversaryEd-1920x1080-1.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"hero\", \"widget\"],\r\n \"showAlways\": false,\r\n \"url\": \"https://aoe.ms/25-years-of-aoe\"\r\n}",
            1664348400,
            1668067200
        ],
        [
            37,
            "Mods - Royal Rumble",
            "Royal Rumble",
            "Check out Royal Rumble, a new mod from the Age IV dev team.",
            "Alongside the Beta launch of the _Age of Empires_ Content Editor, the development team has released a new mod for you to try - Royal Rumble! \r\n\r\nAchieve victory by eliminating enemy Kings while defending your own in this classic game mode inspired by Regicide in Age of Empires II.",
            "https://www.ageofempires.com/wp-content/uploads/2022/04/UGC_Banner_v2_1920x1080-3.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"ugc\"]\r\n}",
            1649278800,
            1672473600
        ],
        [
            38,
            "Mods - Content Editor",
            "Content Editor",
            "The Age IV Content Editor is your one-stop shop for custom play.",
            "Want to create your own highly specialized map? Want to play with a French Knight that\u2019s overpowered to the nth degree?\n\nWith the launch of Season One, the Beta release of the _Age of Empires IV_ Content Editor will allow you to play around with several customization options. \n\nClick on the link below to find out more!",
            "https://www.ageofempires.com/wp-content/uploads/2022/04/UGC_Banner_v2_1920x1080-3.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"ugc\"],\r\n \"url\": \"https://aoe.ms/content-editor-beta\"\r\n}",
            1649242800,
            1672473600
        ],
        [
            39,
            "Mods - Welcome to Mods!",
            "Welcome to Mods!",
            "Learn more about creating and using mods!",
            "We're excited to have brought the Age of Empires IV Content Editor (Beta) online as part of Season One! This free content creation tool provides new and advanced creators with the ability to sculpt their own maps, craft unique mission scenarios, forge data driven tuning packs and envision new modes of play for Age IV.\r\n\r\nThe Age IV Content Editing tool will initially be launched in a BETA format. This will enable the Age IV team to fix bugs, refine existing features and develop new ones. Your feedback is incredibly important to us, and will be critical in our efforts to further enhance the editor for all players.\r\n\r\nClick on the link below to find out more about the Content Editor and the tutorial docs created by the team to further help guide creators through the process of understanding the various features and functionality the tooling provides.",
            "https://www.ageofempires.com/wp-content/uploads/2022/04/UGC_Banner_v2_1920x1080-3.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"ugc\"],\r\n \"url\": \"https://aoe.ms/mod-workshop\"\r\n}",
            1649228400,
            1672473600
        ],
        [
            16,
            "News - New to Age",
            "New to Age?",
            "Here is where you can start!",
            "Welcome to _Age of Empires IV_! There's a lot for you to play and dive into. Don't know where to start? Click below for some advice from our own _Age of Empires IV_ experts!",
            "https://www.ageofempires.com/wp-content/uploads/2021/10/Community_Tab_NewtoAge4.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"featured\"],\r\n \"url\": \"https://aoe.ms/newtoage4\"\r\n}",
            1635231605,
            2234847600
        ],
        [
            17,
            "News - Video Playlist",
            "Watch more AOE",
            "Check out our Age IV videos on YouTube.",
            "Looking for more _Age of Empires IV_ content? \n  \nThe _Age of Empires IV_ playlist over on our YouTube page has you covered with Game Trailers, Behind the Scenes, Developer Showcases, and more!",
            "https://www.ageofempires.com/wp-content/uploads/2021/10/Community_Tab_Thumbs_CuratedPlaylist.png",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"featured\"],\r\n \"url\": \"https://aoe.ms/aoe4-yt-playlist\"\r\n}",
            1635231604,
            2234847600
        ],
        [
            18,
            "News - Code of Conduct",
            "Code of Conduct",
            "Read the Code of Conduct for Age of Empires",
            "With the release of the _Age of Empires IV_ Season One update, we welcome all our players and creators who are enjoying the new content, including mods! \r\n\r\nFind out more about what makes us such a diverse community and our commitment to making _Age of Empires_ a welcome and safe place to engage.",
            "https://www.ageofempires.com/wp-content/uploads/2021/04/NDA2_1920x1080.png",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"featured\", \"ugc\"],\r\n \"url\": \"https://aoe.ms/codeofconduct\"\r\n}",
            1635231603,
            2234847600
        ],
        [
            13,
            "News - More News Static",
            "MORE NEWS",
            "Read up on more news here.",
            "For more news, information, and updates go to ageofempires.com!",
            "https://static.ageofempires.com/aoe/wp-content/uploads/2021/04/Placeholder_1920x1080.png",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"featured\"],\r\n \"url\": \"https://www.ageofempires.com/news?game=aoeiv\"\r\n}",
            1633676400,
            2234995200
        ],
        [
            2,
            "Social - Discord",
            "Discord",
            "Join the chat on Discord.",
            null,
            "https://static.ageofempires.com/aoe/wp-content/uploads/2021/06/social_discord.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"social\"],\r\n \"url\": \"https://discord.gg/ageofempires\"\r\n}",
            1622660400,
            2209017600
        ],
        [
            3,
            "Social - Facebook",
            "Facebook",
            "Check out our Facebook page.",
            null,
            "https://static.ageofempires.com/aoe/wp-content/uploads/2021/06/social_facebook.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"social\"],\r\n \"url\": \"https://www.facebook.com/ageofempires/\"\r\n}",
            1622660400,
            2209017600
        ],
        [
            1,
            "Social - Forums",
            "Forums",
            "Join the discussion on the official Forums.",
            null,
            "https://www.ageofempires.com/wp-content/uploads/2021/04/BugForums2_1920x1080.png",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"social\"],\r\n \"url\": \"https://forums.ageofempires.com/c/age-of-empires-iv/184\"\r\n}",
            1622574000,
            2209017600
        ],
        [
            4,
            "Social - Twitter",
            "Twitter",
            "Catch the latest updates on Twitter.",
            null,
            "https://static.ageofempires.com/aoe/wp-content/uploads/2021/06/social_twitter.jpg",
            "",
            "{\r\n \"version\": 1,\r\n \"categories\": [\"social\"],\r\n \"url\": \"https://twitter.com/AgeOfEmpires\"\r\n}",
            -62135524800,
            2209017600
        ]
    ],
    [
        [
            "Season 3 - Event 1a - Anniversary",
            1666716600,
            1669708740,
            1669708740,
            22,
            0,
            null,
            ""
        ],
        [
            "Season 3 - Login Reward 1 - Anniversary",
            1666716600,
            1669708740,
            1669708740,
            24,
            0,
            null,
            ""
        ],
        [
            "Season 3 - Login Reward 2 - Anniversary - chibi wololo",
            1666716600,
            1669708740,
            1669708740,
            25,
            0,
            null,
            ""
        ],
        [
            "Season 3 - Login Reward 3 - Coin",
            1666716600,
            1669708740,
            1669708740,
            26,
            0,
            null,
            ""
        ],
        [
            "Season 3 - Takeover Image - Anniversary",
            1666718100,
            1669708740,
            1669708740,
            28,
            0,
            null,
            "{\"frontEndImagePath\":\"\\\\Images\\\\backgrounds\\\\events\\\\s03_25anniversary.png\"}"
        ],
        [
            "Season 3 - Solo Ranked Season",
            1666804500,
            1676534340,
            1893484800,
            31,
            6,
            "Season 3",
            "{\"leaderboard\":{\"leaderboards\":[{\"copyFromBase\":1,\"scoringType\":2}],\"decay\":{\"reqRating\":1400,\"minDays\":15,\"amountPerDay\":5,\"maxAmount\":200},\"rankLevels\":{\"customRanks\":[{\"name\":\"Conqueror III\",\"locID\":\"11202624\",\"icon\":\"\\\\Images\\\\multiplayer\\\\conquerer_3.png\",\"icon2\":\"ffab3c\",\"level\":18,\"tier\":6,\"minRating\":1600,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1200},{\"name\":\"Conqueror II\",\"locID\":\"11202625\",\"icon\":\"\\\\Images\\\\multiplayer\\\\conquerer_2.png\",\"icon2\":\"ffab3c\",\"level\":17,\"tier\":6,\"minRating\":1500,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1200},{\"name\":\"Conqueror I\",\"locID\":\"11202626\",\"icon\":\"\\\\Images\\\\multiplayer\\\\conquerer_1.png\",\"icon2\":\"ffab3c\",\"level\":16,\"tier\":6,\"minRating\":1400,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1200},{\"name\":\"Diamond III\",\"locID\":\"11202621\",\"icon\":\"\\\\Images\\\\multiplayer\\\\diamond_3.png\",\"icon2\":\"699dfd\",\"level\":15,\"tier\":5,\"minRating\":1350,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1199},{\"name\":\"Diamond II\",\"locID\":\"11202622\",\"icon\":\"\\\\Images\\\\multiplayer\\\\diamond_2.png\",\"icon2\":\"699dfd\",\"level\":14,\"tier\":5,\"minRating\":1300,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1199},{\"name\":\"Diamond I\",\"locID\":\"11202623\",\"icon\":\"\\\\Images\\\\multiplayer\\\\diamond_1.png\",\"icon2\":\"699dfd\",\"level\":13,\"tier\":5,\"minRating\":1200,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1199},{\"name\":\"Platinum III\",\"locID\":\"11202618\",\"icon\":\"\\\\Images\\\\multiplayer\\\\platinum_3.png\",\"icon2\":\"65a1c4\",\"level\":12,\"tier\":4,\"minRating\":1150,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1198},{\"name\":\"Platinum II\",\"locID\":\"11202619\",\"icon\":\"\\\\Images\\\\multiplayer\\\\platinum_2.png\",\"icon2\":\"65a1c4\",\"level\":11,\"tier\":4,\"minRating\":1100,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1198},{\"name\":\"Platinum I\",\"locID\":\"11202620\",\"icon\":\"\\\\Images\\\\multiplayer\\\\platinum_1.png\",\"icon2\":\"65a1c4\",\"level\":10,\"tier\":4,\"minRating\":1000,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1198},{\"name\":\"Gold III\",\"locID\":\"11202615\",\"icon\":\"\\\\Images\\\\multiplayer\\\\gold_3.png\",\"icon2\":\"ffd469\",\"level\":9,\"tier\":3,\"minRating\":900,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1197},{\"name\":\"Gold II\",\"locID\":\"11202616\",\"icon\":\"\\\\Images\\\\multiplayer\\\\gold_2.png\",\"icon2\":\"ffd469\",\"level\":8,\"tier\":3,\"minRating\":800,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1197},{\"name\":\"Gold I\",\"locID\":\"11202617\",\"icon\":\"\\\\Images\\\\multiplayer\\\\gold_1.png\",\"icon2\":\"ffd469\",\"level\":7,\"tier\":3,\"minRating\":700,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1197},{\"name\":\"Silver III\",\"locID\":\"11202612\",\"icon\":\"\\\\Images\\\\multiplayer\\\\silver_3.png\",\"icon2\":\"a7aebb\",\"level\":6,\"tier\":2,\"minRating\":650,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1196},{\"name\":\"Silver II\",\"locID\":\"11202613\",\"icon\":\"\\\\Images\\\\multiplayer\\\\silver_2.png\",\"icon2\":\"a7aebb\",\"level\":5,\"tier\":2,\"minRating\":600,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1196},{\"name\":\"Silver I\",\"locID\":\"11202614\",\"icon\":\"\\\\Images\\\\multiplayer\\\\silver_1.png\",\"icon2\":\"a7aebb\",\"level\":4,\"tier\":2,\"minRating\":500,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1196},{\"name\":\"Bronze III\",\"locID\":\"11202608\",\"icon\":\"\\\\Images\\\\multiplayer\\\\bronze_3.png\",\"icon2\":\"9d6242\",\"level\":3,\"tier\":1,\"minRating\":450,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1195},{\"name\":\"Bronze II\",\"locID\":\"11202609\",\"icon\":\"\\\\Images\\\\multiplayer\\\\bronze_2.png\",\"icon2\":\"9d6242\",\"level\":2,\"tier\":1,\"minRating\":400,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1195},{\"name\":\"Bronze I\",\"locID\":\"11202610\",\"icon\":\"\\\\Images\\\\multiplayer\\\\bronze_1.png\",\"icon2\":\"9d6242\",\"level\":1,\"tier\":1,\"minRating\":0,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1195}]},\"pointUpdate\":{\"winPtsDefault\":0,\"losePtsDefault\":0,\"maxWinPts\":45,\"minWinPts\":2,\"maxLosePts\":45,\"minLosePts\":4,\"bonusPtsPerDay\":5,\"maxPtsAllowBonus\":2400,\"maxWinPtsWithBonus\":10,\"maxBonusPtsDefault\":5,\"placementMatch\":5,\"adjustmentOnWinPlacementAbs\":\"0.175\",\"adjustmentOnLosePlacementAbs\":\"0.1\",\"adjustmentOnWinPlacementRel\":\"0.02\",\"adjustmentOnLosePlacementRel\":\"0.02\",\"adjustmentOnWinDefault\":\"0.05\",\"adjustmentOnLoseDefault\":\"0.05\",\"winDifferenceToApply\":100,\"loseDifferenceToApply\":100}}}"
        ],
        [
            "Season 3 - Team Ranked Season",
            1666804500,
            1676534340,
            1893484800,
            32,
            6,
            "Season 3",
            "{\"leaderboard\":{\"leaderboards\":[{\"name\":\"Season 3 Team\",\"scoringType\":2,\"visibleToPublic\":true,\"mapEntries\":[{\"matchType\":2,\"race\":-1,\"statGroupType\":1},{\"matchType\":3,\"race\":-1,\"statGroupType\":1},{\"matchType\":4,\"race\":-1,\"statGroupType\":1}]}],\"decay\":{\"reqRating\":1400,\"minDays\":15,\"amountPerDay\":5,\"maxAmount\":200},\"rankLevels\":{\"customRanks\":[{\"name\":\"Conqueror III\",\"locID\":\"11202624\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_conquerer_3.png\",\"icon2\":\"ffab3c\",\"level\":18,\"tier\":6,\"minRating\":1600,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1206},{\"name\":\"Conqueror II\",\"locID\":\"11202625\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_conquerer_2.png\",\"icon2\":\"ffab3c\",\"level\":17,\"tier\":6,\"minRating\":1500,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1206},{\"name\":\"Conqueror I\",\"locID\":\"11202626\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_conquerer_1.png\",\"icon2\":\"ffab3c\",\"level\":16,\"tier\":6,\"minRating\":1400,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1206},{\"name\":\"Diamond III\",\"locID\":\"11202621\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_diamond_3.png\",\"icon2\":\"699dfd\",\"level\":15,\"tier\":5,\"minRating\":1350,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1205},{\"name\":\"Diamond II\",\"locID\":\"11202622\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_diamond_2.png\",\"icon2\":\"699dfd\",\"level\":14,\"tier\":5,\"minRating\":1300,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1205},{\"name\":\"Diamond I\",\"locID\":\"11202623\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_diamond_1.png\",\"icon2\":\"699dfd\",\"level\":13,\"tier\":5,\"minRating\":1200,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1205},{\"name\":\"Platinum III\",\"locID\":\"11202618\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_platinum_3.png\",\"icon2\":\"65a1c4\",\"level\":12,\"tier\":4,\"minRating\":1150,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1204},{\"name\":\"Platinum II\",\"locID\":\"11202619\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_platinum_2.png\",\"icon2\":\"65a1c4\",\"level\":11,\"tier\":4,\"minRating\":1100,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1204},{\"name\":\"Platinum I\",\"locID\":\"11202620\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_platinum_1.png\",\"icon2\":\"65a1c4\",\"level\":10,\"tier\":4,\"minRating\":1000,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1204},{\"name\":\"Gold III\",\"locID\":\"11202615\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_gold_3.png\",\"icon2\":\"ffd469\",\"level\":9,\"tier\":3,\"minRating\":900,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1203},{\"name\":\"Gold II\",\"locID\":\"11202616\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_gold_2.png\",\"icon2\":\"ffd469\",\"level\":8,\"tier\":3,\"minRating\":800,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1203},{\"name\":\"Gold I\",\"locID\":\"11202617\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_gold_1.png\",\"icon2\":\"ffd469\",\"level\":7,\"tier\":3,\"minRating\":700,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1203},{\"name\":\"Silver III\",\"locID\":\"11202612\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_silver_3.png\",\"icon2\":\"a7aebb\",\"level\":6,\"tier\":2,\"minRating\":650,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1202},{\"name\":\"Silver II\",\"locID\":\"11202613\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_silver_2.png\",\"icon2\":\"a7aebb\",\"level\":5,\"tier\":2,\"minRating\":600,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1202},{\"name\":\"Silver I\",\"locID\":\"11202614\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_silver_1.png\",\"icon2\":\"a7aebb\",\"level\":4,\"tier\":2,\"minRating\":500,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1202},{\"name\":\"Bronze III\",\"locID\":\"11202608\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_bronze_3.png\",\"icon2\":\"9d6242\",\"level\":3,\"tier\":1,\"minRating\":450,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1201},{\"name\":\"Bronze II\",\"locID\":\"11202609\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_bronze_2.png\",\"icon2\":\"9d6242\",\"level\":2,\"tier\":1,\"minRating\":400,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1201},{\"name\":\"Bronze I\",\"locID\":\"11202610\",\"icon\":\"\\\\Images\\\\multiplayer\\\\team_bronze_1.png\",\"icon2\":\"9d6242\",\"level\":1,\"tier\":1,\"minRating\":0,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1201}]},\"pointUpdate\":{\"winPtsDefault\":0,\"losePtsDefault\":0,\"maxWinPts\":45,\"minWinPts\":2,\"maxLosePts\":45,\"minLosePts\":4,\"bonusPtsPerDay\":5,\"maxPtsAllowBonus\":2400,\"maxWinPtsWithBonus\":10,\"maxBonusPtsDefault\":5,\"placementMatch\":5,\"adjustmentOnWinPlacementAbs\":\"0.175\",\"adjustmentOnLosePlacementAbs\":\"0.1\",\"adjustmentOnWinPlacementRel\":\"0.02\",\"adjustmentOnLosePlacementRel\":\"0.02\",\"adjustmentOnWinDefault\":\"0.05\",\"adjustmentOnLoseDefault\":\"0.05\",\"winDifferenceToApply\":100,\"loseDifferenceToApply\":100}}}"
        ],
        [
            "Season 1 - Ranked Season - Festival of Ages",
            1649869200,
            1656608400,
            1893484800,
            3,
            6,
            "Season 1",
            "{\"leaderboard\":{\"leaderboards\":[{\"copyFromBase\":1,\"scoringType\":2}],\"decay\":{\"reqRating\":1015,\"minDays\":15,\"amountPerDay\":5,\"maxAmount\":200},\"rankLevels\":{\"customRanks\":[{\"name\":\"Conqueror III\",\"locID\":\"11202624\",\"icon\":\"\\\\Images\\\\multiplayer\\\\conquerer_3.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":18,\"tier\":6,\"minRating\":1600,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1059},{\"name\":\"Conqueror II\",\"locID\":\"11202625\",\"icon\":\"\\\\Images\\\\multiplayer\\\\conquerer_2.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":17,\"tier\":6,\"minRating\":1500,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1059},{\"name\":\"Conqueror I\",\"locID\":\"11202626\",\"icon\":\"\\\\Images\\\\multiplayer\\\\conquerer_1.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":16,\"tier\":6,\"minRating\":1400,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1059},{\"name\":\"Diamond III\",\"locID\":\"11202621\",\"icon\":\"\\\\Images\\\\multiplayer\\\\diamond_3.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":15,\"tier\":5,\"minRating\":1300,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1060},{\"name\":\"Diamond II\",\"locID\":\"11202622\",\"icon\":\"\\\\Images\\\\multiplayer\\\\diamond_2.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":14,\"tier\":5,\"minRating\":1230,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1060},{\"name\":\"Diamond I\",\"locID\":\"11202623\",\"icon\":\"\\\\Images\\\\multiplayer\\\\diamond_1.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":13,\"tier\":5,\"minRating\":1130,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1060},{\"name\":\"Platinum III\",\"locID\":\"11202618\",\"icon\":\"\\\\Images\\\\multiplayer\\\\platinum_3.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":12,\"tier\":4,\"minRating\":1090,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1062},{\"name\":\"Platinum II\",\"locID\":\"11202619\",\"icon\":\"\\\\Images\\\\multiplayer\\\\platinum_2.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":11,\"tier\":4,\"minRating\":1050,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1062},{\"name\":\"Platinum I\",\"locID\":\"11202620\",\"icon\":\"\\\\Images\\\\multiplayer\\\\platinum_1.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":10,\"tier\":4,\"minRating\":1015,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1062},{\"name\":\"Gold III\",\"locID\":\"11202615\",\"icon\":\"\\\\Images\\\\multiplayer\\\\gold_3.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":9,\"tier\":3,\"minRating\":980,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1061},{\"name\":\"Gold II\",\"locID\":\"11202616\",\"icon\":\"\\\\Images\\\\multiplayer\\\\gold_2.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":8,\"tier\":3,\"minRating\":930,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1061},{\"name\":\"Gold I\",\"locID\":\"11202617\",\"icon\":\"\\\\Images\\\\multiplayer\\\\gold_1.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":7,\"tier\":3,\"minRating\":880,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1061},{\"name\":\"Silver III\",\"locID\":\"11202612\",\"icon\":\"\\\\Images\\\\multiplayer\\\\silver_3.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":6,\"tier\":2,\"minRating\":840,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1063},{\"name\":\"Silver II\",\"locID\":\"11202613\",\"icon\":\"\\\\Images\\\\multiplayer\\\\silver_2.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":5,\"tier\":2,\"minRating\":800,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1063},{\"name\":\"Silver I\",\"locID\":\"11202614\",\"icon\":\"\\\\Images\\\\multiplayer\\\\silver_1.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":4,\"tier\":2,\"minRating\":770,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1063},{\"name\":\"Bronze III\",\"locID\":\"11202608\",\"icon\":\"\\\\Images\\\\multiplayer\\\\bronze_3.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":3,\"tier\":1,\"minRating\":600,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1058},{\"name\":\"Bronze II\",\"locID\":\"11202609\",\"icon\":\"\\\\Images\\\\multiplayer\\\\bronze_2.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":2,\"tier\":1,\"minRating\":400,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1058},{\"name\":\"Bronze I\",\"locID\":\"11202610\",\"icon\":\"\\\\Images\\\\multiplayer\\\\bronze_1.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":1,\"tier\":1,\"minRating\":0,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1058}]},\"pointUpdate\":{\"winPtsDefault\":3,\"losePtsDefault\":0,\"maxWinPts\":65,\"minWinPts\":10,\"maxLosePts\":45,\"minLosePts\":5,\"maxWinChance\":\"0.8\",\"bonusPtsPerDay\":5,\"maxPtsAllowBonus\":2400,\"maxWinPtsWithBonus\":10,\"maxBonusPtsDefault\":5,\"placementMatch\":5,\"adjustmentOnWinPlacementAbs\":\"0.175\",\"adjustmentOnLosePlacementAbs\":\"0.1\",\"adjustmentOnWinPlacementRel\":\"0.02\",\"adjustmentOnLosePlacementRel\":\"0.02\",\"adjustmentOnWinDefault\":\"0.09\",\"adjustmentOnLoseDefault\":\"0.06\",\"winDifferenceToApply\":250,\"loseDifferenceToApply\":250}}}"
        ],
        [
            "Season 2 - Ranked Season - Map Monsters",
            1657818000,
            1666681200,
            1893484800,
            15,
            6,
            "Season 2",
            "{\"leaderboard\":{\"leaderboards\":[{\"copyFromBase\":1,\"scoringType\":2}],\"decay\":{\"reqRating\":1400,\"minDays\":15,\"amountPerDay\":5,\"maxAmount\":200},\"rankLevels\":{\"customRanks\":[{\"name\":\"Conqueror III\",\"locID\":\"11202624\",\"icon\":\"\\\\Images\\\\multiplayer\\\\conquerer_3.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":18,\"tier\":6,\"minRating\":1600,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1131},{\"name\":\"Conqueror II\",\"locID\":\"11202625\",\"icon\":\"\\\\Images\\\\multiplayer\\\\conquerer_2.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":17,\"tier\":6,\"minRating\":1500,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1131},{\"name\":\"Conqueror I\",\"locID\":\"11202626\",\"icon\":\"\\\\Images\\\\multiplayer\\\\conquerer_1.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":16,\"tier\":6,\"minRating\":1400,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1131},{\"name\":\"Diamond III\",\"locID\":\"11202621\",\"icon\":\"\\\\Images\\\\multiplayer\\\\diamond_3.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":15,\"tier\":5,\"minRating\":1350,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1132},{\"name\":\"Diamond II\",\"locID\":\"11202622\",\"icon\":\"\\\\Images\\\\multiplayer\\\\diamond_2.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":14,\"tier\":5,\"minRating\":1300,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1132},{\"name\":\"Diamond I\",\"locID\":\"11202623\",\"icon\":\"\\\\Images\\\\multiplayer\\\\diamond_1.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":13,\"tier\":5,\"minRating\":1200,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1132},{\"name\":\"Platinum III\",\"locID\":\"11202618\",\"icon\":\"\\\\Images\\\\multiplayer\\\\platinum_3.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":12,\"tier\":4,\"minRating\":1150,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1134},{\"name\":\"Platinum II\",\"locID\":\"11202619\",\"icon\":\"\\\\Images\\\\multiplayer\\\\platinum_2.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":11,\"tier\":4,\"minRating\":1100,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1134},{\"name\":\"Platinum I\",\"locID\":\"11202620\",\"icon\":\"\\\\Images\\\\multiplayer\\\\platinum_1.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":10,\"tier\":4,\"minRating\":1000,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1134},{\"name\":\"Gold III\",\"locID\":\"11202615\",\"icon\":\"\\\\Images\\\\multiplayer\\\\gold_3.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":9,\"tier\":3,\"minRating\":900,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1133},{\"name\":\"Gold II\",\"locID\":\"11202616\",\"icon\":\"\\\\Images\\\\multiplayer\\\\gold_2.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":8,\"tier\":3,\"minRating\":800,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1133},{\"name\":\"Gold I\",\"locID\":\"11202617\",\"icon\":\"\\\\Images\\\\multiplayer\\\\gold_1.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":7,\"tier\":3,\"minRating\":700,\"maxRanking\":100,\"rankingType\":1,\"itemBundleID\":1133},{\"name\":\"Silver III\",\"locID\":\"11202612\",\"icon\":\"\\\\Images\\\\multiplayer\\\\silver_3.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":6,\"tier\":2,\"minRating\":650,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1135},{\"name\":\"Silver II\",\"locID\":\"11202613\",\"icon\":\"\\\\Images\\\\multiplayer\\\\silver_2.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":5,\"tier\":2,\"minRating\":600,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1135},{\"name\":\"Silver I\",\"locID\":\"11202614\",\"icon\":\"\\\\Images\\\\multiplayer\\\\silver_1.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow_blue.png\",\"level\":4,\"tier\":2,\"minRating\":500,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1135},{\"name\":\"Bronze III\",\"locID\":\"11202608\",\"icon\":\"\\\\Images\\\\multiplayer\\\\bronze_3.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":3,\"tier\":1,\"minRating\":450,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1130},{\"name\":\"Bronze II\",\"locID\":\"11202609\",\"icon\":\"\\\\Images\\\\multiplayer\\\\bronze_2.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":2,\"tier\":1,\"minRating\":400,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1130},{\"name\":\"Bronze I\",\"locID\":\"11202610\",\"icon\":\"\\\\Images\\\\multiplayer\\\\bronze_1.png\",\"icon2\":\"\\\\Images\\\\multiplayer\\\\rank_glow.png\",\"level\":1,\"tier\":1,\"minRating\":0,\"maxRanking\":100,\"maxBonusPts\":100,\"rankingType\":1,\"itemBundleID\":1130}]},\"pointUpdate\":{\"winPtsDefault\":0,\"losePtsDefault\":0,\"maxWinPts\":45,\"minWinPts\":2,\"maxLosePts\":45,\"minLosePts\":4,\"maxWinChance\":\"0.8\",\"bonusPtsPerDay\":5,\"maxPtsAllowBonus\":2400,\"maxWinPtsWithBonus\":10,\"maxBonusPtsDefault\":5,\"placementMatch\":5,\"adjustmentOnWinPlacementAbs\":\"0.175\",\"adjustmentOnLosePlacementAbs\":\"0.1\",\"adjustmentOnWinPlacementRel\":\"0.02\",\"adjustmentOnLosePlacementRel\":\"0.02\",\"adjustmentOnWinDefault\":\"0.05\",\"adjustmentOnLoseDefault\":\"0.05\",\"winDifferenceToApply\":100,\"loseDifferenceToApply\":100}}}"
        ]
    ]
]
```
