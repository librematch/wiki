# Building a Lobby Browser for Age of Empires II: Definitive Edition

This guide covers how to interact with the [Worlds Edge Link API](../rlink/) to build custom lobby browsers and spectator tools for Age of Empires games.

## Overview

The [Worlds Edge Link API](../rlink/) provides two main approaches for accessing lobby data:

- **[Community API](../rlink/community/)** - Public, unauthenticated access to lobby listings
- **[Game API](../rlink/game/)** - Authenticated access to ongoing matches and detailed game data

For simpler integration, you can also use the **[aoe2lobby.com WebSocket API](https://wiki.librematch.org/getting-started/example-lobby-browser#alternativewebsocket_api)** which provides real-time updates without polling.

## Quick Start: Community API

### Basic Lobby Listing

For a simple lobby browser, use the community endpoint [/advertisement/findAdvertisements](../rlink/community/advertisement/findadvertisements.md):

```
GET https://aoe-api.worldsedgelink.com/community/advertisement/findAdvertisements?title=age2
```

**Features:**

- No authentication required
- Public lobby data only
- Recommended polling interval: 5 seconds with client-side caching
- No WebSocket/push notification support

This is sufficient for most lobby browsing use cases.

## Advanced: Game API (Authenticated)

For accessing ongoing matches and spectator features, you'll need to authenticate using Steam.

We provide a [reference implementation written in Python](https://github.com/librematch/librematch-steam_auth) that you may want to have a look at.

### Prerequisites

- Steam account with the game purchased
- Node.js environment (examples use JavaScript)
- ''steam-user'' npm package for Steam authentication

### Authentication Flow

#### Step 1: Create Encrypted App Ticket

```javascript
const SteamUser = require('steam-user');
const client = new SteamUser();

// Login to Steam first (with your credentials)
await client.logOn({...});

// Create encrypted app ticket
const APP_ID = 813780; // AoE2:DE
const eticket = await client.createEncryptedAppTicket(
    APP_ID, 
    Buffer.from("RLINK")  // Important: Include RLINK buffer
);

// Encode for API use
const auth = encodeURIComponent(
    eticket.encryptedAppTicket.toString('base64')
);
```

**Important Notes:**

- Always include ''Buffer.from("RLINK")'' as the second parameter
- Don't spam login attempts - Steam will rate limit and require verification codes
- The auth string must be both Base64 and URI encoded

#### Step 2: Platform Login

```javascript
const url = `https://aoe-api.worldsedgelink.com/game/login/platformlogin?`
    + `accountType=STEAM`
    + `&activeMatchId=-1`
    + `&alias=${alias}`
    + `&appID=${APP_ID}`
    + `&auth=${auth}`  // Your encoded ticket from Step 1
    + `&callNum=0`
    + `&clientLibVersion=190`  // Update as game updates
    + `&country=US`
    + `&installationType=windows`
    + `&language=en`
    + `&macAddress=DE-AD-D0-0D-00-00`  // Can be any value
    + `&majorVersion=4.0.0`
    + `&minorVersion=0`
    + `&platformUserID=${steamID}`
    + `&timeoutOverride=0`
    + `&title=age2`;

const response = await axios.post(url);
const sessionId = response.data.sessionID; // Save this!
```

**Key Parameters:**

- ''clientLibVersion'' - Currently 190+ (changes with game updates)
- ''macAddress'' - Can be any valid format
- ''auth'' - Your encoded ticket from Step 1
- Returns a ''sessionID'' needed for subsequent requests

### Getting Game Build Version

The ''appBinaryChecksum'' parameter requires the current game build version. You can obtain this programmatically:

```javascript
const getBuildVersion = async (appId) => {
    const rss = await fetch(
        `https://store.steampowered.com/feeds/news/app/${appId}/`
    );
    const parser = new XMLParser();
    const feed = parser.parse(await rss.text());
    
    let lastUpdateTitle = feed?.rss?.channel?.item
        ?.map(e => e.title)
        .find(e => e.match(/(update.[0-9]+)/gi));
        
    return parseInt(
        lastUpdateTitle.slice(
            lastUpdateTitle.search(/update/gi) + "update".length
        )
    );
}
```

Alternatively, check the bottom-left corner when launching the game.

### Finding Observable Matches

Once authenticated, query ongoing games:

```javascript
const url = `https://aoe-api.worldsedgelink.com/game/advertisement/findObservableAdvertisements?`
    + `appBinaryChecksum=${gameVersion}`
    + `&callNum=0`
    + `&count=50`
    + `&dataChecksum=0`
    + `&desc=1`
    + `&matchType_id=0`
    + `&modName=INVALID`
    + `&modDLLChecksum=0`
    + `&modDLLFile=INVALID`
    + `&modVersion=INVALID`
    + `&start=0`
    + `&sortOrder=1`
    + `&versionFlags=56950784`
    + `&sessionID=${sessionId}`
    + `&connect_id=${sessionId}`;

const response = await axios.get(url);
```

### Filtering Options

#### By Player Profiles

```
&profile_ids=[123456,789012]
```

Filter matches to only show games with specific player profile IDs.

#### By Numeric Tags

```
&numericTagNames=["HasPassword"]
&numericTagValues=[0]
```

Common tags include:

- ''HasPassword'' - Filter by password-protected status
- Other tags available but not fully documented

## Response Format

**Warning:** The Game API returns responses in an obscured array format that is not user-friendly.

```javascript
// Example response structure
[
    someMetadata,
    [  // Array of matches
        [lobbyId, platformSessionId, ...otherFields],
        [lobbyId, platformSessionId, ...otherFields],
        // etc.
    ]
]
```

**Parsing Help:**

- Responses are positional arrays, not named objects
- Element positions are stable across API versions
- See [this reference implementation](https://github.com/luskaner/ageLANServer/blob/dff2ff7d0c7239fad522ce26063986b2dc8001e1/server/internal/models/advertisement.go) for field mappings
- The second element of the response contains the array of advertisements
- Each advertisement follows the order: lobby ID, platform session ID, followed by other fields

## Alternative: WebSocket API

For simpler integration, consider using the aoe2lobby.com WebSocket API:

- Real-time updates (no polling needed)
- Clean, documented data format
- Provides schema information on connection
- Free to use for community projects
- Live for 8+ months with proven reliability

### Connection

**WebSocket URL:** ```
wss://data.aoe2lobby.com/ws/

````
The API supports subscribing to different data feeds by sending JSON subscription messages.

### Subscription Examples
**Subscribe to spectate matches:**
```json

{"action":"subscribe","type":"matches","context":"spectate"}
````

**Subscribe to lobby matches:**

```json
{ "action": "subscribe", "type": "matches", "context": "lobby" }
```

**Subscribe to specific Elo types:**

```json
{
    "action": "subscribe",
    "type": "elotypes",
    "context": "lobby",
    "ids": ["1223", "3", "4"]
}
```

**Subscribe to specific players:**

```json
{
    "action": "subscribe",
    "type": "players",
    "context": "lobby",
    "ids": ["3920944"]
}
```

Player status updates include current status, match ID, and Steam lobby ID:

```json
{
    "player_status": {
        "19501096": {
            "status": "lobby",
            "matchid": "412015195",
            "steam_lobbyid": "109775244730862406"
        }
    }
}
```

### Resources

- Instructions: aoe2lobby.com chat section
- Discord support: [aoe2lobby Discord](https://discord.gg/8BAShCGS)

## Best Practices

Read the [Age of Empires API Usage Guidelines](../rlink/usage.md)!

### Rate Limiting

- Server implements rate limiting - don't spam requests
- Use reasonable polling intervals (5+ seconds)
- Cache results when possible
- Consider batch operations for multiple profile lookups

### Version Management

- ''clientLibVersion'' changes with game updates
- Can be found by inspecting network traffic with Wireshark
- Hardcoded in the game binary/PE file
- Current version as of late 2024: 190+

### Authentication

- Session IDs persist for some time
- Avoid repeated Steam logins (triggers verification)
- Use a dedicated Steam account for service authentication
- Consider running auth service separately from main app

## Additional Resources

### Documentation & Projects

- **Lib:reMatch Steam-Auth:** [Reference implementation (Python)](https://github.com/librematch/librematch-steam_auth)
- **Lib:reMatch OAPI-RLINK-Client:** [Generated example python client incl. openapi.yaml](https://github.com/librematch/librematch-rlink_client)
- **Lib:reMatch Wiki:** [RLINK documentation](https://wiki.librematch.org/rlink/game/start)
- **ageLANServer:** [Open source server implementation](https://github.com/luskaner/ageLANServer) with model definitions
- **aoe2lobby.com:** WebSocket API for easier integration
- **aoe2recs.com:** Example browser implementation

### Community Support

- AOE API developer channels
- [Libre:Match Discord](https://discord.gg/MvuusBxtuB)
- Various open source projects with working examples

## Contributing

This documentation is community-maintained. If you discover new endpoints, parameters, or corrections, please contribute back to help other developers!

---

*Last updated: December 2025 *

*Based on community research and shared knowledge *
