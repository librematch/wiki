# Party Endpoints

Endpoints for match management, including reporting match results, managing peer connections, uploading replays, and handling singleplayer sessions.

> **Authentication:** All endpoints in this section require Steam authentication.

## Endpoints

| Endpoint                                                      | Method | Description                                                  |
| ------------------------------------------------------------- | ------ | ------------------------------------------------------------ |
| [peerAdd](./peeradd.md)                                       | POST   | Register a peer connection for match participants            |
| [peerUpdate](./peerupdate.md)                                 | POST   | Update peer connection status                                |
| [reportMatch](./reportmatch.md)                               | POST   | Submit match results with player stats and replay upload URL |
| [createOrReportSingleplayer](./createorreportsingleplayer.md) | POST   | Create or report results for a singleplayer session          |
| [finalizeReplayUpload](./finalizereplayupload.md)             | POST   | Confirm replay file upload completion                        |
| [sendMatchChat](./sendmatchchat.md)                           | POST   | Send chat messages during a match                            |
