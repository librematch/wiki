# Community API

The Community API provides public, unauthenticated access to Age of Empires game data.

**Base URL:** `https://aoe-api.worldsedgelink.com/community/`

## Rate Limits

The rate limit for requests to the Community API is **50 requests per second**.

## OpenAPI Specification

The OpenAPI spec for the `/community` endpoints can be found at [librematch-rlink_client](https://github.com/librematch/librematch-rlink_client).

## Endpoints

### Advertisement

Lobby and game listings.

- [findAdvertisements](./advertisement/findadvertisements.md) - Find available game lobbies

### Achievement

Player achievements.

- [getAvailableAchievements](./achievement/getavailableachievements.md) - List available achievements
- [getAchievements](./achievement/getachievements.md) - Get player achievements

### Clan

Clan information.

- [find](./clan/find.md) - Search for clans
- [getClanInfoFull](./clan/getclaninfofull.md) - Get detailed clan information

### Community Event

Community events and challenges.

- [getAvailableCommunityEvents](./communityevent/getavailablecommunityevents.md) - List available events

### External

External service integrations.

- [proxysteamuserrequest](./external/proxysteamuserrequest.md) - Steam user data proxy

### Item

In-game items and inventory.

- [getItems](./item/getitems.md) - Get available items

### Leaderboard

Player rankings and statistics.

- [getLeaderBoard2](./leaderboard/getleaderboard2.md) - Get leaderboard data
- [getRecentMatchHistory](./leaderboard/getrecentmatchhistory.md) - Get recent match history
- [getStatGroupsByProfileIDs](./leaderboard/getstatgroupsbyprofileids.md) - Get stats by profile IDs

### News

Game news and announcements.

- [getNews](./news.md) - Get game news
