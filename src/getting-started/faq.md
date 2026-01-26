## FAQ

### General Questions

**Q: Is there a WebSocket API instead of polling?**

A: The official Worlds Edge Link API does not provide WebSocket/push notifications. You must poll the endpoints. However, third-party services like [aoe2lobby.com](https://aoe2lobby.com/) offer WebSocket APIs that aggregate this data. Some developers have proposed creating a service that polls and converts to push notifications.

---

**Q: Should I use an existing lobby browser?**

A: If you just need basic functionality, existing browsers work well. However, building your own is worthwhile for:

- Custom features for specific communities
- Localization and personalization
- Learning and hobby projects
- Integration with other tools

---

**Q: Do I need authentication for a basic lobby browser?**

A: No! The [[GET] /community/advertisement/findAdvertisements](../rlink/community/advertisement/findadvertisements.md) endpoint on the Community API provides public lobby data without authentication. Authentication is only needed for:

- Viewing ongoing ranked games
- Spectator features
- Detailed match information
- Player-specific filtering

---

### Authentication & Setup

**Q: Steam blocked me from logging in, what do I do?**

A: Too many login attempts trigger Steam's security. Wait some time and it will unblock automatically. To avoid this:

- Don't spam login attempts while testing
- Cache your session ID and reuse it
- Use a dedicated account for your service
- Implement proper retry logic with backoff

---

**Q: Why do I need Buffer.from("RLINK")?**

A: This is a required parameter for the encrypted app ticket to work with the Worlds Edge Link API. The ticket must be created specifically for RLINK authentication, not just for the game itself.

---

**Q: How do I find the current clientLibVersion?**

A: Several methods:

- Use Wireshark to capture game network traffic
- Search the game binary/PE file (hardcoded)
- Check community resources (currently 190+)
- Parse Steam RSS feeds for update announcements

Note: This value changes with game updates, so plan for updates.

---

**Q: Where do I get the game build version (appBinaryChecksum)?**

A: Three options:

- Bottom-left corner when launching the game
- Parse Steam RSS feeds programmatically (see code example above)
- Check community resources after updates

---

### API Usage

**Q: Why are the API responses such a horrible structure?**

A: The Game API uses an internal format that returns positional arrays instead of named JSON objects. This is how the game client expects data. The Community API returns cleaner JSON. For Game API responses:

- Positions are stable (consistent across versions)
- Use reference implementations to understand field mappings
- Consider using third-party APIs for cleaner data

---

**Q: Can I filter results to specific players?**

A: Yes! Although not officially documented:

- Use ''profile_ids=[id1,id2]'' parameter
- Use ''numericTagNames'' and ''numericTagValues'' for other filters
- Filtering happens server-side for profile IDs
- Some filtering (like game type) happens client-side in the official game

---

**Q: Are there rate limits?**

A: Yes, the server implements rate limiting. Best practices:

- Poll at reasonable intervals (5+ seconds)
- Implement client-side caching
- Batch requests when possible
- Monitor for rate limit responses

---

**Q: Can I show ongoing ranked games?**

A: Yes, but it requires the authenticated Game API for the [[GET/POST] /game/advertisement/findObservableAdvertisements](../rlink/game/advertisement/findobservableadvertisements.md) endpoint. The Community API only shows lobbies waiting for players, not matches in progress.

---

### Development

**Q: What should I use for macAddress?**

A: You can use any valid MAC address format (e.g., ''DE-AD-D0-0D-00-00''). The API doesn't validate this strictly.

---

**Q: Is there example code I can reference?**

A: Yes! Check these open source projects:

- [ageLANServer (Go)](https://github.com/luskaner/ageLANServer) - Complete server implementation with model definitions
- Various community tools on GitHub
- Code snippets shared in developer communities

---

**Q: Is it legal to use these APIs?**

A: The Community API is public and intended for community use. For the authenticated Game API:

- Read the [Age of Empires API Usage Guidelines](../rlink/usage.md)
- You must own the game on Steam
- Don't abuse the API or spam requests
- Don't create malicious tools (fake lobbies, spam, etc.)
- Respect rate limits and terms of service

---

**Q: Should I use aoe2lobby.com's API instead?**

A: Consider it if you want:

- Real-time WebSocket updates (no polling)
- Cleaner data format
- Less maintenance (they handle game updates)
- Quick integration

Build your own if you need:

- Complete control over data and features
- Custom filtering or processing
- Independence from third-party services
- Learning experience

---

### Troubleshooting

**Q: I'm not getting a session ID, what's wrong?**

A: Common issues:

- Missing ''Buffer.from("RLINK")'' in ticket creation
- Incorrect Base64 and URI encoding of the auth parameter (the encoding must be combination of **encodeURI(base64(encoding))**)
- Outdated ''clientLibVersion''
- Invalid or expired Steam ticket
- Check all required parameters are present

---

**Q: How do I parse the array response?**

A: The response structure is:

- First element: metadata
- Second element: array of matches
- Each match: array starting with [lobbyId, platformSessionId, ...]

See the ageLANServer repository for complete field mappings in the ''advertisement.go'' model.

---

**Q: Do I need a separate authentication service?**

A: It's recommended to separate authentication from your main app:

- Keeps Steam credentials isolated
- Can run on a dedicated account
- Easier to manage session refresh logic
- Can serve multiple clients

---

## Contributing

This documentation is community-maintained. If you discover new endpoints, parameters, or corrections, please contribute back to help other developers!

---

*Last updated: December 2025 *

*Based on community research and shared knowledge *
