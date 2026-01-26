# [GET] /game/CommunityEvent/getAvailableCommunityEvents

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/CommunityEvent/getAvailableCommunityEvents?callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
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
[
    0,
    [],
    [],
    [],
    [],
    [],
    []
]
```

## AoE3:DE

### Request

```
GET /game/CommunityEvent/getAvailableCommunityEvents?callNum=2&connect_id=fflxvvhtmtcx7tmbxff2kauyfdq8n3&lastCallTime=533&sessionID=fflxvvhtmtcx7tmbxff2kauyfdq8n3 HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: deflate, gzip
Cookie: ApplicationGatewayAffinity=29259ca9e836dd7648ed1ca403a17cde;ApplicationGatewayAffinityCORS=29259ca9e836dd7648ed1ca403a17cde;worldsedgelink=-1321719403;
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
            "Ageiversary 2022",
            1666720800,
            1669017600,
            1669017600,
            15,
            1,
            "{ \"name\": 55729, \"priority\" : 1 }"
        ]
    ],
    []
]
```

## AoE4

### Request

```
GET /game/CommunityEvent/getAvailableCommunityEvents?callNum=2&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=727&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19 HTTP/1.1
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
    ],
    [
        [
            21,
            22,
            -1,
            6,
            1525307,
            "{\"challenge\":[{\"periodBegin\":1666691400000,\"slot\":5,\"definitionID\":[1525309,1525311,1525313,1525315,1525329,1525331]}]}"
        ],
        [
            23,
            24,
            -1,
            1,
            1174,
            ""
        ],
        [
            24,
            25,
            -1,
            1,
            1175,
            ""
        ],
        [
            3,
            3,
            -1,
            5,
            -1,
            ""
        ],
        [
            25,
            26,
            -1,
            1,
            1176,
            ""
        ],
        [
            14,
            15,
            -1,
            5,
            -1,
            ""
        ],
        [
            29,
            31,
            -1,
            5,
            -1,
            ""
        ],
        [
            30,
            32,
            -1,
            5,
            -1,
            ""
        ]
    ],
    [],
    [
        [
            3,
            1,
            "Season 1 - Ranked Season - Festival of Ages_Slot1_1v1Ranked",
            1,
            2
        ],
        [
            15,
            2,
            "Season 2 - Ranked Season - Map Monsters_Slot1_1v1Ranked",
            1,
            2
        ],
        [
            31,
            5,
            "Season 3 - Solo Ranked Season_Slot1_1v1Ranked",
            1,
            2
        ],
        [
            32,
            6,
            "Season 3 - Team Ranked Season_Season 3 Team",
            1,
            2
        ]
    ],
    [
        [
            1,
            1,
            1,
            -1,
            3
        ],
        [
            2,
            1,
            1,
            -1,
            15
        ],
        [
            5,
            1,
            1,
            -1,
            31
        ],
        [
            6,
            2,
            1,
            -1,
            32
        ],
        [
            6,
            3,
            1,
            -1,
            32
        ],
        [
            6,
            4,
            1,
            -1,
            32
        ]
    ],
    [
        [
            1,
            -1,
            "Bronze I",
            0,
            100,
            "\\Images\\multiplayer\\bronze_1.png",
            1,
            "Bronze I",
            null,
            1,
            "\\Images\\multiplayer\\rank_glow.png",
            3,
            1058
        ],
        [
            2,
            -1,
            "Bronze II",
            400,
            100,
            "\\Images\\multiplayer\\bronze_2.png",
            1,
            "Bronze II",
            null,
            1,
            "\\Images\\multiplayer\\rank_glow.png",
            3,
            1058
        ],
        [
            3,
            -1,
            "Bronze III",
            600,
            100,
            "\\Images\\multiplayer\\bronze_3.png",
            1,
            "Bronze III",
            null,
            1,
            "\\Images\\multiplayer\\rank_glow.png",
            3,
            1058
        ],
        [
            4,
            -1,
            "Silver I",
            770,
            100,
            "\\Images\\multiplayer\\silver_1.png",
            1,
            "Silver I",
            null,
            2,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            3,
            1063
        ],
        [
            5,
            -1,
            "Silver II",
            800,
            100,
            "\\Images\\multiplayer\\silver_2.png",
            1,
            "Silver II",
            null,
            2,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            3,
            1063
        ],
        [
            6,
            -1,
            "Silver III",
            840,
            100,
            "\\Images\\multiplayer\\silver_3.png",
            1,
            "Silver III",
            null,
            2,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            3,
            1063
        ],
        [
            7,
            -1,
            "Gold I",
            880,
            100,
            "\\Images\\multiplayer\\gold_1.png",
            1,
            "Gold I",
            null,
            3,
            "\\Images\\multiplayer\\rank_glow.png",
            3,
            1061
        ],
        [
            8,
            -1,
            "Gold II",
            930,
            100,
            "\\Images\\multiplayer\\gold_2.png",
            1,
            "Gold II",
            null,
            3,
            "\\Images\\multiplayer\\rank_glow.png",
            3,
            1061
        ],
        [
            9,
            -1,
            "Gold III",
            980,
            100,
            "\\Images\\multiplayer\\gold_3.png",
            1,
            "Gold III",
            null,
            3,
            "\\Images\\multiplayer\\rank_glow.png",
            3,
            1061
        ],
        [
            10,
            -1,
            "Platinum I",
            1015,
            100,
            "\\Images\\multiplayer\\platinum_1.png",
            1,
            "Platinum I",
            null,
            4,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            3,
            1062
        ],
        [
            11,
            -1,
            "Platinum II",
            1050,
            100,
            "\\Images\\multiplayer\\platinum_2.png",
            1,
            "Platinum II",
            null,
            4,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            3,
            1062
        ],
        [
            12,
            -1,
            "Platinum III",
            1090,
            100,
            "\\Images\\multiplayer\\platinum_3.png",
            1,
            "Platinum III",
            null,
            4,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            3,
            1062
        ],
        [
            13,
            -1,
            "Diamond I",
            1130,
            100,
            "\\Images\\multiplayer\\diamond_1.png",
            1,
            "Diamond I",
            null,
            5,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            3,
            1060
        ],
        [
            14,
            -1,
            "Diamond II",
            1230,
            100,
            "\\Images\\multiplayer\\diamond_2.png",
            1,
            "Diamond II",
            null,
            5,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            3,
            1060
        ],
        [
            15,
            -1,
            "Diamond III",
            1300,
            100,
            "\\Images\\multiplayer\\diamond_3.png",
            1,
            "Diamond III",
            null,
            5,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            3,
            1060
        ],
        [
            16,
            -1,
            "Conqueror I",
            1400,
            100,
            "\\Images\\multiplayer\\conquerer_1.png",
            1,
            "Conqueror I",
            null,
            6,
            "\\Images\\multiplayer\\rank_glow.png",
            3,
            1059
        ],
        [
            17,
            -1,
            "Conqueror II",
            1500,
            100,
            "\\Images\\multiplayer\\conquerer_2.png",
            1,
            "Conqueror II",
            null,
            6,
            "\\Images\\multiplayer\\rank_glow.png",
            3,
            1059
        ],
        [
            18,
            -1,
            "Conqueror III",
            1600,
            100,
            "\\Images\\multiplayer\\conquerer_3.png",
            1,
            "Conqueror III",
            null,
            6,
            "\\Images\\multiplayer\\rank_glow.png",
            3,
            1059
        ],
        [
            1,
            -1,
            "Bronze I",
            0,
            100,
            "\\Images\\multiplayer\\bronze_1.png",
            1,
            "Bronze I",
            null,
            1,
            "\\Images\\multiplayer\\rank_glow.png",
            15,
            1130
        ],
        [
            2,
            -1,
            "Bronze II",
            400,
            100,
            "\\Images\\multiplayer\\bronze_2.png",
            1,
            "Bronze II",
            null,
            1,
            "\\Images\\multiplayer\\rank_glow.png",
            15,
            1130
        ],
        [
            3,
            -1,
            "Bronze III",
            450,
            100,
            "\\Images\\multiplayer\\bronze_3.png",
            1,
            "Bronze III",
            null,
            1,
            "\\Images\\multiplayer\\rank_glow.png",
            15,
            1130
        ],
        [
            4,
            -1,
            "Silver I",
            500,
            100,
            "\\Images\\multiplayer\\silver_1.png",
            1,
            "Silver I",
            null,
            2,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            15,
            1135
        ],
        [
            5,
            -1,
            "Silver II",
            600,
            100,
            "\\Images\\multiplayer\\silver_2.png",
            1,
            "Silver II",
            null,
            2,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            15,
            1135
        ],
        [
            6,
            -1,
            "Silver III",
            650,
            100,
            "\\Images\\multiplayer\\silver_3.png",
            1,
            "Silver III",
            null,
            2,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            15,
            1135
        ],
        [
            7,
            -1,
            "Gold I",
            700,
            100,
            "\\Images\\multiplayer\\gold_1.png",
            1,
            "Gold I",
            null,
            3,
            "\\Images\\multiplayer\\rank_glow.png",
            15,
            1133
        ],
        [
            8,
            -1,
            "Gold II",
            800,
            100,
            "\\Images\\multiplayer\\gold_2.png",
            1,
            "Gold II",
            null,
            3,
            "\\Images\\multiplayer\\rank_glow.png",
            15,
            1133
        ],
        [
            9,
            -1,
            "Gold III",
            900,
            100,
            "\\Images\\multiplayer\\gold_3.png",
            1,
            "Gold III",
            null,
            3,
            "\\Images\\multiplayer\\rank_glow.png",
            15,
            1133
        ],
        [
            10,
            -1,
            "Platinum I",
            1000,
            100,
            "\\Images\\multiplayer\\platinum_1.png",
            1,
            "Platinum I",
            null,
            4,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            15,
            1134
        ],
        [
            11,
            -1,
            "Platinum II",
            1100,
            100,
            "\\Images\\multiplayer\\platinum_2.png",
            1,
            "Platinum II",
            null,
            4,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            15,
            1134
        ],
        [
            12,
            -1,
            "Platinum III",
            1150,
            100,
            "\\Images\\multiplayer\\platinum_3.png",
            1,
            "Platinum III",
            null,
            4,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            15,
            1134
        ],
        [
            13,
            -1,
            "Diamond I",
            1200,
            100,
            "\\Images\\multiplayer\\diamond_1.png",
            1,
            "Diamond I",
            null,
            5,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            15,
            1132
        ],
        [
            14,
            -1,
            "Diamond II",
            1300,
            100,
            "\\Images\\multiplayer\\diamond_2.png",
            1,
            "Diamond II",
            null,
            5,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            15,
            1132
        ],
        [
            15,
            -1,
            "Diamond III",
            1350,
            100,
            "\\Images\\multiplayer\\diamond_3.png",
            1,
            "Diamond III",
            null,
            5,
            "\\Images\\multiplayer\\rank_glow_blue.png",
            15,
            1132
        ],
        [
            16,
            -1,
            "Conqueror I",
            1400,
            100,
            "\\Images\\multiplayer\\conquerer_1.png",
            1,
            "Conqueror I",
            null,
            6,
            "\\Images\\multiplayer\\rank_glow.png",
            15,
            1131
        ],
        [
            17,
            -1,
            "Conqueror II",
            1500,
            100,
            "\\Images\\multiplayer\\conquerer_2.png",
            1,
            "Conqueror II",
            null,
            6,
            "\\Images\\multiplayer\\rank_glow.png",
            15,
            1131
        ],
        [
            18,
            -1,
            "Conqueror III",
            1600,
            100,
            "\\Images\\multiplayer\\conquerer_3.png",
            1,
            "Conqueror III",
            null,
            6,
            "\\Images\\multiplayer\\rank_glow.png",
            15,
            1131
        ],
        [
            1,
            -1,
            "Bronze I",
            0,
            100,
            "\\Images\\multiplayer\\bronze_1.png",
            1,
            "Bronze I",
            null,
            1,
            "9d6242",
            31,
            1195
        ],
        [
            2,
            -1,
            "Bronze II",
            400,
            100,
            "\\Images\\multiplayer\\bronze_2.png",
            1,
            "Bronze II",
            null,
            1,
            "9d6242",
            31,
            1195
        ],
        [
            3,
            -1,
            "Bronze III",
            450,
            100,
            "\\Images\\multiplayer\\bronze_3.png",
            1,
            "Bronze III",
            null,
            1,
            "9d6242",
            31,
            1195
        ],
        [
            4,
            -1,
            "Silver I",
            500,
            100,
            "\\Images\\multiplayer\\silver_1.png",
            1,
            "Silver I",
            null,
            2,
            "a7aebb",
            31,
            1196
        ],
        [
            5,
            -1,
            "Silver II",
            600,
            100,
            "\\Images\\multiplayer\\silver_2.png",
            1,
            "Silver II",
            null,
            2,
            "a7aebb",
            31,
            1196
        ],
        [
            6,
            -1,
            "Silver III",
            650,
            100,
            "\\Images\\multiplayer\\silver_3.png",
            1,
            "Silver III",
            null,
            2,
            "a7aebb",
            31,
            1196
        ],
        [
            7,
            -1,
            "Gold I",
            700,
            100,
            "\\Images\\multiplayer\\gold_1.png",
            1,
            "Gold I",
            null,
            3,
            "ffd469",
            31,
            1197
        ],
        [
            8,
            -1,
            "Gold II",
            800,
            100,
            "\\Images\\multiplayer\\gold_2.png",
            1,
            "Gold II",
            null,
            3,
            "ffd469",
            31,
            1197
        ],
        [
            9,
            -1,
            "Gold III",
            900,
            100,
            "\\Images\\multiplayer\\gold_3.png",
            1,
            "Gold III",
            null,
            3,
            "ffd469",
            31,
            1197
        ],
        [
            10,
            -1,
            "Platinum I",
            1000,
            100,
            "\\Images\\multiplayer\\platinum_1.png",
            1,
            "Platinum I",
            null,
            4,
            "65a1c4",
            31,
            1198
        ],
        [
            11,
            -1,
            "Platinum II",
            1100,
            100,
            "\\Images\\multiplayer\\platinum_2.png",
            1,
            "Platinum II",
            null,
            4,
            "65a1c4",
            31,
            1198
        ],
        [
            12,
            -1,
            "Platinum III",
            1150,
            100,
            "\\Images\\multiplayer\\platinum_3.png",
            1,
            "Platinum III",
            null,
            4,
            "65a1c4",
            31,
            1198
        ],
        [
            13,
            -1,
            "Diamond I",
            1200,
            100,
            "\\Images\\multiplayer\\diamond_1.png",
            1,
            "Diamond I",
            null,
            5,
            "699dfd",
            31,
            1199
        ],
        [
            14,
            -1,
            "Diamond II",
            1300,
            100,
            "\\Images\\multiplayer\\diamond_2.png",
            1,
            "Diamond II",
            null,
            5,
            "699dfd",
            31,
            1199
        ],
        [
            15,
            -1,
            "Diamond III",
            1350,
            100,
            "\\Images\\multiplayer\\diamond_3.png",
            1,
            "Diamond III",
            null,
            5,
            "699dfd",
            31,
            1199
        ],
        [
            16,
            -1,
            "Conqueror I",
            1400,
            100,
            "\\Images\\multiplayer\\conquerer_1.png",
            1,
            "Conqueror I",
            null,
            6,
            "ffab3c",
            31,
            1200
        ],
        [
            17,
            -1,
            "Conqueror II",
            1500,
            100,
            "\\Images\\multiplayer\\conquerer_2.png",
            1,
            "Conqueror II",
            null,
            6,
            "ffab3c",
            31,
            1200
        ],
        [
            18,
            -1,
            "Conqueror III",
            1600,
            100,
            "\\Images\\multiplayer\\conquerer_3.png",
            1,
            "Conqueror III",
            null,
            6,
            "ffab3c",
            31,
            1200
        ],
        [
            1,
            -1,
            "Bronze I",
            0,
            100,
            "\\Images\\multiplayer\\team_bronze_1.png",
            1,
            "Bronze I",
            null,
            1,
            "9d6242",
            32,
            1201
        ],
        [
            2,
            -1,
            "Bronze II",
            400,
            100,
            "\\Images\\multiplayer\\team_bronze_2.png",
            1,
            "Bronze II",
            null,
            1,
            "9d6242",
            32,
            1201
        ],
        [
            3,
            -1,
            "Bronze III",
            450,
            100,
            "\\Images\\multiplayer\\team_bronze_3.png",
            1,
            "Bronze III",
            null,
            1,
            "9d6242",
            32,
            1201
        ],
        [
            4,
            -1,
            "Silver I",
            500,
            100,
            "\\Images\\multiplayer\\team_silver_1.png",
            1,
            "Silver I",
            null,
            2,
            "a7aebb",
            32,
            1202
        ],
        [
            5,
            -1,
            "Silver II",
            600,
            100,
            "\\Images\\multiplayer\\team_silver_2.png",
            1,
            "Silver II",
            null,
            2,
            "a7aebb",
            32,
            1202
        ],
        [
            6,
            -1,
            "Silver III",
            650,
            100,
            "\\Images\\multiplayer\\team_silver_3.png",
            1,
            "Silver III",
            null,
            2,
            "a7aebb",
            32,
            1202
        ],
        [
            7,
            -1,
            "Gold I",
            700,
            100,
            "\\Images\\multiplayer\\team_gold_1.png",
            1,
            "Gold I",
            null,
            3,
            "ffd469",
            32,
            1203
        ],
        [
            8,
            -1,
            "Gold II",
            800,
            100,
            "\\Images\\multiplayer\\team_gold_2.png",
            1,
            "Gold II",
            null,
            3,
            "ffd469",
            32,
            1203
        ],
        [
            9,
            -1,
            "Gold III",
            900,
            100,
            "\\Images\\multiplayer\\team_gold_3.png",
            1,
            "Gold III",
            null,
            3,
            "ffd469",
            32,
            1203
        ],
        [
            10,
            -1,
            "Platinum I",
            1000,
            100,
            "\\Images\\multiplayer\\team_platinum_1.png",
            1,
            "Platinum I",
            null,
            4,
            "65a1c4",
            32,
            1204
        ],
        [
            11,
            -1,
            "Platinum II",
            1100,
            100,
            "\\Images\\multiplayer\\team_platinum_2.png",
            1,
            "Platinum II",
            null,
            4,
            "65a1c4",
            32,
            1204
        ],
        [
            12,
            -1,
            "Platinum III",
            1150,
            100,
            "\\Images\\multiplayer\\team_platinum_3.png",
            1,
            "Platinum III",
            null,
            4,
            "65a1c4",
            32,
            1204
        ],
        [
            13,
            -1,
            "Diamond I",
            1200,
            100,
            "\\Images\\multiplayer\\team_diamond_1.png",
            1,
            "Diamond I",
            null,
            5,
            "699dfd",
            32,
            1205
        ],
        [
            14,
            -1,
            "Diamond II",
            1300,
            100,
            "\\Images\\multiplayer\\team_diamond_2.png",
            1,
            "Diamond II",
            null,
            5,
            "699dfd",
            32,
            1205
        ],
        [
            15,
            -1,
            "Diamond III",
            1350,
            100,
            "\\Images\\multiplayer\\team_diamond_3.png",
            1,
            "Diamond III",
            null,
            5,
            "699dfd",
            32,
            1205
        ],
        [
            16,
            -1,
            "Conqueror I",
            1400,
            100,
            "\\Images\\multiplayer\\team_conquerer_1.png",
            1,
            "Conqueror I",
            null,
            6,
            "ffab3c",
            32,
            1206
        ],
        [
            17,
            -1,
            "Conqueror II",
            1500,
            100,
            "\\Images\\multiplayer\\team_conquerer_2.png",
            1,
            "Conqueror II",
            null,
            6,
            "ffab3c",
            32,
            1206
        ],
        [
            18,
            -1,
            "Conqueror III",
            1600,
            100,
            "\\Images\\multiplayer\\team_conquerer_3.png",
            1,
            "Conqueror III",
            null,
            6,
            "ffab3c",
            32,
            1206
        ]
    ]
]
```
