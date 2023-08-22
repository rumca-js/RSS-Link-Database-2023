# Source:Matt Rickard, URL:https://matt-rickard.com/rss, language:en-US

## Git Merge Strategies and Algorithms
 - [https://matt-rickard.com/git-merge-strategies-and-algorithms](https://matt-rickard.com/git-merge-strategies-and-algorithms)
 - RSS feed: https://matt-rickard.com/rss
 - date published: 2023-07-29T13:30:58+00:00

How does git merge one or more branches? A look at the different merge strategies and algorithms.

Recursive. If more than one common ancestor can be used for a three-way merge, it creates a merged tree of the common ancestors and uses that tree as a reference for the three-way merge. If there are conflicts, it can use heuristics to try and automatically resolve them (e.g., picking the file that’s been modified most recently).

ort (“Ostensibly Recursive’s Twin”). The new default merge strategy

