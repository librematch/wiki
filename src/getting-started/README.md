# Getting Started

Welcome to the LibreMatch developer documentation! This section will help you get started with building applications using the Worlds Edge Link API for Age of Empires games.

## What You Can Build

The Worlds Edge Link API enables you to create:

- **Lobby Browsers** - Display and filter available game lobbies
- **Match Spectator Tools** - View and follow ongoing games
- **Player Tracking** - Monitor specific players' activities
- **Community Tools** - Custom integrations for your local gaming community
- **Statistics Dashboards** - Aggregate and visualize game data

## Choose Your Path

### I Want to Build a Lobby Browser

Start here if you want to create a tool that displays game lobbies and matches.

→ **[Example: Building a Lobby Browser](./example-lobby-browser.md)**

This guide covers:

- Quick start with the [public Community API (no authentication)](../rlink/community/)
- Advanced features using the [authenticated Game API](https://wiki.librematch.org/getting-started/example-lobby-browser#advancedgame_api_authenticated)
- Code examples and best practices
- Response parsing and data handling

### I Have Questions

Check our comprehensive FAQ for quick answers to common questions.

→ **[Frequently Asked Questions](./faq.md)**

Topics covered:

- General API questions
- Authentication and setup
- API usage and filtering
- Development tips
- Troubleshooting

## Quick Links

### API Endpoints

| Endpoint Type                        | Authentication | Use Case                       | Documentation                                                                |
| ------------------------------------ | -------------- | ------------------------------ | ---------------------------------------------------------------------------- |
| [Community API](../rlink/community/) | None required  | Public lobby listings          | [Quick Start Guide](./example-lobby-browser.md#quick-start-community-api)    |
| [Game API](../rlink/game/)           | Steam required | Ongoing matches, detailed data | [Advanced Guide](./example-lobby-browser.md#advanced-game-api-authenticated) |

### Essential Resources

- **[RLINK Documentation](https://wiki.librematch.org/rlink/start)** - Complete API reference
- **[Libre:Match Discord](https://discord.gg/MvuusBxtuB)** - Community support and discussion

### Open Source Projects

**LibreMatch Organization** - [GitHub](https://github.com/librematch)

- **[librematch-collector](https://github.com/librematch/librematch-collector)** - Polling, diffing, parsing and converting data from the Relic Link API for storing in Libre:Match Database
- **[librematch-rlink_client](https://github.com/librematch/librematch-rlink_client)** - Relic Link API-Client generated from OpenAPI
- **[librematch-steam_auth](https://github.com/librematch/librematch-steam_auth)** - Steam authentication proxy for use with Relic Link API
- **[ageLANServer](https://github.com/luskaner/ageLANServer)** - Open source LAN server implementation with model definitions

## Before You Begin

**For Basic Lobby Browsers:**

- No special requirements - just make HTTP requests!
- Recommended: 5-second polling interval with caching

**For Advanced Features (Spectating, Match Data):**

- Steam account with the game purchased
- Node.js or similar environment for authentication
- Understanding of Steam authentication flow

## Need Help?

- Browse the **[FAQ](./faq.md)** for common questions
- Check the **[example implementations](./example-lobby-browser.md)**
- Join the community on **[Discord](https://discord.gg/MvuusBxtuB)**
- Explore **[open source projects](https://github.com/luskaner/ageLANServer)** for working code

## Contributing

Found something missing or incorrect? This documentation is community-maintained. Contributions are welcome to help fellow developers!

---

*Ready to start? Pick a guide above and begin building! *
