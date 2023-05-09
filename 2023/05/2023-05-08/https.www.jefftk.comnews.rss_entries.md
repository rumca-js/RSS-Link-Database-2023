# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Dance Profit Sharing
 - [https://www.jefftk.com/p/dance-profit-sharing](https://www.jefftk.com/p/dance-profit-sharing)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-05-08 08:00:00+00:00

<p><span>

With most endeavors that have a financial component there's a spectrum
of approaches that differ on how they assign risk.  At the "low risk"
end you have agreements to pay a specific amount ("we pay
$100/person"), while at the "high risk" end it depends on how things
go go ("everyone gets a share of the take").  Contra dance events
generally go towards the low risk end: most of the time I'm playing
for a fixed fee.

</span>

<p>

I've been thinking about this, though, because the dance I help run
does profit sharing.  The idea is, we <a href="https://www.bidadance.org/payscale">guarantee</a> $125/performer
and then if there's profit left over after fixed expenses half of it
goes to the performers.  I wasn't around for the initial
implementation, but I think there were probably two reasons:

</p>

<p>

</p>

<ol>
<li><p>When a band or caller draws a big crowd that's something we'd like
   to encourage, and we're happy to share some of the rewards with
   them.

</p></li>
<li><p>How much money we have available to pay performers depends on
   attendance.  Profit sharing means that we pay performers more, to
   the extent that it doesn't risk our financial health.
</p></li>
</ol>



<p>

You don't want to go too far in the direction of sharing risk, though,
because the event has most of the responsibility for attendance and is
also in a better position than many of the performers to take the loss
from a low-turnout dance.

</p>

<p>

While I like this system overall, a major downside is that it requires
you to determine how profitable this event was before paying the
performers.  I mean, it's possible to just pay everyone the guarantees
and sort it out later, but that means following up with people to send
additional payments, which might be relatively small.  So you're
filling out a <a href="https://www.bidadance.org/attendance-financials-template">pretty
complicated form</a> by hand at the dance after counting the money
when you'd rather be dancing.

</p>

<p>

Could we get similar effects without needing to compute profit in the
moment?  What if we use attendance instead?  Here's how payments would
look with a bonus of $1 for every attendee over 120:

</p>

<p>

<a href="https://www.jefftk.com/per-performer-extra-payments-big.png"><img class="mobile-fullwidth" height="337" src="https://www.jefftk.com/per-performer-extra-payments.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

The main places where these two systems differ is in their handling of
large and small bands.  With the current system a duo is much more
likely to get additional money than a quartet, because fixed expenses
are two performers lower.  While I do play in <a href="https://www.kingfisherband.com/">a duo</a> and would be tempted
to say otherwise, I don't see a general reason to pay smaller bands
more.

</p>

<p>

Another nice thing about this structure is that it's easy to tweak to
keep the dance financially healthy.  The threshold or per-person
amount could change in either direction, and it's much less of a big
deal than changing guarantees.

</p>

<p>

I don't know if our dance will switch to this, but if we do I'll plan
to post back in a year or so with how it's gone for us.

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid02wj7tn6ErxRzYci48JqXUpxXk2sRY8UaU5GzrRq1RPfczmy44yAzoqwTX8YV5GyhJl">facebook</a>, <a href="https://lesswrong.com/posts/QacKfd7Efd53AzwBM">lesswrong</a></i></p>

