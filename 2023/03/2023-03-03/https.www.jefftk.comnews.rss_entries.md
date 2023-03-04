# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Measuring Ads Opt-Out Compliance
 - [https://www.jefftk.com/p/measuring-ads-opt-out-compliance](https://www.jefftk.com/p/measuring-ads-opt-out-compliance)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-03-03 08:00:00+00:00

<p><span>

There's an interesting preprint out by Liu, Iqbal, and Saxena, </span>

<a href="https://arxiv.org/abs/2202.00885">Opted Out, Yet Tracked: Are
Regulations Enough to Protect Your Privacy?</a>.  They describe an
experiment they ran to figure out whether your choices on consent
dialog boxes actually do anything.  The idea is that if they work you
expect to see consistently lower bids in the "opt out" than "opt in"
case.  While I think the experiment wasn't quite right, with a few
tweaks it would be really informative.



<p>

The basic design makes sense:

</p>

<p>

</p>

<ol>

<li><p>Limit to publishers who run client-side auctions ("header
bidding") so you can see the bids.

</p></li>
<li><p>Visit some sites on a range of topics so advertisers can start
estimating your interests and decide to market to you.  (And also a
control group that skips this step.)

</p></li>
<li><p>Visit a publisher and see how much advertisers bid if you
opt in vs opt out.

</p></li>
</ol>



<p>

The main issue I see is that their implementation of (2) was probably
not good enough to get advertisers excited about bidding specifically
for their views:

</p>

<p>

</p>

<blockquote> <i>3.3.1 Simulating Interest Personas.</i> Since
advertisers bidding behavior is different for different user
interests, we simulate 16 user interest personas to capture a wide
spectrum of bidding behavior.  User personas are based on 16 Alexa
top websites by categories lists. To simulate each persona, we
initialize a fresh browser profile in an OpenWPM instance, on a fresh
EC2 node with a unique IP, iteratively visit top-50 websites in each
category, and update browser profile after each visit. Our rationale
in simulating personas is to convince advertisers and trackers of each
persona's interests, so that the advertisers bid higher when they
target personalized ads to each persona. In addition to the
above-mentioned 16 personas, we also include a control persona, i.e.,
an empty browser profile. Control persona acts as a baseline and
allows us to measure differences in bidding behavior.
</blockquote>



<p>

The sixteen personas they used were "Adult, Art, Business, Computers,
Games, Health, Home, Kids, News, Recreation, Reference, Regional,
Science, Shopping, Society, and Sports".

</p>

<p>

These are pretty bland, and I wouldn't expect advertisers knowing
you'd visited some sites in those categories to change their behavior
much.  This study would have been much better if they'd used some
sites with very strong commercial intent and high profit margins, like
mattresses, car sales, or credit cards.  Here's a test you can run at
home:

</p>

<p>

</p>

<ul>

<li><p>Open a new private browsing window and make sure third party
cookies are enabled.

</p></li>
<li><p>Search for either "sports" or "mattresses" and open the top
three results.

</p></li>
<li><p>Open <tt>cnn.com</tt> or another site with pretty normal ads
and see what you get.

</p></li>
</ul>



<p>

When I do this with "sports" I get ads that don't seem to have anything
to do with sports.  When I do it with "mattresses" I get a ton of big
(high bid!) ads for mattresses:

</p>

<p>

<a href="https://www.jefftk.com/example-mattress-ads-on-cnn-big.png"><img class="mobile-fullwidth" height="359" src="https://www.jefftk.com/example-mattress-ads-on-cnn.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

So I'd be very interested to see a repeat of this study where instead
of using generic Alexa top-16 categories they used specific high-value
categories, and with a screenshot step to check whether ads were
likely informed by those categories.

</p>

<p>

I'd also like to see a different control persona, where instead of
using an empty browser profile they visited several sites with minimal
commercial implications.  The problem is I'm worried that their
control is getting lower bids because it looks so obviously like a
bot, not because it has no personalization history.

</p>

<p>

(Disclosure: I used to work on ads at Google; speaking only for
myself.  I don't work in the ad industry anymore and have no plans to
return.)

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid02LXBTdMJuBpStRL5GvQRUCiKU9dDNALdTB7opuEw18Jc3y9x1J93N6dE4FSoV4zXVl">facebook</a>, <a href="https://mastodon.mit.edu/@jefftk/109960178688370697">mastodon</a></i></p>

