# Leaderboard Endpoints

Endpoints for accessing player rankings, statistics, and match history.

> **Authentication:** All endpoints in this section require Steam authentication.

## Endpoints

| Endpoint                                                                        | Method   | Description                                                              |
| ------------------------------------------------------------------------------- | -------- | ------------------------------------------------------------------------ |
| [getAvailableLeaderboards](./getavailableleaderboards.md)                       | GET      | Get all leaderboard definitions, match types, civilizations, and regions |
| [getLeaderBoard](./getleaderboard.md)                                           | GET      | Get ranked leaderboard entries with player stats                         |
| [getPartyStat](./getpartystat.md)                                               | GET      | Get statistics for a party/team                                          |
| [getPersonalStat](./getpersonalstat.md)                                         | GET      | Get personal statistics for a player                                     |
| [getRecentMatchHistory](./getrecentmatchhistory.md)                             | GET/POST | Get recent match history for player(s)                                   |
| [getRecentMatchSinglePlayerHistory](./getrecentmatchsingleplayerhistory.md)     | GET      | Get single-player match history                                          |
| [getStatGroupsByProfileIDs](./getstatgroupsbyprofileids.md)                     | GET      | Get stat groups for multiple profile IDs                                 |
| [getStatsForLeaderboardByProfileName](./getstatsforleaderboardbyprofilename.md) | GET      | Search leaderboard stats by player name                                  |
| [setAvatarStatValues](./setavatarstatvalues.md)                                 | POST     | Update avatar statistics                                                 |
