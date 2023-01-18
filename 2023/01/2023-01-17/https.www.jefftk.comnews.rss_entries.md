# Source Jeff Kaufmann, Source URL:https://www.jefftk.com/news.rss, Source language: en-US

## Ad Fraud Detection Prediction Market
 - [https://www.jefftk.com/p/ad-fraud-detection-prediction-market](https://www.jefftk.com/p/ad-fraud-detection-prediction-market)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-01-17 08:00:00+00:00
 - user: None

<p><span>

In my post on </span>

<a href="https://www.jefftk.com/p/can-ads-be-gdpr-compliant">the GDPR status
of ads</a> I wrote that I expected that European data protection
agencies would more likely than not rule that collecting personal
information for ad fraud detection requires consent:



<p>

</p>

<blockquote>
Is it within the legitimate interests of sites to collect user data
for ad fraud detection?  The ad industry has historically thought that
it was. For example, the <a href="https://iabeurope.eu/tcf-2-0/">IAB's
TCFv2</a>, the standard protocol consent popups use to talk to ad
networks, categorizes ad fraud detection <a href="https://iabeurope.eu/iab-europe-transparency-consent-framework-policies/">under
"Special Purpose 1"</a>, with users having "No right-to-object to
processing under legitimate interests". On the other hand, based on
points 52 and 53 of the <a href="https://www.legifrance.gouv.fr/cnil/id/CNILTEXT000046768989">recent
Microsoft ruling</a> I would predict that French regulators would rule
that since users do not visit sites to see ads, sites cannot claim
that they have a legitimate interest in using personal data to attempt
to determine whether their ads are being viewed by real people.

<p>

This is not settled; among other things the Microsoft ruling was
primarily considering ePrivacy which is stricter on some points. But I
think it's more likely than not that when we get clarity from the
regulators it will turn out that the kind of detailed tracking of user
behavior necessary for effective detection of ad fraud is not
considered to be within a publisher's legitimate interests.
</p>
</blockquote>



<p>

There was some informed pushback on this, <a href="https://mastodon.mit.edu/@hugo@mastodon.xyz/109652754082599760">from
Hugo
Roy and Michael Kleber</a>: a <a href="https://hroy.eu/">privacy
lawyer</a> and a <a href="https://mastodon.mit.edu/@Log3overLog2@mathstodon.xyz">privacy
engineer</a>.  This has definitely pushed me in the direction of
thinking I've misunderstood the situation and it's more likely that
the conventional ad industry interpretation is correct.  Which would
be a good thing in my book: as I said at the end of my post I do think
ad fraud detection should be permitted without user opt-in.

</p>

<p>

But I did want to write more about why I had, and to some extent still
hold, the view I did.  As Hugo referenced, fraud detection is
specifically called out in the GDPR as a legitimate interest:

</p>

<p>

</p>

<blockquote>
The processing of personal data strictly necessary for the purposes of
preventing fraud also constitutes a legitimate interest of the data
controller concerned.
<br />
&#8212;<a href="https://www.privacy-regulation.eu/en/recital-47-GDPR.htm">Recital 47</a>
</blockquote>



<p>

The main way I could see a decision preventing the continued operation
of economically effective ad fraud detection is that a court might
rule that the status quo involves collecting too much. Ad fraud
detection looks something like collecting every signal you can and
then looking for patterns that distinguish people from bots.  How do
you know if a signal will be useful?  Start logging it and feed it
into the analysis.  A company might have trouble convincing a court
that they really need all this data, especially when there's
collection they can't justify in terms of current utility.  But if
this gets limited to where you can only collect what you can show is
immediately useful, and don't have a way to learn from real traffic
what new signals you might want to be logging, then more and more bots
will get around detection.

</p>

<p>

A secondary way I could see a decision like this happening is if a
data protection agency decided that, while a publisher has a
legitimate interest in preventing itself from being defrauded by the
user, it doesn't have a legitimate interest in (delegating) collecting
data to demonstrate that it is not defrauding its advertisers.  Yes,
there is a sense in which the data collection is for the purpose of
preventing fraud, but it's essentially the publisher preventing
themself from committing fraud. A court could draw a distinction
between intrusion into an individual user's privacy for the purpose of
determining whether that individual user is defrauding the publisher,
but not for the purpose of determining whether there's fraud happening
between the publisher and the advertiser, which the user has nothing
to do with.

</p>

<p>

This is speculation: can we use a prediction market to get a better
estimate?  The one I made earlier on the <a href="https://manifold.markets/JeffKaufman/will-the-github-copilot-litigation">GitHub
Co-pilot litigation</a> seems to be going well so far, so here's <a href="https://manifold.markets/JeffKaufman/does-the-gdpr-ban-ad-fraud-detectio">another
market</a>:

</p>

<p>



</p>

<p>

Before the comments from Roy and Kleber I would have put this at ~65%;
now I'm at ~45%.  But if you think I'm wrong, take my (play) money!

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid02w9RNnFAv5XS1KKobdSJBpAuA46wDv9VHFwsWCyEcBFLHJrVCAncGESDgukNvkUwal">facebook</a>, <a href="https://lesswrong.com/posts/mvFBxbhfXcdkXRNAP">lesswrong</a>, <a href="https://mastodon.mit.edu/@jefftk/109705887759211573">mastodon</a></i></p>
