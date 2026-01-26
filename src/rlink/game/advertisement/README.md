# Advertisement Endpoints

Endpoints for managing game lobbies and advertisements. These endpoints handle lobby creation, joining, spectating, and lobby state management.

> **Authentication:** All endpoints in this section require Steam authentication.

## Endpoints

| Endpoint                                                          | Method   | Description                                                          |
| ----------------------------------------------------------------- | -------- | -------------------------------------------------------------------- |
| [findAdvertisements](./findadvertisements.md)                     | GET      | Search for game lobbies with filters (profile IDs, match type, mods) |
| [findObservableAdvertisements](./findobservableadvertisements.md) | GET/POST | Find ongoing matches available for spectating                        |
| [getAdvertisements](./getadvertisements.md)                       | GET      | Get list of available game lobbies                                   |
| [getLanAdvertisements](./getlanadvertisements.md)                 | GET      | Get LAN game lobbies                                                 |
| [host](./host.md)                                                 | POST     | Create a new game lobby                                              |
| [join](./join.md)                                                 | POST     | Join an existing game lobby                                          |
| [leave](./leave.md)                                               | POST     | Leave a game lobby                                                   |
| [startObserving](./startobserving.md)                             | POST     | Start spectating a match                                             |
| [stopObserving](./stopobserving.md)                               | POST     | Stop spectating a match                                              |
| [update](./update.md)                                             | POST     | Update lobby settings                                                |
| [updatePlatformLobbyID](./updateplatformlobbyid.md)               | POST     | Update the Steam lobby ID                                            |
| [updateState](./updatestate.md)                                   | POST     | Update lobby state (e.g., starting game)                             |
| [updateTags](./updatetags.md)                                     | POST     | Update lobby tags/metadata                                           |
