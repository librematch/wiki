# API Reference - Constants & Enums

This page provides a quick reference for all IDs and constants used in the WorldsEdgeLink API.

> **Source:** These values are extracted from the API responses of [/community/leaderboard/GetAvailableLeaderboards](../rlink/community/leaderboard/getavailableleaderboards.md) and [/game/automatch2/getAutomatchMap](../rlink/game/automatch2/getautomatchmap.md).

## Leaderboards

| ID | Name             | Description                      |
| -- | ---------------- | -------------------------------- |
| 1  | `SOLO_DM_RANKED` | 1v1 Death Match                  |
| 2  | `TEAM_DM_RANKED` | Team Death Match (2v2, 3v3, 4v4) |
| 3  | `SOLO_RM_RANKED` | 1v1 Random Map                   |
| 4  | `TEAM_RM_RANKED` | Team Random Map (2v2, 3v3, 4v4)  |
| 5  | `SOLO_BR_RANKED` | Battle Royale (FFA)              |
| 13 | `SOLO_EW_RANKED` | 1v1 Empire Wars                  |
| 14 | `TEAM_EW_RANKED` | Team Empire Wars (2v2, 3v3, 4v4) |

## Match Types

| ID | Name           | Mode                    |
| -- | -------------- | ----------------------- |
| 2  | 1V1            | Death Match             |
| 3  | 2V2            | Death Match             |
| 4  | 3V3            | Death Match             |
| 5  | 4V4            | Death Match             |
| 6  | 1V1            | Random Map              |
| 7  | 2V2            | Random Map              |
| 8  | 3V3            | Random Map              |
| 9  | 4V4            | Random Map              |
| 10 | FFA            | Battle Royale           |
| 26 | 1V1            | Empire Wars             |
| 27 | 2V2            | Empire Wars             |
| 28 | 3V3            | Empire Wars             |
| 29 | 4V4            | Empire Wars             |
| 60 | CUSTOM_DM_1v1  | Custom Death Match 1v1  |
| 61 | CUSTOM_DM_TEAM | Custom Death Match Team |

## Civilizations (Races)

| ID | Name        |
| -- | ----------- |
| 0  | Aztecs      |
| 1  | Berbers     |
| 2  | Britons     |
| 3  | Bulgarians  |
| 4  | Burmese     |
| 5  | Byzantines  |
| 6  | Celts       |
| 7  | Chinese     |
| 8  | Cumans      |
| 9  | Ethiopians  |
| 10 | Franks      |
| 11 | Goths       |
| 12 | Huns        |
| 13 | Incas       |
| 14 | Hindustanis |
| 15 | Italians    |
| 16 | Japanese    |
| 17 | Khmer       |
| 18 | Koreans     |
| 19 | Lithuanians |
| 20 | Magyars     |
| 21 | Malay       |
| 22 | Malians     |
| 23 | Mayans      |
| 24 | Mongols     |
| 25 | Persians    |
| 26 | Portuguese  |
| 27 | Saracens    |
| 28 | Slavs       |
| 29 | Spanish     |
| 30 | Tatars      |
| 31 | Teutons     |
| 32 | Turks       |
| 33 | Vietnamese  |
| 34 | Vikings     |
| 35 | Burgundians |
| 36 | Sicilians   |
| 37 | Poles       |
| 38 | Bohemians   |
| 39 | Bengalis    |
| 40 | Dravidians  |
| 41 | Gurjaras    |

> **Note:** Civilization IDs may shift when new DLCs are released. See the [Changelog](../librematch/data_sources/changelog/) for historical changes.

## Leaderboard Regions

| ID | Name          |
| -- | ------------- |
| 0  | Europe        |
| 1  | Middle East   |
| 2  | Asia          |
| 3  | North America |
| 4  | South America |
| 5  | Oceania       |
| 6  | Africa        |
| 7  | Unknown       |

## Maps (Selection)

Common ranked maps:

| ID | Filename            | Map Name         |
| -- | ------------------- | ---------------- |
| 1  | AfricanClearing.rms | African Clearing |
| 2  | Arabia.rms          | Arabia           |
| 3  | Arena.rms           | Arena            |
| 4  | FourLakes.rms       | Four Lakes       |
| 5  | Islands.rms         | Islands          |
| 6  | nomad.rms           | Nomad            |
| 7  | Yucatan.rms         | Yucatan          |
| 14 | Black_Forest.rms    | Black Forest     |
| 17 | Fortress.rms        | Fortress         |
| 20 | Mediterranean.rms   | Mediterranean    |
| 23 | megarandom.rms2     | Mega Random      |
| 26 | Michi.rms           | Michi            |
| 29 | Nile Delta.rms      | Nile Delta       |
| 36 | Ghost_Lake.rms      | Ghost Lake       |
| 37 | goldenpit.rms2      | Golden Pit       |
| 38 | GoldenSwamp.rms     | Golden Swamp     |
| 39 | Kilimanjaro.rms     | Kilimanjaro      |
| 40 | valley.rms2         | Valley           |
| 41 | acropolis.rms2      | Acropolis        |
| 43 | Serengeti.rms       | Serengeti        |

> **Note:** Map IDs vary by match type (1v1, 2v2, etc.). The full list is available in the [getAutomatchMap endpoint](../rlink/game/automatch2/getautomatchmap.md).

## Game Titles

| Value  | Game                                   |
| ------ | -------------------------------------- |
| `age1` | Age of Empires: Definitive Edition     |
| `age2` | Age of Empires II: Definitive Edition  |
| `age3` | Age of Empires III: Definitive Edition |
| `age4` | Age of Empires IV                      |

## Platforms

| Value              | Platform               |
| ------------------ | ---------------------- |
| `PC_STEAM`         | Steam                  |
| `PC_WINDOWS_STORE` | Microsoft Store / Xbox |

## Result Codes

| Code | Message           | Description                      |
| ---- | ----------------- | -------------------------------- |
| 0    | `SUCCESS`         | Request successful               |
| -1   | `FAILED`          | Generic failure                  |
| 2    | `INVALID_SESSION` | Session expired, re-authenticate |

## HTTP Status Codes

| Code | Meaning           | Action                            |
| ---- | ----------------- | --------------------------------- |
| 200  | OK                | Request successful                |
| 429  | Too Many Requests | Rate limited - back off and retry |
| 403  | Forbidden         | Invalid or expired session        |

## Rate Limits

| API           | Limit        | Recommendation                |
| ------------- | ------------ | ----------------------------- |
| Community API | 50 req/sec   | Safe for most use cases       |
| Game API      | ~200 req/min | Use 100 req/30 sec for safety |

See [Usage Guidelines](../rlink/usage.md) for more details.
