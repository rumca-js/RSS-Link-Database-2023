# Source:Matt Rickard, URL:https://matt-rickard.com/rss, language:en-US

## Type Constraints for LLM Output
 - [https://matt-rickard.com/type-constraints-for-llm-output](https://matt-rickard.com/type-constraints-for-llm-output)
 - RSS feed: https://matt-rickard.com/rss
 - date published: 2023-09-05T13:30:02+00:00

If you want to coerce a typed JSON response out of an LLM, you have a few options:

Control the token distributions via state machines with a regex or context-free grammar. The benefit of this method is correctness. You are guaranteed to get a valid response on the first generation. It comes at the cost of compute (the token distributions are computed and modified on every generation) and development time (it’s hard to define a valid regex or context-free grammar for every request/response that

