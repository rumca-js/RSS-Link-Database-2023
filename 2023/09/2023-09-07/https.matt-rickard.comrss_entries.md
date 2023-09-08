# Source:Matt Rickard, URL:https://matt-rickard.com/rss, language:en-US

## Raft: The Distribute Systems Algorithm
 - [https://matt-rickard.com/raft-the-distribute-systems-algorithm](https://matt-rickard.com/raft-the-distribute-systems-algorithm)
 - RSS feed: https://matt-rickard.com/rss
 - date published: 2023-09-07T13:30:43+00:00

Consensus algorithms are at the core of distributed systems. How do you manage consistency across multiple servers or nodes?

The Raft Consensus Algorithm is a distributed system protocol that’s widely used (including by systems like Kubernetes, via etcd). It is equivalent in fault tolerance and consistency guarantees to Paxos, which is often seen as a more complex approach.

Here’s a simplification of the algorithm:

Overall design: Elect a leader among the servers, which is responsible for man

