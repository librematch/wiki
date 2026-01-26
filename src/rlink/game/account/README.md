# Account Endpoints

Endpoints for managing player profiles and account settings.

> **Authentication:** All endpoints in this section require Steam authentication.

## Endpoints

| Endpoint                                                  | Method | Description                          |
| --------------------------------------------------------- | ------ | ------------------------------------ |
| [findProfiles](./findprofiles.md)                         | GET    | Search for player profiles by name   |
| [findProfilesByPlatformId](./findprofilesbyplatformid.md) | GET    | Find profiles by Steam ID or Xbox ID |
| [getProfileName](./getprofilename.md)                     | GET    | Get a player's display name          |
| [getProfileProperty](./getprofileproperty.md)             | GET    | Get profile properties/settings      |
| [setAvatarMetadata](./setavatarmetadata.md)               | POST   | Update avatar metadata               |
| [setLanguage](./setlanguage.md)                           | POST   | Set preferred language               |
