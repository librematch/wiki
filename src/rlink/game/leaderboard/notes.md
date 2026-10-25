# AoE2:DE leaderboard payloads - field layouts

The Leaderboard endpoints look like opaque nested arrays, and the client parses
them **positionally**: there are no field names on the wire. This page lists the
layouts we had to match to make the ladder, the party stats and the match
history render in a local RLink-compatible server
([ageLANServer](https://github.com/luskaner/ageLANServer)).

> Empirical, from the PC client build tested in October 2026. Older captures in
> this wiki can show shorter forms of the same arrays (see the notes per table).

## Shared response shape

`getLeaderBoard`, `getPartyStat`, `getStatGroupsByProfileIDs` and
`getStatsForLeaderboardByProfileName` all return the same four elements:

```jsonc
[
    0, // result status code
    [/* statGroups */],
    [/* profileInfos */],
    [/* leaderboardStats */],
]
```

The three arrays are matched **by index**: `statGroups[i]`, `profileInfos[i]`
and `leaderboardStats[i]` describe the same player, in the same order.

If the arrays are not aligned (different lengths, a stat group whose profile is
missing, or a stats array that is shorter than the stat groups), the client
discards the whole response and logs:

```
LeaderboardCache - response was not formatted correctly
```

Our first attempt failed exactly like that. The safe rule is: only emit an entry
when you can fill all three positions, and skip the player otherwise.

## statGroup (5 fields)

| Index | Field         | Notes                                      |
| ----- | ------------- | ------------------------------------------ |
| 0     | statGroupID   | Same value as `statGroup_ids` in `peerAdd` |
| 1     | statGroupName | Empty string when unnamed                  |
| 2     | metaData      | Empty string when there is none            |
| 3     | type          | `1` for a single player                    |
| 4     | profileIDs    | Array of profile IDs, e.g. `[5591467]`     |

## profileInfo (14 or 15 fields)

| Index | Field                  | Notes                                                 |
| ----- | ---------------------- | ----------------------------------------------------- |
| 0     | entityVersion          | Unix timestamp, only needs to be stable               |
| 1     | profileID              |                                                       |
| 2     | name                   | Platform path, e.g. `/steam/76561199163227629`        |
| 3     | metaData               | Avatar metadata as a JSON string, `""` when none      |
| 4     | alias                  | Display name                                          |
| 5     | sanitizedAlias         | Only for clients with lib version >= 190              |
| 6     | clanName               | Empty string when the player has no clan              |
| 7     | personalStatGroupID    |                                                       |
| 8     | xp                     |                                                       |
| 9     | level                  |                                                       |
| 10    | leaderboardRegionID    |                                                       |
| 11    | banInfo                | `null` when the player is not banned                  |
| 12    | platformUserID         | **String**, not a number (e.g. `"76561199163227629"`) |
| 13    | accountType            | `3` Steam, `9` Xbox                                   |
| 14    | linkedPlatformAccounts | Empty array when none                                 |

The sample in [getLeaderBoard](./getleaderboard.md) has the 14-field form
(without `sanitizedAlias`), because it was captured with an older client. In
that form every field after `alias` shifts down by one, so `clanName` is at
index 5 and `linkedPlatformAccounts` at index 13.

## leaderboardStat (19 fields)

| Index | Field             | Notes                                    |
| ----- | ----------------- | ---------------------------------------- |
| 0     | statGroupID       |                                          |
| 1     | leaderboardID     | Ladder ID, `3` for 1v1 random map        |
| 2     | wins              |                                          |
| 3     | losses            |                                          |
| 4     | streak            |                                          |
| 5     | disputes          | `0` when unused                          |
| 6     | drops             |                                          |
| 7     | ranking           | `-1` when unranked                       |
| 8     | rankTotal         | `-1` when unranked                       |
| 9     | regionRanking     | `-1` when unused                         |
| 10    | regionRankTotal   | `-1` when unused                         |
| 11    | level             |                                          |
| 12    | rating            | MMR / Elo                                |
| 13    | lastMatchTime     | Unix timestamp                           |
| 14    | highestRank       |                                          |
| 15    | highestRankLevel  |                                          |
| 16    | highestRating     |                                          |
| 17    | platformRank      | Only for clients with lib version >= 190 |
| 18    | platformRankTotal | Only for clients with lib version >= 190 |

The sample in [getLeaderBoard](./getleaderboard.md) shows a 14-field form
(`statGroupID` through `lastMatchTime`), captured before `highest*` and
`platform*` were added. The current client expects the longer form; the 17-field
form has no `platformRank`/`platformRankTotal` and ends at `highestRating`.

The same array is used outside the Leaderboard endpoints:

- `platformlogin` includes it in `selectProfile`.
- The account/profile payloads include an `extraProfileInfo` with the same
  positional layout: 17 fields, or 19 with the two `platform*` fields.

## Ladder ID is not the queue ID

The 1v1 random map ladder is `leaderboard_id=3`. The automatch queues use
`matchTypes=[6]` (and `20`/`1` appear in other client builds). A server has to
map queue IDs to ladder IDs instead of reusing one for the other.

`getLeaderBoard` also receives `start` and `count`. `start` is **1-based**
(`start=1` is the first entry), so the page offset is `start - 1`.

## getRecentMatchHistory

```jsonc
[
    0, // result status code
    [/* matches */],
]
```

Each match has **16 fields**:

| Index | Field                     | Notes                                                    |
| ----- | ------------------------- | -------------------------------------------------------- |
| 0     | matchHistoryID            |                                                          |
| 1     | creatorProfileID          |                                                          |
| 2     | mapName                   |                                                          |
| 3     | maxPlayers                |                                                          |
| 4     | matchTypeID               | `0` custom, `26` for a 1v1 ranked automatch              |
| 5     | encodedOptions            | Opaque string                                            |
| 6     | encodedSlots              | Opaque string                                            |
| 7     | description               | `"AUTOMATCH"` for automatch, the map name for customs    |
| 8     | startGameTime             | Unix timestamp                                           |
| 9     | completionTime            | Unix timestamp                                           |
| 10    | observerTotal             |                                                          |
| 11    | matchHistoryReportResults | See below                                                |
| 12    | matchHistoryItems         | Empty array when there are none                          |
| 13    | matchUrls                 | Empty array when there are no replays                    |
| 14    | matchVersionInfo          | 7 fields, e.g. `["INVALID","INVALID","INVALID",0,0,0,0]` |
| 15    | matchHistoryMemberStats   | See below                                                |

`matchHistoryReportResults` entries have **9 fields**:

`matchHistoryID`, `profileID`, `resultType` (`1` win, `0` loss), `teamID`,
`raceID`, `xpGained`, `counters` (JSON string), `customUpdates` (JSON string),
`matchStartDate`.

`matchHistoryMemberStats` entries have **13 fields**:

`matchHistoryID`, `profileID`, `raceID`, `statGroupID`, `teamID`, `wins`,
`losses`, `streak`, `arbitration`, `outcome`, `oldRating`, `newRating`,
`reportType`.

`oldRating`/`newRating` are what the client shows as the MMR change in the match
history. If the server does not store ratings it can send the same value twice
or `0`.

The request uses `profile_ids` (an array). Clients may pad it with repeated or
placeholder IDs, so a server should de-duplicate them and ignore unknown ones.
