# Leaderboard Endpoints (Community)

Public endpoints for querying leaderboards, player statistics, and match history without authentication. These are the most commonly used endpoints for third-party tools and websites.

> **Note:** These are unauthenticated public endpoints. For authenticated leaderboard operations, see [/game/leaderboard](../../game/leaderboard/).

## Endpoints

| Endpoint                                                  | Method | Description                                       |
| --------------------------------------------------------- | ------ | ------------------------------------------------- |
| [getAvailableLeaderboards](./getavailableleaderboards.md) | GET    | Get list of available leaderboards with metadata  |
| [getLeaderBoard2](./getleaderboard2.md)                   | GET    | Get leaderboard rankings with player stats        |
| [getPersonalStat](./getpersonalstat.md)                   | GET    | Get a player's statistics across all leaderboards |
| [getAvatarStatForProfile](./getavatarstatforprofile.md)   | GET    | Get avatar/profile stats for a player             |
| [getMatchHistory](./getmatchhistory.md)                   | GET    | Get match details by match ID(s)                  |
| [getRecentMatchHistory](./getrecentmatchhistory.md)       | GET    | Get a player's recent match history               |
| [getReplayFiles](./getreplayfiles.md)                     | GET    | Get signed download URLs for replay files         |
