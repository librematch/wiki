# Relationship Endpoints

Endpoints for managing social relationships between players, including friends lists, blocked users, and online presence status.

> **Authentication:** All endpoints in this section require Steam authentication.

## Endpoints

| Endpoint                                        | Method | Description                                             |
| ----------------------------------------------- | ------ | ------------------------------------------------------- |
| [getRelationships](./getrelationships.md)       | GET    | Get player's friends, blocked users, and recent players |
| [getPresenceData](./getpresencedata.md)         | GET    | Get online status and presence data for related players |
| [setPresence](./setpresence.md)                 | POST   | Set player's online presence status                     |
| [setPresenceProperty](./setpresenceproperty.md) | POST   | Update a specific presence property                     |
| [ignore](./ignore.md)                           | POST   | Add a player to the blocked/ignored list                |
| [clearRelationship](./clearrelationship.md)     | POST   | Remove a relationship (unfriend, unblock)               |
