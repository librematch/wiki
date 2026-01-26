# Architecture (Overview)

## Example (Bright Sky)

[Bright Sky](https://brightsky.dev/) pulls weather data from DWD and implements a JSON-API on top of it for its users.
Their architecture looks like on the image on the right side. It's some kind of the same what we also want to achieve.

This is taken from the [Official repository](https://github.com/jdemaeyer/brightsky/#architecture):

- The brightsky worker, which leverages the logic contained in the brightsky Python package to retrieve weather records from the DWD server, parse them, and store them in a database. It will periodically poll the DWD servers for new data.
- The brightsky web server (API), which serves as gate to our database and processes all queries for weather records coming from the outside world.
- A PostgreSQL database consisting of two relevant tables:

1. sources contains information on the locations for which we hold weather records, and
1. weather contains the history of actual meteorological measurements (or forecasts) for these locations.

- A Redis server, which is used as the backend of the worker's task queue.

### LibreMatch

Basically, we should poll the Relic Link API endpoints for all data every so many seconds (this time is our minimum latency for our whole system).
So the time frame in which we see certain information (Match infos, wins of games) and could deliver information to our API.

Then we parse the results into a data structure of ourselves to make error handling easier and also deal with types of data and not handle everything as a huge JSON-Array that is being exposed by the Relic Link API. This data we send to the database, which is our persistence layer. From our persistence layer, we are able to request data for our endpoints that we expose to the users.
Some endpoints may require a Pub/Sub API (e.g. live updates for match information), some are fine with the usual REST-API approach.
