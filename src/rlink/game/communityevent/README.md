# Community Event Endpoints

Endpoints for time-limited community events, including seasonal events, ranked seasons, and special celebrations like anniversary events. Events can contain challenges, login rewards, and leaderboard configurations.

> **Authentication:** All endpoints in this section require Steam authentication.

## Endpoints

| Endpoint                                                        | Method | Description                                                                        |
| --------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------- |
| [getAvailableCommunityEvents](./getavailablecommunityevents.md) | GET    | Get all active community events with season data, rank configurations, and rewards |
| [getEventChallengeProgress](./geteventchallengeprogress.md)     | GET    | Get player's progress on event-specific challenges                                 |
| [getEventStats](./geteventstats.md)                             | GET    | Get player statistics for a specific event (rating, ranking, etc.)                 |
