# Source:Matt Rickard, URL:https://matt-rickard.com/rss, language:en-US

## Pitfalls of Database Migrations
 - [https://matt-rickard.com/pitfalls-of-database-migrations](https://matt-rickard.com/pitfalls-of-database-migrations)
 - RSS feed: https://matt-rickard.com/rss
 - date published: 2023-10-03T13:30:44+00:00

Database migrations sound difficult but are even more difficult in practice. Unlike stateless code, they are an arrow in time.

 1. Development / production parity is impossible. You can (and should) try to recreate production state as much as possible. This is much easier at the API and web tiers of your application. There might be different endpoints, different API keys, or different network rules, but there are workarounds for coercing them to be somewhat reproducible between environments. Wh

