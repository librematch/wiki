# Cloud Endpoints

Endpoints for cloud storage operations, including downloading game data files and retrieving temporary credentials for Azure blob storage access.

> **Authentication:** All endpoints in this section require Steam authentication.

## Endpoints

| Endpoint                                      | Method   | Description                                                               |
| --------------------------------------------- | -------- | ------------------------------------------------------------------------- |
| [getFileURL](./getfileurl.md)                 | GET/POST | Get download URLs for cloud-hosted game files (SGA archives, locale data) |
| [getTempCredentials](./gettempcredentials.md) | GET      | Get temporary SAS credentials for Azure blob storage access               |
