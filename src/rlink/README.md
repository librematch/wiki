# WorldsEdgeLink API

## Age of Empires API Usage Guidelines

Please check the following [Age of Empires API Usage Guidelines](./usage.md) before you design or implement anything.

## API Root

https://aoe-api.worldsedgelink.com/

### Endpoints

- [Community API](./community/) - Public, unauthenticated endpoints
- [Game API](./game/) - Authenticated endpoints requiring Steam login

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

## Authentication

Check our [Authentication Helper](https://github.com/librematch/librematch-steam_auth)

## General Notes

Some stuff is zlib-compressed. E.g. inside `slotinfo` there's a `metaData` field that seems to be a **two-pass base64 string holding binary data**.

Example

Heres an example from the slotinfo property:

```
$ echo 'eNrVkF1PwjAUhv0tvR6GMjYniTeDVWfcgLJ2gvGibl0o3QduEyHG/y6dgUiMF8YLs6uevufknCcP7GkPb2BdFolIuZsnxbmIwcCyTN0yLzVQ1awWRe6OwABqoOYsU2VXAwmLDo39r2QRP5a5vOMbnh5/HqujZbBbNxMdtUZkfMJLVLKMe7NmTlSYs3jXXFE3X6omznjNRqxmYABceWtjguwpQf1pGKvXCe6XNmkybM+6TW+MHQkDiUtPGuYsoGMiocqHFMkdzekidNav8xUaRjCdP11vV6y3haGMQ9/x8/2cjREyAoixT4znuZ5OKKJI5VO6uKHZUhBC1T7bE+4VeNe+u+vAE22dL97giTfVOYj7rP9krvuTud9S9lpBqbeCst8KSqMVlGYrKC/+ifLx7APyMc1P' | base64 -d | zlib-flate -uncompress

12,[{"profileInfo.id":8863869,"stationID":1,"teamID":0,"factionID":0,"raceID":0,"rankLevel":0,"rankMatchTypeID":-1,"timePerFrameMS":0,"isReady":1,"status":0,"metaData":"IkJBRUFBQUF4QWdBQUFETXhBUUFBQURBS0FBQUFOREk1TkRrMk56STVOUk1BQUFCVFkyVnVZWEpwYjFCc1lYbGxja2x1WkdWNENnQUFBRFF5T1RRNU5qY3lPVFVFQUFBQVZHVmhiUUVBQUFBMiI="},{"profileInfo.id":-1,"stationID":-1,"teamID":1,"factionID":-1,"raceID":-1,"rankLevel":0,"rankMatchTypeID":-1,"timePerFrameMS":0,"isReady":0,"status":0,"metaData":""},{"profileInfo.id":-1,"stationID":-1,"teamID":2,"factionID":-1,"raceID":-1,"rankLevel":0,"rankMatchTypeID":-1,"timePerFrameMS":0,"isReady":0,"status":0,"metaData":""},{"profileInfo.id":-1,"stationID":-1,"teamID":3,"factionID":-1,"raceID":-1,"rankLevel":0,"rankMatchTypeID":-1,"timePerFrameMS":0,"isReady":0,"status":0,"metaData":""},{"profileInfo.id":-1,"stationID":-1,"teamID":4,"factionID":-1,"raceID":-1,"rankLevel":0,"rankMatchTypeID":-1,"timePerFrameMS":0,"isReady":0,"status":0,"metaData":""},{"profileInfo.id":-1,"stationID":-1,"teamID":5,"factionID":-1,"raceID":-1,"rankLevel":0,"rankMatchTypeID":-1,"timePerFrameMS":0,"isReady":0,"status":0,"metaData":""},{"profileInfo.id":-1,"stationID":-1,"teamID":6,"factionID":-1,"raceID":-1,"rankLevel":0,"rankMatchTypeID":-1,"timePerFrameMS":0,"isReady":0,"status":0,"metaData":""},{"profileInfo.id":-1,"stationID":-1,"teamID":7,"factionID":-1,"raceID":-1,"rankLevel":0,"rankMatchTypeID":-1,"timePerFrameMS":0,"isReady":0,"status":0,"metaData":""}]
```

There are also options that use `b64(zlib(b64(data)))`.
