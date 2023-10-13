# Source:Matt Rickard, URL:https://matt-rickard.com/rss, language:en-US

## Nagle's Algorithm
 - [https://matt-rickard.com/nagles-algorithm-2](https://matt-rickard.com/nagles-algorithm-2)
 - RSS feed: https://matt-rickard.com/rss
 - date published: 2023-10-12T13:30:30+00:00

200 milliseconds doesn’t sound like a lot, but it’s an eternity for latency-sensitive code (you could travel around the world at the speed of light in 133ms). If you’re working with latency-sensitive code over the network, you might have found that sometimes your requests take much longer than expected. Up to 200ms, even for basic requests on localhost.

Nagle’s Algorithm was introduced in 1984 to reduce the number of packets sent over TCP/IP. Suppose many small data packets are sent over the ne

