# Rss links database for year 2023

Captured using Django application: [https://github.com/rumca-js/Django-rss-feed](https://github.com/rumca-js/Django-rss-feed).

 - I have defined multiple RSS sources, from which I gather URL data.
 - every hour I ping RSS sources, if it contains new data
 - every day I commit data from yesterday and push that to this repository

# Data

 - RSS links are captured for each source separately
 - two files formats for each day and source: JSON and markdown
 - markdown file is generated as a form of preview, JSON can be reused, imported
 - a link can be made 'persistent' and such links are stored 'forever'

# Goal

 - Archive purposes
 - Google sucks at providing results for various topics (dead internet)
 - Data analysis

# Inspirations

 - I Tracked Everything I Read on the Internet for a Year [https://www.tdpain.net/blog/a-year-of-reading](https://www.tdpain.net/blog/a-year-of-reading).
 - Automating a Reading List [https://zanshin.net/2022/09/11/automating-a-reading-list/](https://zanshin.net/2022/09/11/automating-a-reading-list/)
 - Google Search Is Dying [https://dkb.io/post/google-search-is-dying](https://dkb.io/post/google-search-is-dying)
 - Luke Smith: Remember to Consoom Next Content on YouTube [https://www.youtube.com/watch?v=nI3GVw2JSEI](https://www.youtube.com/watch?v=nI3GVw2JSEI). As a society we provide news instead of building a data base of important information
 - Bright Insight: YES, They Really Are Deleting the Internet And it’s WAY Worse Than You Think [https://www.youtube.com/watch?v=8O_NvPpbsbw](https://www.youtube.com/watch?v=8O_NvPpbsbw). Data are removed from 'visibility' in Google and other platforms.

## Video in Polish

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/QHBcLrlgaxY/0.jpg)](https://www.youtube.com/watch?v=QHBcLrlgaxY)

# Data analysis

With these data we can perform further analysis:

 - how many of old links are not any longer valid (link rot test)
 - capture all domains from RSS links (internal, and leading outside?). Analyse which domains are most common
 - which site generates most entries
 - we can capture all external links from entries, to capture where these sites lead to (check network effect, etc)
 - we can verify who reported first on certain topics

# Problems

 - Google fails to deliver content of small creators (blogs etc. private pages). Google focuses on corporate hosting. Most common links are towards YouTube, Google maps, Facebook, reddit
 - We cannot replace Google search
 - Google provides only 31 pages of news (in news filter) and around 10 pages for ordinary search. This is a very small number. It is like looking through keyhole at the Internet
 - Link rot is real. My links may be not working after some time
 - Is the data relevant, or useful for anyone?
 - Either we would like to record data from 'well established sources' or gather as many links as possible. I think web engines do it? We cannot gather too much data, as it can destroy our potato servers.
 - there are other RSS solutions like 'feedly', but it is an app, not data. You cannot parse it, you do not own the data, you can only do things that feedly allows you to do

# Ending notes

All links belong to us!

