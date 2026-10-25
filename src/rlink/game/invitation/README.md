# Invitation Endpoints

Endpoints for managing game lobby invitations, allowing players to invite others to join their game or cancel pending invitations.

> **Authentication:** All endpoints in this section require Steam authentication.

## Endpoints

| Endpoint                                    | Method | Description                                    |
| ------------------------------------------- | ------ | ---------------------------------------------- |
| [extendInvitation](./extendinvitation.md)   | POST   | Send a game lobby invitation to another player |
| [replyToInvitation](./replytoinvitation.md) | POST   | Answer a received invitation (accept/decline)  |
| [cancelInvitation](./cancelinvitation.md)   | POST   | Cancel a pending invitation                    |

The full party invitation sequence, including the WSS messages exchanged by the
inviter and the invitee, is documented in [notes](./notes.md).
