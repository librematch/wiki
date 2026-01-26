# Challenge Endpoints

Endpoints for managing in-game challenges and tracking challenge progress. Challenges are time-limited objectives that reward players with items upon completion.

> **Authentication:** All endpoints in this section require Steam authentication.

## Endpoints

| Endpoint                                                                | Method | Description                                            |
| ----------------------------------------------------------------------- | ------ | ------------------------------------------------------ |
| [getChallenges](./getchallenges.md)                                     | GET    | Get available challenges with encrypted data signature |
| [getChallengeProgress](./getchallengeprogress.md)                       | GET    | Get current player's challenge progress                |
| [getChallengeProgressByProfileID](./getchallengeprogressbyprofileid.md) | GET    | Get challenge progress for a specific profile          |
| [updateProgressBatched](./updateprogressbatched.md)                     | POST   | Update progress for multiple challenges at once        |
