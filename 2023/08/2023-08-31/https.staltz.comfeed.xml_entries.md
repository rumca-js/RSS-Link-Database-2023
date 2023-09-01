# Source:André Staltz, URL:https://staltz.com/feed.xml, language:en-US

## JavaScript Getter-Setter Pyramid
 - [https://staltz.com/javascript-getter-setter-pyramid.html](https://staltz.com/javascript-getter-setter-pyramid.html)
 - RSS feed: https://staltz.com/feed.xml
 - date published: 2023-08-31T10:48:35.222667+00:00

The cornerstone of JavaScript is the function. It is a flexible abstraction that works as the basis for other abstractions, such as Promises, Iterables, Observables, and others. I have been teaching these concepts in conferences and workshops, and over time I have found an elegant summary of these abstractions, layed out in a pyramid. In this blog post I’ll provide a tour through these layers in the pyramid. FUNCTIONS X =&gt; Y &lt;?xml version=”1.0” encoding=”UTF-8” standalone=”no”?&gt; Function Value The very base of JavaScript are the first-class values such as numbers, strings, objects, booleans, etc. Although you could still write a program that uses just values and control flow, very soon you would need to write a function to improve your program. Functions are unavoidable abstractions in JavaScript, they are often required for async I/O via callbacks. The word “function” in JavaScript does not refer to “pure functions” like in functional programming. It’s better to understand 

## The year tech giants peaked – 2018, a retrospective
 - [https://staltz.com/the-year-tech-giants-peaked-2018-a-retrospective.html](https://staltz.com/the-year-tech-giants-peaked-2018-a-retrospective.html)
 - RSS feed: https://staltz.com/feed.xml
 - date published: 2023-08-31T10:48:35.221126+00:00

2018 marked history as the year when governments made tech giants responsible for election interference and tumult in democracy. Centralization and decentralization were central themes in cyberspace this year, while regulation and freedom also defined the rhetoric of many actors. We understood how closely cyberspace and meatspace affect each other, demonstrated by a couple of key events in 2018. FB and GOOG peaked (Source: Reuters) When the Cambridge Analytica data scandal was published on March 17th, FB stock took a big hit. In April, Zuckerberg appeared before U.S. Congress to testify, leaving answers that many felt were unsatisfactory. A few months later, as their Q2 earnings report demonstrated little to no growth, many investors immediately sold their stock, leading to 20% drop in price ($120 billion in value). Many seemed to realize that FB is not doing well, neither as a business, nor as a platform for humane discourse. As a result, FB stock prices this year went 2 years back 

## Rust for Mobile? Not yet
 - [https://staltz.com/rust-for-mobile-not-yet.html](https://staltz.com/rust-for-mobile-not-yet.html)
 - RSS feed: https://staltz.com/feed.xml
 - date published: 2023-08-31T10:48:35.217953+00:00

It’s been 1 year and 1 month since I announced ssb-neon on SSB as an effort to gradually migrate the SSB tech stack from JS to Rust. I learned a lot about the technical details of actually doing this in production (in Manyverse) and have some lessons to share. Summary Since Manyverse version 0.2110.5, all Rust libraries have been removed. This was a sad decision that I had to take, for various technical reasons that I’ll explain below. ssb-neon, renamed to ssb-rsjs (to decouple ourselves from the Neon library in specific), was also supposed to be a community effort. I thought people would spontaneously contribute a Rust variant of simple libraries like ssb-ref, ssb-serve-blobs, etc, because I trusted in the spontaneous and modular contribution model that powered the pull-stream community and the callbag community. To my surprise, apart from the two initial ones I built, no one else made an ssb-rsjs library. @Daan (if I remember correctly) tried to start one, and @glyph built one for 

## Some people want to run their own servers
 - [https://staltz.com/some-people-want-to-run-their-own-servers.html](https://staltz.com/some-people-want-to-run-their-own-servers.html)
 - RSS feed: https://staltz.com/feed.xml
 - date published: 2023-08-31T10:48:35.216364+00:00

This post is a reply to Moxie’s recent article “My first impressions on web3”. Although I am writing a criticism, I am grateful for Moxie’s post because it exposes several truths that underlie web3, which most people are not willing to see. There is a surprising amount of centralization actively brewing in the “decentralized” space and most of its advocates don’t seem concerned. I think money (especially loads of money) blinds people to the uncomfortable truths that Moxie made explicit. At the same time, Moxie referred to other uncomfortable truths but somehow didn’t address them directly. This is why I felt compelled to write. I liked the honesty of his post but I want an even more honest discussion. Some claims he wrote are factually wrong and sound like mere ideology. Let’s begin with the first one: People don’t want to run their own servers, and never will. This cannot be factually true, some people want to run their own servers. What is the thriving self-hosted open source commu

## The Myth of Mass Collaboration
 - [https://staltz.com/the-myth-of-mass-collaboration.html](https://staltz.com/the-myth-of-mass-collaboration.html)
 - RSS feed: https://staltz.com/feed.xml
 - date published: 2023-08-31T10:48:35.214848+00:00

There is a general belief that the internet has supercharged collective intelligence and allowed humans to collaborate at scale, producing knowledge and creating masterpieces. On the surface, it seems true. To name a few archetypal examples: Wikipedia, open source projects such as Linux, hacktivism, and crowdsourced science experiments such as Rosetta@home. However, those successes did not happen as coordination, planning, and execution at a global scale. There is little collaboration taking place. I used to believe there was mass collaboration on the internet. But I’ve realized that collaboration is extremely hard. It does not scale, especially not at internet scale. The examples we look up to are either not collaborative on the microscopic level, or are rare exceptions to the rule. Goals and teamwork To collaborate on something is to work together with others towards a common goal. How often do people have a common goal? RARELY. Put three co-founders together to build a company, an

## Parametric Progress
 - [https://staltz.com/parametric-progress.html](https://staltz.com/parametric-progress.html)
 - RSS feed: https://staltz.com/feed.xml
 - date published: 2023-08-31T10:48:35.211384+00:00

It’s been some 10 years since I started my career as a developer, and one of the most important habits I have learned is something I call “Parametric Progress”. I would have told younger me about this, if I could. When you’re working on changing a system (and codebases are systems), it is extremely tempting to change more aspects than you’re originally planned to. Say you wanted to just fix a bug. You found the culprit, but you also saw a badly named variable, a function that could be split into two, some code style changes to make, some libraries to be updated, and something else that seemed like a bug. So you fixed all of those things, and you committed it. This may seem efficient, because you are doing more work in one go, but it’s not. It’s actually the opposite. It is more efficient to fix only one thing per git commit. Choose one aspect, or one “parameter”, and change only that. Then, see what happens, learn about the effects of your change, and then move on to the next paramet

## Back to the Web
 - [https://staltz.com/back-to-the-web.html](https://staltz.com/back-to-the-web.html)
 - RSS feed: https://staltz.com/feed.xml
 - date published: 2023-08-31T10:48:35.209716+00:00

I used to blog a lot more. There are a lot of reasons for that, perhaps the biggest one is the standards I hold myself to. Ever since my articles started getting viral and being mentioned in the news, writing on my blog is not a light activity anymore. I want to change that. We are currently witnessing the most fragmented environment for social networks since the dawn of Twitter and Facebook. The two reasons are: Twitter is in decay, and decentralized alternatives are alive and thriving. This is good and bad. Good because, hey, we’re finally decentralizing this space! Bad because it’s unclear (at least that’s how I’ve been feeling) where to publish your content. I used to be very active on Twitter, but Twitter is ruined for me now. It’s not about mister Tesla, actually. It’s all the changes that they’re making to Twitter that makes it objectively worse than before. A quick list of complaints: “For You” tab is visually bugged on Android, long form tweets with “read more” button are a 

