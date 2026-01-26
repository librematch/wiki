# [GET] /community/leaderboard/GetAvatarStatForProfile

[Example request](https://aoe-api.worldsedgelink.com/community/leaderboard/GetAvatarStatForProfile?title=age2&profile_names=[%22/steam/76561197984749679%22])

## Request

| parameter     | type       | value                      | comments |
| ------------- | ---------- | -------------------------- | -------- |
| title         | str/enum   | age1, age2, age3, age4     |          |
| profile_names | array[str] | e.g. ["/steam/<steam_id>"] |          |

## Response

### AoE2:DE

```
{
  "result": {
    "code": 0,
    "message": "SUCCESS"
  },
  "avatarStatsForProfile": [
    {
      "profile_id": 196240,
      "avatarstat_id": 1,
      "value": 1845,
      "lastupdated": 1664821730
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2,
      "value": 2257,
      "lastupdated": 1664824306
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 3,
      "value": 102,
      "lastupdated": 1664543322
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 4,
      "value": 115,
      "lastupdated": 1662126936
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 5,
      "value": 73,
      "lastupdated": 1664375288
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 6,
      "value": 78,
      "lastupdated": 1661174868
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 7,
      "value": 65,
      "lastupdated": 1664805235
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 8,
      "value": 86,
      "lastupdated": 1664738137
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 9,
      "value": 41,
      "lastupdated": 1663857093
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 10,
      "value": 70,
      "lastupdated": 1664801959
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 11,
      "value": 93,
      "lastupdated": 1664550298
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 12,
      "value": 53,
      "lastupdated": 1664800693
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 13,
      "value": 84,
      "lastupdated": 1664821730
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 14,
      "value": 101,
      "lastupdated": 1662646374
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 15,
      "value": 54,
      "lastupdated": 1656451684
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 16,
      "value": 61,
      "lastupdated": 1663678517
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 17,
      "value": 71,
      "lastupdated": 1663512692
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 18,
      "value": 79,
      "lastupdated": 1664032978
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 19,
      "value": 116,
      "lastupdated": 1663511055
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 20,
      "value": 70,
      "lastupdated": 1663777500
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 21,
      "value": 60,
      "lastupdated": 1664741757
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 22,
      "value": 64,
      "lastupdated": 1664025968
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 23,
      "value": 50,
      "lastupdated": 1662991895
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 24,
      "value": 84,
      "lastupdated": 1657667959
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 25,
      "value": 57,
      "lastupdated": 1664553540
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 26,
      "value": 66,
      "lastupdated": 1654257725
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 27,
      "value": 65,
      "lastupdated": 1664803870
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 28,
      "value": 60,
      "lastupdated": 1658353231
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 29,
      "value": 70,
      "lastupdated": 1662648662
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 30,
      "value": 131,
      "lastupdated": 1663515910
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 31,
      "value": 66,
      "lastupdated": 1664740068
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 32,
      "value": 44,
      "lastupdated": 1664555928
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 33,
      "value": 60,
      "lastupdated": 1659956167
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 34,
      "value": 53,
      "lastupdated": 1663681533
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 35,
      "value": 119,
      "lastupdated": 1663425497
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 36,
      "value": 103,
      "lastupdated": 1659984820
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 37,
      "value": 87,
      "lastupdated": 1661359315
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 38,
      "value": 1181,
      "lastupdated": 1664821730
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 39,
      "value": 71867,
      "lastupdated": 1644600017
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 40,
      "value": 63196,
      "lastupdated": 1590445116
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 41,
      "value": 54056,
      "lastupdated": 1601508247
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 42,
      "value": 7088,
      "lastupdated": 1587672760
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 43,
      "value": 1820,
      "lastupdated": 1645994407
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 44,
      "value": 587315,
      "lastupdated": 1666350780
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 45,
      "value": 492834,
      "lastupdated": 1666277546
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 46,
      "value": 3788,
      "lastupdated": 1664824306
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 47,
      "value": 33564,
      "lastupdated": 1664824307
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 48,
      "value": 23147,
      "lastupdated": 1664824307
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 49,
      "value": 22,
      "lastupdated": 1642699546
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 50,
      "value": 6986,
      "lastupdated": 1664824307
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 51,
      "value": 112,
      "lastupdated": 1613239790
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 52,
      "value": 1341,
      "lastupdated": 1664821714
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 53,
      "value": 6914,
      "lastupdated": 1664823296
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 54,
      "value": 19473,
      "lastupdated": 1664807649
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 55,
      "value": 265,
      "lastupdated": 1660311031
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 56,
      "value": 7487,
      "lastupdated": 1664821724
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 57,
      "value": 2292,
      "lastupdated": 1664821434
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 59,
      "value": 575,
      "lastupdated": 1666378996
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 60,
      "value": 2964,
      "lastupdated": 1664824307
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 61,
      "value": 2655,
      "lastupdated": 1666272605
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 63,
      "value": 304,
      "lastupdated": 1663765422
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 64,
      "value": 28,
      "lastupdated": 1579635385
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 65,
      "value": 9,
      "lastupdated": 1662832252
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 69,
      "value": 219,
      "lastupdated": 1664736518
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 70,
      "value": 242,
      "lastupdated": 1664741757
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 71,
      "value": 104,
      "lastupdated": 1658518183
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 72,
      "value": 185,
      "lastupdated": 1664805235
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 73,
      "value": 109,
      "lastupdated": 1663854494
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 74,
      "value": 117,
      "lastupdated": 1662653204
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 75,
      "value": 93,
      "lastupdated": 1664803871
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 76,
      "value": 163,
      "lastupdated": 1664800693
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 77,
      "value": 136,
      "lastupdated": 1663683543
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 78,
      "value": 89,
      "lastupdated": 1662917253
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 79,
      "value": 134,
      "lastupdated": 1660931004
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 80,
      "value": 206,
      "lastupdated": 1664802710
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 81,
      "value": 128,
      "lastupdated": 1664555928
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 82,
      "value": 99,
      "lastupdated": 1664032978
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 83,
      "value": 130,
      "lastupdated": 1664024426
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 84,
      "value": 137,
      "lastupdated": 1664733092
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 85,
      "value": 141,
      "lastupdated": 1660938017
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 86,
      "value": 76,
      "lastupdated": 1663854494
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 87,
      "value": 103,
      "lastupdated": 1664550298
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 88,
      "value": 121,
      "lastupdated": 1664379013
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 89,
      "value": 119,
      "lastupdated": 1663858737
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 90,
      "value": 102,
      "lastupdated": 1662832252
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 91,
      "value": 137,
      "lastupdated": 1663857094
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 92,
      "value": 87,
      "lastupdated": 1663434463
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 93,
      "value": 137,
      "lastupdated": 1664738137
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 94,
      "value": 101,
      "lastupdated": 1663858737
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 95,
      "value": 103,
      "lastupdated": 1663766872
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 96,
      "value": 155,
      "lastupdated": 1664740068
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 97,
      "value": 78,
      "lastupdated": 1664461568
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 98,
      "value": 94,
      "lastupdated": 1664801959
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 99,
      "value": 93,
      "lastupdated": 1664821730
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 100,
      "value": 106,
      "lastupdated": 1664460137
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 101,
      "value": 140,
      "lastupdated": 1663777500
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 102,
      "value": 149,
      "lastupdated": 1662733102
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 103,
      "value": 144,
      "lastupdated": 1663857094
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 104,
      "value": 1202,
      "lastupdated": 1637176716
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 105,
      "value": 2715,
      "lastupdated": 1590445123
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 106,
      "value": 2362,
      "lastupdated": 1586542566
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 107,
      "value": 83,
      "lastupdated": 1574360632
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 108,
      "value": 298,
      "lastupdated": 1573492938
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 109,
      "value": 190,
      "lastupdated": 1579445688
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 111,
      "value": 8636,
      "lastupdated": 1664824307
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 142,
      "value": 3778,
      "lastupdated": 1666378971
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 143,
      "value": 461,
      "lastupdated": 1666378971
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 144,
      "value": 193,
      "lastupdated": 1663432615
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 153,
      "value": 5091,
      "lastupdated": 1664824266
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 154,
      "value": 329,
      "lastupdated": 1643651869
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 155,
      "value": 187075,
      "lastupdated": 1666350745
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 156,
      "value": 3252,
      "lastupdated": 1664824322
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 157,
      "value": 128,
      "lastupdated": 1634149885
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 158,
      "value": 263483,
      "lastupdated": 1645986873
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 159,
      "value": 14347,
      "lastupdated": 1662410427
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 160,
      "value": 512,
      "lastupdated": 1625324434
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 163,
      "value": 7,
      "lastupdated": 1621498349
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 165,
      "value": 78,
      "lastupdated": 1666378997
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 166,
      "value": 1478,
      "lastupdated": 1666378997
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 167,
      "value": 33,
      "lastupdated": 1666378997
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 168,
      "value": 3369,
      "lastupdated": 1625397812
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 169,
      "value": 639,
      "lastupdated": 1625320810
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 170,
      "value": 10,
      "lastupdated": 1619796153
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 171,
      "value": 659,
      "lastupdated": 1664824307
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 172,
      "value": 84009,
      "lastupdated": 1664824307
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 173,
      "value": 2967,
      "lastupdated": 1664824307
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 174,
      "value": 36,
      "lastupdated": 1657733209
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 175,
      "value": 26,
      "lastupdated": 1664468459
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 176,
      "value": 40,
      "lastupdated": 1664031535
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 177,
      "value": 61,
      "lastupdated": 1663858737
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 184,
      "value": 19,
      "lastupdated": 1664031535
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 185,
      "value": 24,
      "lastupdated": 1664733092
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 186,
      "value": 18,
      "lastupdated": 1663254117
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 187,
      "value": 35,
      "lastupdated": 1663690703
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 194,
      "value": 62604,
      "lastupdated": 1664031524
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 195,
      "value": 22,
      "lastupdated": 1664736518
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 196,
      "value": 18,
      "lastupdated": 1664802710
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 197,
      "value": 14,
      "lastupdated": 1661961561
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 198,
      "value": 1,
      "lastupdated": 1662392675
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 199,
      "value": 3,
      "lastupdated": 1664282542
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 200,
      "value": 9,
      "lastupdated": 1663777500
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 1001,
      "value": 37035,
      "lastupdated": 1595964196
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 1002,
      "value": 37035,
      "lastupdated": 1595964196
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 1003,
      "value": 60636,
      "lastupdated": 1601427762
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 1004,
      "value": 13311,
      "lastupdated": 1601558744
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2060,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2061,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2067,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2068,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2069,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2070,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2071,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2072,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2073,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2074,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2075,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2076,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2077,
      "value": 13,
      "lastupdated": 1633525772
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2078,
      "value": 13,
      "lastupdated": 1633533992
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2079,
      "value": 13,
      "lastupdated": 1633535824
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2080,
      "value": 13,
      "lastupdated": 1635011490
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2081,
      "value": 13,
      "lastupdated": 1635013888
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2082,
      "value": 13,
      "lastupdated": 1635016045
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2083,
      "value": 13,
      "lastupdated": 1635019436
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2202,
      "value": 13,
      "lastupdated": 1642689852
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2203,
      "value": 13,
      "lastupdated": 1642693452
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2204,
      "value": 13,
      "lastupdated": 1642694869
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2205,
      "value": 13,
      "lastupdated": 1642696112
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2206,
      "value": 13,
      "lastupdated": 1642698041
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2207,
      "value": 13,
      "lastupdated": 1642699547
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2235,
      "value": 13,
      "lastupdated": 1659964477
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2236,
      "value": 13,
      "lastupdated": 1659968663
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2237,
      "value": 13,
      "lastupdated": 1662133529
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2238,
      "value": 13,
      "lastupdated": 1662917253
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2239,
      "value": 13,
      "lastupdated": 1663434463
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2245,
      "value": 13,
      "lastupdated": 1657565991
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2246,
      "value": 13,
      "lastupdated": 1657568908
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2247,
      "value": 13,
      "lastupdated": 1657570526
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2248,
      "value": 13,
      "lastupdated": 1657572368
    },
    {
      "profile_id": 196240,
      "avatarstat_id": 2249,
      "value": 13,
      "lastupdated": 1657574769
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
        "avatarStatsForProfile": {
            "type": "array",
            "items": {
                "type": "object",
                "properties": {
                    "profile_id": {
                        "type": "integer"
                    },
                    "avatarstat_id": {
                        "type": "integer"
                    },
                    "value": {
                        "type": "integer"
                    },
                    "lastupdated": {
                        "type": "integer"
                    }
                },
                "required": [
                    "avatarstat_id",
                    "lastupdated",
                    "profile_id",
                    "value"
                ]
            }
        }
    },
    "required": [
        "avatarStatsForProfile",
        "result"
    ]
}
```
