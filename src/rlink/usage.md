## Age of Empires API Usage Guidelines

### Rate Limits and Access Patterns

1. The game API has rate limits of approximately 200 requests per minute
1. Rate limit violations trigger a 429 HTTP error
1. Recommended configuration: Implement a throttler at 100 requests per 30 seconds for safety

### Recommended Access Patterns

Safe to access:

1. Ongoing games
1. Match histories
1. Leaderboards

### Optimization Strategy

Use a dual-API approach:

1. Game API
   - Primary use: Fetching ongoing observable games
   - Expected usage: 10-15 requests per minute
2. Community API
   - Use for match histories and leaderboards
   - Benefits from higher rate limits
   - Reduces load on main game API

### Actions to Avoid

1. Accessing chat channels
1. Accessing presence-related features
1. Making POST requests
1. Creating lobbies via API
1. Any other write operations

### Error Handling

Implement logging for rate limit errors (HTTP 429) to monitor API usage patterns

### Request Headers

Include a `User-Agent` header that identifies your project and
provides contact details (e.g. email, Discord ID). This is good
practice for any API you consume, not just Age of Empires.

```
User-Agent: MyProject/1.0 (contact@example.com; Discord: user#1234)
```

### Timeouts

Set request timeouts generously. Some endpoints (especially
`getRecentMatchHistory`) can take longer to respond. A timeout
of 5 seconds is too short -- use longer timeouts (15-30 seconds
recommended) to avoid terminating requests that are still being
processed server-side.

Short client-side timeouts cause the server to log 499 status
codes (client closed connection). At scale this can trigger
server-side alerts and be mistaken for connectivity issues,
which puts unnecessary burden on the operations team. In the
worst case your IP may be banned to protect the service.

### Self-Throttling on Errors

When you encounter timeouts or errors, log them and
self-throttle. Do not retry aggressively. Play as nicely as
possible with the game servers and investigate issues proactively.
