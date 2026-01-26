# Automatch2 Endpoints

Endpoints for the newer ranked matchmaking system.

> **Authentication:** All endpoints in this section require Steam authentication.

## Endpoints

| Endpoint                                | Method | Description                                  |
| --------------------------------------- | ------ | -------------------------------------------- |
| [getAutomatchMap](./getautomatchmap.md) | GET    | Get available ranked maps with map pool info |
| [polling](./polling.md)                 | GET    | Poll for matchmaking status updates          |
| [stoppolling](./stoppolling.md)         | POST   | Stop matchmaking polling                     |
| [updateStatus](./updatestatus.md)       | POST   | Update matchmaking status                    |
