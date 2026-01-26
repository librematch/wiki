# [GET] /community/achievement/getAchievements

[Example request](https://aoe-api.worldsedgelink.com/community/achievement/getAchievements?title=age2&profileids=[196240])

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
    "userAchievementsMap": [
        {
            "196240": [
                {
                    "achievement_id": 83,
                    "achieveddate": 1589903767
                },
                {
                    "achievement_id": 109,
                    "achieveddate": 1604004966
                },
                {
                    "achievement_id": 44,
                    "achieveddate": 1604333155
                },
                {
                    "achievement_id": 136,
                    "achieveddate": 1604679159
                },
                {
                    "achievement_id": 128,
                    "achieveddate": 1608661935
                },
                {
                    "achievement_id": 142,
                    "achieveddate": 1611755922
                },
                {
                    "achievement_id": 143,
                    "achieveddate": 1611855029
                },
                {
                    "achievement_id": 144,
                    "achieveddate": 1612122594
                },
                {
                    "achievement_id": 139,
                    "achieveddate": 1612123236
                },
                {
                    "achievement_id": 140,
                    "achieveddate": 1614355800
                },
                {
                    "achievement_id": 148,
                    "achieveddate": 1615119718
                },
                {
                    "achievement_id": 149,
                    "achieveddate": 1615121997
                },
                {
                    "achievement_id": 141,
                    "achieveddate": 1617733467
                },
                {
                    "achievement_id": 133,
                    "achieveddate": 1626186501
                },
                {
                    "achievement_id": 134,
                    "achieveddate": 1626186706
                },
                {
                    "achievement_id": 12,
                    "achieveddate": 1626187672
                },
                {
                    "achievement_id": 45,
                    "achieveddate": 1626187673
                },
                {
                    "achievement_id": 129,
                    "achieveddate": 1626187674
                },
                {
                    "achievement_id": 131,
                    "achieveddate": 1626187733
                },
                {
                    "achievement_id": 115,
                    "achieveddate": 1626188152
                },
                {
                    "achievement_id": 112,
                    "achieveddate": 1626192383
                },
                {
                    "achievement_id": 119,
                    "achieveddate": 1626192638
                },
                {
                    "achievement_id": 15,
                    "achieveddate": 1626633993
                },
                {
                    "achievement_id": 29,
                    "achieveddate": 1626635965
                },
                {
                    "achievement_id": 127,
                    "achieveddate": 1626636927
                },
                {
                    "achievement_id": 31,
                    "achieveddate": 1626637032
                },
                {
                    "achievement_id": 33,
                    "achieveddate": 1626638896
                },
                {
                    "achievement_id": 18,
                    "achieveddate": 1626639657
                },
                {
                    "achievement_id": 23,
                    "achieveddate": 1626641109
                },
                {
                    "achievement_id": 48,
                    "achieveddate": 1626642476
                },
                {
                    "achievement_id": 117,
                    "achieveddate": 1626642476
                },
                {
                    "achievement_id": 19,
                    "achieveddate": 1626642851
                },
                {
                    "achievement_id": 21,
                    "achieveddate": 1626644123
                },
                {
                    "achievement_id": 132,
                    "achieveddate": 1628613360
                },
                {
                    "achievement_id": 170,
                    "achieveddate": 1628614147
                },
                {
                    "achievement_id": 46,
                    "achieveddate": 1628619993
                },
                {
                    "achievement_id": 156,
                    "achieveddate": 1628620589
                },
                {
                    "achievement_id": 157,
                    "achieveddate": 1628869582
                },
                {
                    "achievement_id": 168,
                    "achieveddate": 1628873000
                },
                {
                    "achievement_id": 152,
                    "achieveddate": 1628878560
                },
                {
                    "achievement_id": 17,
                    "achieveddate": 1629303481
                },
                {
                    "achievement_id": 113,
                    "achieveddate": 1629305874
                },
                {
                    "achievement_id": 22,
                    "achieveddate": 1629305907
                },
                {
                    "achievement_id": 5,
                    "achieveddate": 1629307654
                },
                {
                    "achievement_id": 4,
                    "achieveddate": 1629368805
                },
                {
                    "achievement_id": 10,
                    "achieveddate": 1629374144
                },
                {
                    "achievement_id": 35,
                    "achieveddate": 1629375500
                },
                {
                    "achievement_id": 3,
                    "achieveddate": 1629376982
                },
                {
                    "achievement_id": 42,
                    "achieveddate": 1629477458
                },
                {
                    "achievement_id": 27,
                    "achieveddate": 1629479486
                },
                {
                    "achievement_id": 7,
                    "achieveddate": 1629487607
                },
                {
                    "achievement_id": 20,
                    "achieveddate": 1629621159
                },
                {
                    "achievement_id": 24,
                    "achieveddate": 1629624030
                },
                {
                    "achievement_id": 155,
                    "achieveddate": 1629630730
                },
                {
                    "achievement_id": 6,
                    "achieveddate": 1629824368
                },
                {
                    "achievement_id": 2,
                    "achieveddate": 1629827763
                },
                {
                    "achievement_id": 14,
                    "achieveddate": 1629905140
                },
                {
                    "achievement_id": 26,
                    "achieveddate": 1629906849
                },
                {
                    "achievement_id": 30,
                    "achieveddate": 1630080582
                },
                {
                    "achievement_id": 32,
                    "achieveddate": 1630082477
                },
                {
                    "achievement_id": 28,
                    "achieveddate": 1630088891
                },
                {
                    "achievement_id": 159,
                    "achieveddate": 1632588508
                },
                {
                    "achievement_id": 169,
                    "achieveddate": 1633535469
                },
                {
                    "achievement_id": 166,
                    "achieveddate": 1635016031
                },
                {
                    "achievement_id": 163,
                    "achieveddate": 1635019437
                },
                {
                    "achievement_id": 36,
                    "achieveddate": 1637346511
                },
                {
                    "achievement_id": 151,
                    "achieveddate": 1637412992
                },
                {
                    "achievement_id": 34,
                    "achieveddate": 1637772075
                },
                {
                    "achievement_id": 9,
                    "achieveddate": 1637783208
                },
                {
                    "achievement_id": 167,
                    "achieveddate": 1638132862
                },
                {
                    "achievement_id": 16,
                    "achieveddate": 1638641089
                },
                {
                    "achievement_id": 13,
                    "achieveddate": 1638990179
                },
                {
                    "achievement_id": 40,
                    "achieveddate": 1639145635
                },
                {
                    "achievement_id": 38,
                    "achieveddate": 1640711462
                },
                {
                    "achievement_id": 114,
                    "achieveddate": 1640719295
                },
                {
                    "achievement_id": 8,
                    "achieveddate": 1640883486
                },
                {
                    "achievement_id": 137,
                    "achieveddate": 1641915812
                },
                {
                    "achievement_id": 116,
                    "achieveddate": 1642176763
                },
                {
                    "achievement_id": 43,
                    "achieveddate": 1642364336
                },
                {
                    "achievement_id": 39,
                    "achieveddate": 1642698624
                },
                {
                    "achievement_id": 135,
                    "achieveddate": 1642782629
                },
                {
                    "achievement_id": 11,
                    "achieveddate": 1643319146
                },
                {
                    "achievement_id": 138,
                    "achieveddate": 1643321248
                },
                {
                    "achievement_id": 108,
                    "achieveddate": 1643500101
                },
                {
                    "achievement_id": 25,
                    "achieveddate": 1643504337
                },
                {
                    "achievement_id": 37,
                    "achieveddate": 1644595009
                },
                {
                    "achievement_id": 189,
                    "achieveddate": 1654269119
                },
                {
                    "achievement_id": 191,
                    "achieveddate": 1654271337
                },
                {
                    "achievement_id": 188,
                    "achieveddate": 1654271769
                },
                {
                    "achievement_id": 187,
                    "achieveddate": 1654428877
                },
                {
                    "achievement_id": 186,
                    "achieveddate": 1655128807
                },
                {
                    "achievement_id": 180,
                    "achieveddate": 1657570506
                },
                {
                    "achievement_id": 181,
                    "achieveddate": 1657572348
                },
                {
                    "achievement_id": 182,
                    "achieveddate": 1657574098
                },
                {
                    "achievement_id": 179,
                    "achieveddate": 1657574770
                },
                {
                    "achievement_id": 153,
                    "achieveddate": 1657733074
                },
                {
                    "achievement_id": 172,
                    "achieveddate": 1659968663
                },
                {
                    "achievement_id": 154,
                    "achieveddate": 1662642348
                },
                {
                    "achievement_id": 173,
                    "achieveddate": 1662917254
                },
                {
                    "achievement_id": 174,
                    "achieveddate": 1663433276
                },
                {
                    "achievement_id": 171,
                    "achieveddate": 1663434464
                }
            ]
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
        "userAchievementsMap": {
            "type": "array",
            "items": {
                "type": "object",
                "properties": {
                    "196240": {
                        "type": "array",
                        "items": {
                            "type": "object",
                            "properties": {
                                "achievement_id": {
                                    "type": "integer"
                                },
                                "achieveddate": {
                                    "type": "integer"
                                }
                            },
                            "required": [
                                "achieveddate",
                                "achievement_id"
                            ]
                        }
                    }
                },
                "required": [
                    "196240"
                ]
            }
        }
    },
    "required": [
        "result",
        "userAchievementsMap"
    ]
}
```
