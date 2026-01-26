# Data Sources

This section documents all available data sources that LibreMatch uses to collect Age of Empires game data.

## WorldsEdgeLink API (RLINK)

The primary source for game data is the WorldsEdgeLink API.

- **[WorldsEdgeLink Introduction](../../rlink/)** - Overview and general information
- **[API Changelog](./changelog/)** - History of API changes

### Endpoints

| API                                     | Authentication | Description                                                                               |
| --------------------------------------- | -------------- | ----------------------------------------------------------------------------------------- |
| [Community API](../../rlink/community/) | None           | Public lobby listings, leaderboards, achievements. Most data should be fetched from here. |
| [Game API](../../rlink/game/)           | Steam required | Ongoing matches, detailed data. Use sparingly for essential features only.                |

## Other Data Sources

- **[Age of Empires Official API](../../aoe/)** - Official API at ageofempires.com
- **[Steam Web API](../../steam/)** - Steam platform integration

## Miscellaneous

- **[gRPC API (CA:DE)](../../grpc/)** - gRPC-based API for Command & Conquer: Definitive Edition
