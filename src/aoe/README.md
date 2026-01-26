# Age of Empires Official API

Documentation for the official Age of Empires API at ageofempires.com.

## API Root

- Production: `https://api.ageofempires.com`
- Development: `https://api-dev.ageofempires.com` (for /Poll only)

## Endpoints

### Main APIs

- [API v1](./api/v1/) - Version 1 endpoints (bugs, mods)
- [API v2](./api/v2/) - Version 2 endpoints (leaderboards)
- [API v4](./api/v4/) - Version 4 endpoints (mods)

### Game-Specific APIs

- [Age I: DE](./api/agede/) - Age of Empires: Definitive Edition
- [Age II: DE](./api/ageii/) - Age of Empires II: Definitive Edition
- [Age III: DE](./api/ageiii/) - Age of Empires III: Definitive Edition
- [Age IV](./api/ageiv/) - Age of Empires IV

### Other Endpoints

- [Web API](./webapi/) - Web-related endpoints
- [Poll API](./poll/) - Polling endpoints

### Special

#### Mod Pictures

[Example Request](https://cdn.ageofempires.com/aoe-mods/2/3903/3ced7b44.png)

#### Server Status

[Example Request](https://cdn.ageofempires.com/aoe/rl-server-status.json)

#### CountryList

[Example Request](https://www.ageofempires.com/wp-content/themes/ageOfEmpires/resources/assets/json/CountryList.json)

#### errorMessaging

[Example Request](https://www.ageofempires.com/wp-admin/admin-ajax.php?action=getErrorMsg)

#### wordpressAjax

[Example Request](https://www.ageofempires.com/wp-admin/admin-ajax.php)

### Recorded games

```
https://aoe.ms/replay/?gameId=<game_id>&profileId=<profile_id>
```

[Example request](https://aoe.ms/replay/?gameId=156900198&profileId=2858362)

| parameter | type  | value     | comments |
| --------- | ----- | --------- | -------- |
| gameId    | int64 | 156900198 |          |
| profileId | int64 | 2858362   |          |

Where <profile_id> is the perspective of the recorded game. Basically from which client it was uploaded.
Matters for view lock.

## API-Endpoints as JSON
