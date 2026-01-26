# Login Endpoints

Endpoints for authentication and session management. These are the core endpoints needed to establish an authenticated connection to the API.

> **Authentication:** `platformlogin` creates the session; other endpoints require an active session.

## Endpoints

| Endpoint                            | Method | Description                                  |
| ----------------------------------- | ------ | -------------------------------------------- |
| [platformlogin](./platformlogin.md) | POST   | Authenticate with Steam and create a session |
| [logout](./logout.md)               | POST   | End the current session                      |
| [readSession](./readsession.md)     | GET    | Read/validate current session state          |

## Authentication Flow

1. Create an encrypted Steam app ticket with `Buffer.from("RLINK")`
2. Call `platformlogin` with the Base64+URI encoded ticket
3. Store the returned `sessionID` for subsequent requests
4. Include `sessionID` and `connect_id` in all authenticated requests
