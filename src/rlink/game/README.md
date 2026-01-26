# Game API (Authenticated)

The Game API provides authenticated access to Age of Empires game data. Requires Steam authentication.

**Base URL:** `https://aoe-api.worldsedgelink.com/game/`

## Authentication

Steam authentication is required. See the [Getting Started Guide](../../getting-started/example-lobby-browser.md#advanced-game-api-authenticated) for authentication flow details.

You can also check our [Steam Auth Helper](https://github.com/librematch/librematch-steam_auth) reference implementation.

## OpenAPI Specification

The OpenAPI spec for the `/game` endpoints can be found at [librematch-rlink_client](https://github.com/librematch/librematch-rlink_client).

## Reverse Engineering

If you see that something is missing, you can use [Wireshark](https://www.wireshark.org) to capture and analyze game network traffic.

## Endpoints

### Login

Session management.

- [platformlogin](./login/platformlogin.md) - Authenticate with Steam
- [logout](./login/logout.md) - End session

### Account

Account management.

- [getProfileName](./account/getprofilename.md) - Get profile name
- [setProfileName](./account/setprofilename.md) - Set profile name

### Achievement

Player achievements (authenticated).

- [getAchievements](./achievement/getachievements.md) - Get achievements
- [grantAchievement](./achievement/grantachievement.md) - Grant achievement

### Advertisement

Game lobbies and matches.

- [findObservableAdvertisements](./advertisement/findobservableadvertisements.md) - Find spectatable matches
- [getAdvertisements](./advertisement/getadvertisements.md) - Get lobby listings
- [host](./advertisement/host.md) - Host a game

### Automatch

Ranked matchmaking.

- [getAutomatchMap](./automatch/getautomatchmap.md) - Get automatch map pool

### Automatch2

Enhanced matchmaking.

- [cancelSearch](./automatch2/cancelsearch.md) - Cancel matchmaking search
- [startSearch](./automatch2/startsearch.md) - Start matchmaking search
- [getMatchInfo](./automatch2/getmatchinfo.md) - Get match information

### Challenge

Challenge system.

- [getChallenges](./challenge/getchallenges.md) - Get available challenges
- [getRewardDefinitions](./challenge/getrewarddefinitions.md) - Get reward definitions

### Chat

In-game chat.

- [getChatChannels](./chat/getchatchannels.md) - Get chat channels
- [getOfflineMessages](./chat/getofflinemessages.md) - Get offline messages

### Clan

Clan management (authenticated).

- [create](./clan/create.md) - Create a clan
- [getClanInfoFull](./clan/getclaninfofull.md) - Get clan details
- [join](./clan/join.md) - Join a clan
- [leave](./clan/leave.md) - Leave a clan

### Cloud

Cloud save functionality.

- [getFileURL](./cloud/getfileurl.md) - Get cloud file URL
- [setFile](./cloud/setfile.md) - Upload to cloud

### Community Event

Event participation.

- [getAvailableCommunityEvents](./communityevent/getavailablecommunityevents.md) - List events
- [claimReward](./communityevent/claimreward.md) - Claim event reward

### Invitation

Game invitations.

- [sendInvitation](./invitation/sendinvitation.md) - Send game invite
- [extendInvitation](./invitation/extendinvitation.md) - Extend invitation

### Item

Item management.

- [getItems](./item/getitems.md) - Get inventory items
- [signItems](./item/signitems.md) - Sign items

### Leaderboard

Rankings (authenticated).

- [getLeaderBoard2](./leaderboard/getleaderboard2.md) - Get leaderboard
- [getRecentMatchHistory](./leaderboard/getrecentmatchhistory.md) - Match history

### News

Game news.

- [getNews](./news/getnews.md) - Get news feed

### Party

Party system.

- [create](./party/create.md) - Create party
- [join](./party/join.md) - Join party
- [leave](./party/leave.md) - Leave party
- [sendMessage](./party/sendmessage.md) - Send party message

### Player Report

Report players.

- [report](./playerreport/report.md) - Report a player

### Relationship

Friends and blocks.

- [getRelationships](./relationship/getrelationships.md) - Get friend list
- [setPresence](./relationship/setpresence.md) - Set online presence
