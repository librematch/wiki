# Authentication

Sometimes resources will need authorization to be accessed by privileged community members. Such members could be tournament organizers and admins that want to set up a schedule within the backend to delay the access to certain player information for a limited amount of time. This could be needed during tournaments, so people aren't able to find out results of matches before they are officially concluded (e.g. in case of casting recorded games) and spoil other people with the results.

The Relic Link ID aka RLINK_ID is a unique identifier for every player on the Relic Link platform, no matter if the person bought a game on Steam or Microsoft Store.

Authentication for a player on the Steam platform could be achieved by utilizing [web browser based authentication with Steam OpenID](https://partner.steamgames.com/doc/features/auth#website).
