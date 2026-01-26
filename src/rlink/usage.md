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
