## Lobby creation (hacky)

- Problem: How can we create custom lobbies in an automated way from outside the game? And who does it? How to make that as easy as possible?
- this might be a bit reverse engineering and an external tool, but I assume not impossible (other ideas how to interface with the game are welcome)

1. this GPLv3-fork of the AoE2DE SDK (C++) might be helpful?
1. or a custom python script that reads the game?
1. autohotkey script?
1. check if possible: what about reversing the API endpoint on their backend and sending a request for opening a lobby in the name of any user that matched?
1. can the user itself join via a link?
1. is the lobby kept open automatically? or do we need to simulate some user activity in the lobby until everyone joined?

- theoretically could be done later if the UX is nice and easy also without
- lobby id once created should be distributed to the participants as a direct link `aoe2de:\/\/0/89697553` people can just click
