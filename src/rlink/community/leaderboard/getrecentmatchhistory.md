# [GET] /community/leaderboard/getRecentMatchHistory

[Example request](https://aoe-api.worldsedgelink.com/community/leaderboard/getRecentMatchHistory?title=age2&profile_names=[%22/steam/76561197984749679%22])

## Request

| parameter     | type       | value                      | comments |
| ------------- | ---------- | -------------------------- | -------- |
| title         | str/enum   | age1, age2, age3, age4     |          |
| profile_names | array[str] | e.g. ["/steam/<steam_id>"] |          |
| profile_ids   | array[int] | e.g. ["<relic_link_id>"]   |          |
| aliases       | array[str] | e.g. [BlackRock]           |          |

## Response

### AoE2:DE

```
{
  "result": {
    "code": 0,
    "message": "SUCCESS"
  },
  "matchHistoryStats": [
    {
      "id": 183556359,
      "creator_profile_id": 199325,
      "mapname": "FrigidLake.rms",
      "maxplayers": 2,
      "matchtype_id": 26,
      "options": "eNpFUtFugzAM/Jd9waAQqY+pQqdKcyK6ZBp7LJuQwjb60CqQr5+DHcrTCdvnO1+ezkMr8SvBT1EGREoKCPwvXu+HBNUYjYdA9UZcaKYy6lrTv5OAlmfsFA4JqS4YL5sEjZU4AwkWxrtLAtqCuJT7uXO329n/mPPHMXxFHT7f9te+qZ2zz3vmEWDhSDMnoeNp5dTebTq0zzvH0niqG9WLb9K0M74vSOeQdRY6Tgvzl+ZvZM40s+qss3ZA7SC7BGf0Nms7HslTK8B3hJUTr7Zh3CbMfNu+0tipoH093sVRPTZYd6tGvP8M0tGeOBUg17lZq2mmDBq8XR8Ow4rRZ7Polnsi9qzcTWX8wLpH5B6IG+ugZGDOBVS+12lGnlU3eLxt9uxBwLBqWXB/yf53SQt4x/0O/ef+LvtYUEsJlMti1BTZM2ofXqh3THO8HzAbvlXscl41eHx3VK8e9T7nXWDe7Lddtrzt9i536V3y3nrL1mIW5L8ClfmHeXujjzdc4b0C3dzV5vf9/vQPbS3yvQ==",
      "slotinfo": "eNq9kFFPgzAUhf0tfa5mFDVhiS9z6wIRHQUqm/GhQAlNSyFQTabxv7s2LsZkPvji0zn33nPvTT4Pwad3MIx9IxQPddNfiBrMvSDw0RUEk2FG9DpcHloQGM46a2cQNKw6Dg7VyCpuLQqs1/KOv3L1NdEyZqZqs/3gIuf2juj4ho94ZB2PU5cTE+Gs3rs39unL5NodN2zJDANzEErskxwvkhz7CXW6IpRYXdAseijXkSFatfRNka2s1/d02KZyECWNpl2Osc0lRXvrNN+lJVZFvIrcfvZYBZs0vAEf8BSLa3Q5+8ECfbPwfmPhof9lkfyZRX2aRXFk8Xz2CSorqfs=",
      "description": "AUTOMATCH",
      "startgametime": 1664802149,
      "completiontime": 1664802709,
      "observertotal": 4,
      "matchhistoryreportresults": [
        {
          "matchhistory_id": 183556359,
          "profile_id": 199325,
          "resulttype": 0,
          "teamid": 0,
          "race_id": 29,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1664802149
        },
        {
          "matchhistory_id": 183556359,
          "profile_id": 196240,
          "resulttype": 1,
          "teamid": 1,
          "race_id": 12,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1664802149
        }
      ],
      "matchhistoryitems": [],
      "matchurls": []
    },
    {
      "id": 85506328,
      "creator_profile_id": 196240,
      "mapname": "FourLakes.rms",
      "maxplayers": 2,
      "matchtype_id": 2,
      "options": "eNpFUtFqwzAM/Jd+QZM0hj3swa2zkRXZBOyO7LFpMTjQFMaI46+fYstpno5Id7qTvOtsx/ErwU2Bz4gEZzL/C8+/4wrF6JWDOdUbdk31g3TPOv1rGXTE0dN8XJHoZ+V4s0IlLHJghYVy5roCqYHdHz/+Lr5O+vTrL5fbDN91uJX1eN7fzkbv35J2z8CayEWPFZA3qdFbnGP3rzmG3ZOPSrmhSHybvRUyTAt5K9VjjBzpBuREb3XWAc0Z8H6FHvN4KTj1blql0lORtAbMaVI9NFiPXiv06oGbpBGmAnjkodbk004b3MUwH23EpXLNIjvqCdgTtZuDcpY8jahtkzbWQfCZNBcQeect3qn5iP2uZTLncZB3uOD8krJVqxdwhvoNg62/zzkW9FLSzhclpkCZ0bv9TL3jyqP5gHtvaRd9vkUNIt8KME9H9SG/o0K6nLdb8J3RLcdcr5R41jS33u6m8RYp/+Glb/3rLWxv8gDbPg3euH3f/QMzquR+",
      "slotinfo": "eNrNj90KgkAQhXuWvd6i1QoLupEyjIL87SK6GHSsRV1Ft0Cid8+fIqIeoKtzZs5who8p9HAjeZFFPEFTRNmAh2SmaKqqjSgpJUieCXNRryiRCGljh5REELyCeiogwMYypfEi3uAVk2ci4i3I4OxWeXvSZ3UPT3GHhVFAilunveOljRBWdUX39FK26xQlLEACmREzNoTtGbrlGarlt7p0Pb9R3Y/DPazW9jMfm6f5nNzpNxebTpTR8IOLvbnYv3A5v7kmHdex9wByE4a2",
      "description": "AUTOMATCH",
      "startgametime": 1618868684,
      "completiontime": 1618869103,
      "observertotal": 0,
      "matchhistoryreportresults": [
        {
          "matchhistory_id": 85506328,
          "profile_id": 283384,
          "resulttype": 0,
          "teamid": 0,
          "race_id": 12,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1618868684
        },
        {
          "matchhistory_id": 85506328,
          "profile_id": 196240,
          "resulttype": 1,
          "teamid": 1,
          "race_id": 12,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1618868684
        }
      ],
      "matchhistoryitems": [],
      "matchurls": []
    },
    {
      "id": 169858702,
      "creator_profile_id": 335285,
      "mapname": "lombardia.rms2",
      "maxplayers": 4,
      "matchtype_id": 7,
      "options": "eNpFUstugzAQ/Jd8QSBgtUdHJhVS1xapHZXeElShmiTkEgH++q69NvFp5H3NzO7m2DccXw52dHxCJDiD9Ocez72HYnDKwkTxil0oXijxKOmvZtDEGj1Oe49EOynLKw+V5lgDHmbKmosHUgM7X/n0cz/9fd2u2Xn7tnT5oeysbLrvY9Xo7Tv1bhlwE2qR4y5xkxq5hTl9/prTJh6FdI+S4h2TzogQF+NMf2anbB1qpG3Zb+Tua2jmkDyYQaCe4EE1oweO6oetst2Behr2qauIG49j3371ROkxi1zQE0NxV2E86NqhrjlqnMGNGXCaLT1fmo2+ddO+Dxj1VotsYo5LmqpC2T70Bo38m556YxwEn2LPJegJ+TXqId5gayajh2ABtQcuC87Pgbehj+cC1sR8w2DNb5OOBbnk0bcFvY5edci9/6DcwdfF+YA7iF65dQcl2LRXKF7xLt1cJm3S2yxph0qvN7nzNxnnluo+UL3GXZD+AsR6N/N6N6/7LdCvuG9TqtvpufkHFG3xaQ==",
      "slotinfo": "eNq9kttPgzAYxf1b+oxm5SaQ+DK3LhCZ41ZhxocCJSNcA9VkGv93ATWGeBsvPH2nPaf9kl8O5Ln7F1A3VZLmVC+T6iKNgQZVmRcXHGgZYWlV6iug8RxglBS97IyERJ9Gd2pIRHsp97LMbugTzT+MMjMJiw7usR4S57D7Ji3ojjaoIQU1nSGXtjYl8bFb/L7zsR2uC8rIijACNKBnSLA9tLQ8JFh4mGsX2/1cYte4DTcGs8v8gJ9zO8jizRbXgZPVaYiNdu8h1Ocsv74eprd3QpT75toY3rt3kbpz9Cvwyn1HIQgSr0gjFPALBfwNBT8zC2cyi/xnFv5fLBayIoviCIZ4Qi+gMi+MAE6E4W6nF0OVRV5SRyyEE4oBL+dlYU0uRvxPMR7O3gAlpVLU",
      "description": "AUTOMATCH",
      "startgametime": 1657731492,
      "completiontime": 1657733209,
      "observertotal": 1,
      "matchhistoryreportresults": [
        {
          "matchhistory_id": 169858702,
          "profile_id": 196240,
          "resulttype": 1,
          "teamid": 0,
          "race_id": 6,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1657731492
        },
        {
          "matchhistory_id": 169858702,
          "profile_id": 335285,
          "resulttype": 0,
          "teamid": 1,
          "race_id": 26,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1657731492
        },
        {
          "matchhistory_id": 169858702,
          "profile_id": 3068644,
          "resulttype": 1,
          "teamid": 0,
          "race_id": 18,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1657731492
        },
        {
          "matchhistory_id": 169858702,
          "profile_id": 964259,
          "resulttype": 0,
          "teamid": 1,
          "race_id": 17,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1657731492
        }
      ],
      "matchhistoryitems": [],
      "matchurls": [
        {
          "profile_id": 964259,
          "url": "https://rl0aoelivemk2blob.blob.core.windows.net/cloudfiles/952469/aoelive_/age2/replay/windows/4.0.0/0/M_169858702_6078abab91f29e8b5df7d4f419d11677354ba9688802d3d013bb077ca07b65ab.gz",
          "size": 541614,
          "datatype": 0
        }
      ]
    },
    {
      "id": 137085400,
      "creator_profile_id": 2212083,
      "mapname": "Runestones.rms",
      "maxplayers": 8,
      "matchtype_id": 9,
      "options": "eNpFUstugzAQ/Jd8ASTGUo+O7KQ+2BapHZVrSOVq04ZcKsBf38UP4LTy7szOzrBrfcvw2ysYAhux4oyq8hZef8el5I/JgBpTX9Bb6hMNrya9SarajLHDeFwq3o0GmFhKwz1i1FLWBtxtKbRV1FWSXH7u/ON5d5fP67c5Xd+taISy+uxs9Za4O6qYi1jUeCjatEVtcY+vtj2OfiUdBwN9nfC+aKt1GOasbW+ej4jR0CMmamsMtPFNWfSARcyE9zQZQwyIjHlQnfcoPtSp36NH4hT7Af2w7JS4FNWWZd4WtcRbJm3xFtalGoZJgcszfdE7GT6QxC1Qm5CJWy3co+KZE1atM2qdUl5yNtDlHGQwIJMWaKkGdk48qMXKOs9jLrLM78sdCr3RIPMe9HFMN6N2cvRxtllweX9Af6fsxeqvQS/z/xLwntI/mF+SvLRdubfCfHM+vln7wW+Z2lfOwpEt85WfbP+en0tWhqviT23Qn90/rH3fhQ==",
      "slotinfo": "eNq91FtPgzAUB3A/S5/R0BZYWeLL3LpA3Ny47WJ86KDLCJcRQJNp/O4CagzxRvfAUw/toSS//DkQSfcvIMuP+zDmRro/XoUBGGJVJkRFEihKVobH1BhXexIoOUvqUpbAnvmfB9VTznxel5DUdRrd8icef5yk0YyV/sE5ZU3LJazuCRO+4DnNWcJndtMXFhZnwam64v2jj0WznfCSjVnJwBAYEcWWS0dLl+Kl16yTDbTqdeQ55t1uapZWGh+859jaRMF07mUbO8rCnWcWW5fSum/pzG+a1d3aOxqvZxOzed9Z+frCNq7Bq/QdAyGIZIJbGPALA/6KAfvFWHmiGObPGOs/MFRMkKbLLQylSzJQvxieMAYVTwbUNaS0LVCXYKj9WrjCFiPxYCBFqaaG2sJQOwQD92thiVqsD2dMDE0fELk9MbQOwUA9B2MpjBGcEwxMdK39l5AOwVD6tXCELbJzgqEhDFsUgy4Do+fhaQtbxP/k4uHiDWVupQE=",
      "description": "AUTOMATCH",
      "startgametime": 1641495992,
      "completiontime": 1641497348,
      "observertotal": 3,
      "matchhistoryreportresults": [
        {
          "matchhistory_id": 137085400,
          "profile_id": 3508852,
          "resulttype": 0,
          "teamid": 0,
          "race_id": 18,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1641495992
        },
        {
          "matchhistory_id": 137085400,
          "profile_id": 2212083,
          "resulttype": 1,
          "teamid": 1,
          "race_id": 11,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1641495992
        },
        {
          "matchhistory_id": 137085400,
          "profile_id": 5382690,
          "resulttype": 0,
          "teamid": 0,
          "race_id": 12,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1641495992
        },
        {
          "matchhistory_id": 137085400,
          "profile_id": 196240,
          "resulttype": 1,
          "teamid": 1,
          "race_id": 15,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1641495992
        },
        {
          "matchhistory_id": 137085400,
          "profile_id": 2443505,
          "resulttype": 0,
          "teamid": 0,
          "race_id": 3,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1641495992
        },
        {
          "matchhistory_id": 137085400,
          "profile_id": 2697803,
          "resulttype": 1,
          "teamid": 1,
          "race_id": 25,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1641495992
        },
        {
          "matchhistory_id": 137085400,
          "profile_id": 2438960,
          "resulttype": 0,
          "teamid": 0,
          "race_id": 4,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1641495992
        },
        {
          "matchhistory_id": 137085400,
          "profile_id": 266231,
          "resulttype": 1,
          "teamid": 1,
          "race_id": 12,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1641495992
        }
      ],
      "matchhistoryitems": [],
      "matchurls": []
    },
    {
      "id": 39119092,
      "creator_profile_id": 196240,
      "mapname": "Megarandom.rms2",
      "maxplayers": 6,
      "matchtype_id": 8,
      "options": "eNpFUtFuwyAM/Jd+QdO0SHskhVaRBjQdrEofG02Z6FaqSVMCXz8DZuHJsu98Z5vVaewovI2wLtAJIkaJoJgLz9+c4+SWcVtpn7uca4noEKfd1MSI9ZOy0AGe1K46JpwJ6rv6uph+Oq/P5p01r1f9ub9crj/dfVe/PYaXUydSH+AeMrclMrQ8xdYs2qzojJV63HM9uFpm/lZZnnN6IALnin7RWw2c5E1pF3KOR7+JIzQnCudRzM3I2SlrUIcSmes1zDs3MWSDB80pxzwAFv3xNeQPua+BWegxxz0RC6ZetEei8s5n8DbvU30IsbdgFPHt4tVy2L2JoYe7bfBeXgTns5cW9PupGVOf6MVLxMNdfMFLW+ZowUvvUQf2KHBmA776hFWRx1A/DOX29bJfsS3+JNTxZlXSSPUOdoU3DSP5QL7ShW/++Qr+YLn58rdGX+6rmCh/tIq+Vn+3l9Vp",
      "slotinfo": "eNq9lFFrgzAUhfdb8uxGEpM4C30pncOxwrTVMUofLho3sWrRbFDG/vuMtAzZOvQlT/fknksuH4eEUGv7iQ5NneV76VdZfZOnaEZcQRm2UKtA5XXlL7uWhZSEUsvOyCA5G92pgURqSW2tq+JRfsj9yamKFajkbXM89CPX+p68lE+y8Roo5Wrdz+VtKCE99mv00ve2b5dSwRIUoBnyC68KI28RRJ4dxH2920Sxrou4SJ/h/iE8+dx/nc/Rl/Wbi1GOsTvgsn+4yCUum5rlCv7mEhe5iOs4nAy46Ji8HLNc8dS8CGG3zBmC8RGBUWEWbD01MME4FvaAi40IzDWL9YIn5kWxyx0xwBJj3pfhfyP6N67d1TfIbJIA",
      "description": "AUTOMATCH",
      "startgametime": 1600367457,
      "completiontime": 1600368887,
      "observertotal": 0,
      "matchhistoryreportresults": [
        {
          "matchhistory_id": 39119092,
          "profile_id": 196240,
          "resulttype": 1,
          "teamid": 0,
          "race_id": 23,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1600367457
        },
        {
          "matchhistory_id": 39119092,
          "profile_id": 425009,
          "resulttype": 0,
          "teamid": 1,
          "race_id": 32,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1600367457
        },
        {
          "matchhistory_id": 39119092,
          "profile_id": 197751,
          "resulttype": 1,
          "teamid": 0,
          "race_id": 27,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1600367457
        },
        {
          "matchhistory_id": 39119092,
          "profile_id": 1148471,
          "resulttype": 0,
          "teamid": 1,
          "race_id": 26,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1600367457
        },
        {
          "matchhistory_id": 39119092,
          "profile_id": 645063,
          "resulttype": 1,
          "teamid": 0,
          "race_id": 9,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1600367457
        },
        {
          "matchhistory_id": 39119092,
          "profile_id": 209576,
          "resulttype": 0,
          "teamid": 1,
          "race_id": 33,
          "xpgained": 1,
          "counters": "{}",
          "matchstartdate": 1600367457
        }
      ],
      "matchhistoryitems": [],
      "matchurls": []
    }
  ],
  "profiles": [
    {
      "profile_id": 1030879,
      "name": "/steam/76561198053896791",
      "alias": "aegus",
      "personal_statgroup_id": 1262109,
      "xp": 1278,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "be"
    },
    {
      "profile_id": 2733807,
      "name": "/steam/76561197994886806",
      "alias": "Yakoileo",
      "personal_statgroup_id": 2465256,
      "xp": 1941,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "de"
    },
    {
      "profile_id": 262670,
      "name": "/steam/76561198049454319",
      "alias": "GleeF",
      "personal_statgroup_id": 69446,
      "xp": 486,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "de"
    },
    {
      "profile_id": 251817,
      "name": "/steam/76561198388423593",
      "alias": "异邦之人",
      "personal_statgroup_id": 55831,
      "xp": 824,
      "level": 1,
      "leaderboardregion_id": 2,
      "country": "cn"
    },
    {
      "profile_id": 459716,
      "name": "/steam/76561198162951354",
      "alias": "Yaguar",
      "personal_statgroup_id": 302202,
      "xp": 1219,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "de"
    },
    {
      "profile_id": 2210218,
      "name": "/steam/76561198018573455",
      "alias": "Slappy The Happybara",
      "personal_statgroup_id": 1964413,
      "xp": 476,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "gb"
    },
    {
      "profile_id": 890300,
      "name": "/steam/76561198148687930",
      "alias": "Bluestar The Goat",
      "personal_statgroup_id": 741210,
      "xp": 1242,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "fr"
    },
    {
      "profile_id": 2436978,
      "name": "/steam/76561199044782924",
      "alias": "Jonas B 1",
      "personal_statgroup_id": 2178540,
      "xp": 1063,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "de"
    },
    {
      "profile_id": 1579822,
      "name": "/steam/76561198033283718",
      "alias": "Morovun",
      "personal_statgroup_id": 1362042,
      "xp": 1508,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "pl"
    },
    {
      "profile_id": 261045,
      "name": "/steam/76561198008192094",
      "alias": "UhtredShield",
      "personal_statgroup_id": 67391,
      "xp": 4070,
      "level": 2,
      "leaderboardregion_id": 3,
      "country": "us"
    },
    {
      "profile_id": 699609,
      "name": "/steam/76561198080566571",
      "alias": "ABH",
      "personal_statgroup_id": 562132,
      "xp": 273,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "se"
    },
    {
      "profile_id": 645063,
      "name": "/steam/76561198278909141",
      "alias": "Debbie",
      "personal_statgroup_id": 504593,
      "xp": 417,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "de"
    },
    {
      "profile_id": 701099,
      "name": "/steam/76561197965781826",
      "alias": "Pudge_Spencer",
      "personal_statgroup_id": 563709,
      "xp": 447,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "ch"
    },
    {
      "profile_id": 1649071,
      "name": "/steam/76561198402192081",
      "alias": "Yumeko",
      "personal_statgroup_id": 1429431,
      "xp": 329,
      "level": 1,
      "leaderboardregion_id": 2,
      "country": "cn"
    },
    {
      "profile_id": 1819870,
      "name": "/steam/76561198809738927",
      "alias": "Grubby",
      "personal_statgroup_id": 1594338,
      "xp": 33,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "nl"
    },
    {
      "profile_id": 1148471,
      "name": "/steam/76561199013074510",
      "alias": "EasyThisi",
      "personal_statgroup_id": 974567,
      "xp": 286,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "de"
    },
    {
      "profile_id": 224581,
      "name": "/steam/76561198023009717",
      "alias": "Fingolfin",
      "personal_statgroup_id": 21333,
      "xp": 1107,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "nl"
    },
    {
      "profile_id": 2714104,
      "name": "/xboxlive/22BEDCBDFDE7B225FD27084513A200D28EE296E3",
      "alias": "UmpahPahALADI",
      "personal_statgroup_id": 2446300,
      "xp": 6,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "de"
    },
    {
      "profile_id": 2443505,
      "name": "/steam/76561198273192464",
      "alias": "Element",
      "personal_statgroup_id": 2184780,
      "xp": 877,
      "level": 1,
      "leaderboardregion_id": 4,
      "country": "ar"
    },
    {
      "profile_id": 10198859,
      "name": "/steam/76561199285326382",
      "alias": "空心",
      "personal_statgroup_id": 5840698,
      "xp": 1119,
      "level": 1,
      "leaderboardregion_id": 2,
      "country": "cn"
    },
    {
      "profile_id": 2085896,
      "name": "/xboxlive/F3A31CA4C06ACF6E2B9BDC8E9FA55E973BF36006",
      "alias": "dam1746",
      "personal_statgroup_id": 1851227,
      "xp": 1071,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "be"
    },
    {
      "profile_id": 2524736,
      "name": "/steam/76561198007008274",
      "alias": "D•F•S | Imperio_cc",
      "personal_statgroup_id": 2263475,
      "xp": 2376,
      "level": 2,
      "leaderboardregion_id": 0,
      "country": "de"
    },
    {
      "profile_id": 1867124,
      "name": "/steam/76561198098960668",
      "alias": "Fox.Capout",
      "personal_statgroup_id": 1639684,
      "xp": 2244,
      "level": 2,
      "leaderboardregion_id": 0,
      "country": "fr"
    },
    {
      "profile_id": 196240,
      "name": "/steam/76561197984749679",
      "alias": "GL.TheViper",
      "personal_statgroup_id": 200,
      "xp": 3091,
      "level": 2,
      "leaderboardregion_id": 0,
      "country": "de"
    },
    {
      "profile_id": 1241193,
      "name": "/xboxlive/C1D081A37EDAD5A906FD4FD11117330936E2CB6E",
      "alias": "Rulianx",
      "personal_statgroup_id": 1047395,
      "xp": 625,
      "level": 1,
      "leaderboardregion_id": 0,
      "country": "fr"
    },
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
        "matchHistoryStats": {
            "type": "array",
            "items": {
                "type": "object",
                "properties": {
                    "id": {
                        "type": "integer"
                    },
                    "creator_profile_id": {
                        "type": "integer"
                    },
                    "mapname": {
                        "type": "string"
                    },
                    "maxplayers": {
                        "type": "integer"
                    },
                    "matchtype_id": {
                        "type": "integer"
                    },
                    "options": {
                        "type": "string"
                    },
                    "slotinfo": {
                        "type": "string"
                    },
                    "description": {
                        "type": "string"
                    },
                    "startgametime": {
                        "type": "integer"
                    },
                    "completiontime": {
                        "type": "integer"
                    },
                    "observertotal": {
                        "type": "integer"
                    },
                    "matchhistoryreportresults": {
                        "type": "array",
                        "items": {
                            "type": "object",
                            "properties": {
                                "matchhistory_id": {
                                    "type": "integer"
                                },
                                "profile_id": {
                                    "type": "integer"
                                },
                                "resulttype": {
                                    "type": "integer"
                                },
                                "teamid": {
                                    "type": "integer"
                                },
                                "race_id": {
                                    "type": "integer"
                                },
                                "xpgained": {
                                    "type": "integer"
                                },
                                "counters": {
                                    "type": "string"
                                },
                                "matchstartdate": {
                                    "type": "integer"
                                }
                            },
                            "required": [
                                "counters",
                                "matchhistory_id",
                                "matchstartdate",
                                "profile_id",
                                "race_id",
                                "resulttype",
                                "teamid",
                                "xpgained"
                            ]
                        }
                    },
                    "matchhistoryitems": {
                        "type": "array"
                    },
                    "matchurls": {
                        "type": "array",
                        "items": {
                            "type": "object",
                            "properties": {
                                "profile_id": {
                                    "type": "integer"
                                },
                                "url": {
                                    "type": "string"
                                },
                                "size": {
                                    "type": "integer"
                                },
                                "datatype": {
                                    "type": "integer"
                                }
                            },
                            "required": [
                                "datatype",
                                "profile_id",
                                "size",
                                "url"
                            ]
                        }
                    },
                    ####NEW ADDITION 11042023####
                    "matchhistorymember": {
                        "matchhistory_id": {
                            "type: "integer"
                        },
                        "profile_id": {
                             "type: "integer"
                        },
                        "race_id": {
                             "type: "integer"
                        },
                        "statgroup_id": {
                             "type: "integer"
                        },
                        "teamid": {
                              "type: "integer"
                        },
                        "wins": {
                            "type: "integer"
                        },
                        "losses": {
                             "type: "integer"
                        },
                        "streak": {
                            "type: "integer"
                        },
                        "arbitration": {
                             "type: "integer"
                        },
                        "outcome": {
                            "type: "integer"
                        },
                        "oldrating": {
                            "type: "integer"
                        },
                        "newrating": {
                             "type: "integer"
                        },
                        "reporttype": {
                             "type: "integer"
                        }
                    }
                },
                "required": [
                    "completiontime",
                    "creator_profile_id",
                    "description",
                    "id",
                    "mapname",
                    "matchhistoryitems",
                    "matchhistoryreportresults",
                    "matchtype_id",
                    "matchurls",
                    "maxplayers",
                    "observertotal",
                    "options",
                    "slotinfo",
                    "startgametime"
                ]
            }
        },
        "profiles": {
            "type": "array",
            "items": {
                "type": "object",
                "properties": {
                    "profile_id": {
                        "type": "integer"
                    },
                    "name": {
                        "type": "string"
                    },
                    "alias": {
                        "type": "string"
                    },
                    "personal_statgroup_id": {
                        "type": "integer"
                    },
                    "xp": {
                        "type": "integer"
                    },
                    "level": {
                        "type": "integer"
                    },
                    "leaderboardregion_id": {
                        "type": "integer"
                    },
                    "country": {
                        "type": "string"
                    }
                },
                "required": [
                    "alias",
                    "country",
                    "leaderboardregion_id",
                    "level",
                    "name",
                    "personal_statgroup_id",
                    "profile_id",
                    "xp"
                ]
            }
        }
    },
    "required": [
        "matchHistoryStats",
        "profiles",
        "result"
    ]
}
```
