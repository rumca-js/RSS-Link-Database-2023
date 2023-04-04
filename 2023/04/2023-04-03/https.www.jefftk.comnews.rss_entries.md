# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## AWS Has Raised Prices Before
 - [https://www.jefftk.com/p/aws-has-raised-prices-before](https://www.jefftk.com/p/aws-has-raised-prices-before)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-04-03 08:00:00+00:00

<p><span>

There's some speculation around whether AWS will need to raise
their prices, as many tech companies announce inflation-driven
increases.  One consideration that people will sometimes give is that
AWS has never raised prices before, except that this isn't quite true.
The following is not actually important, but I want to write it up
anyway out of pedantry.

</span>

<p>

When AWS S3 launched in <a href="https://press.aboutamazon.com/2006/3/amazon-web-services-launches">March 2006</a> their initial pricing was:

</p>

<p>

</p>

<blockquote>
Storage
<br />
$0.15 per GB-Month of storage used
<p>
Data Transfer
<br />
$0.20 per GB - data uploaded
$0.20 per GB - data downloaded
</p>
</blockquote>



<p>

In <a href="https://web.archive.org/web/20070502160305/http://www.amazon.com/S3-AWS-home-page-Money/b?ie=UTF8&amp;node=16427261">June
2007</a> they switched to:

</p>

<p>

</p>

<blockquote>
Storage<br />
$0.15 per GB-Month of storage used
<p>
Data Transfer<br />
$0.10 per GB - all data uploaded<br />
$0.18 per GB - first 10 TB / month data downloaded<br />
$0.16 per GB - next 40 TB / month data downloaded<br />
$0.13 per GB - data downloaded / month over 50 TB
</p>
<p>
Data transferred between Amazon S3 and Amazon EC2 is free of charge
</p>
<p>
Requests<br />
$0.01 per 1,000 PUT or LIST requests<br />
$0.01 per 10,000 GET and all other requests*<br />
* No charge for delete requests
</p>
</blockquote>



<p>

They went from requests being free to a low per-request charge,
lowering the data transfer cost at the same time.  For very
request-heavy workloads this was a price increase on balance, and some
customers needed to make implementation changes to avoid sending so
many requests.

</p>

<p>

That this was, as far as I know, the only time they've raised prices in
15+ years is impressive, and speaks well of their commitment to
predictability.  But it just annoys me when people claim they've never
done it.

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid02jsx5bKfNsVeiuKJDD8BkKYSiSrTMsUdFLRDTJ8zkjMbtXeqezBrXgF5Jo74Nyp85l">facebook</a>, <a href="https://lesswrong.com/posts/ip7mCxL28gPLGJoDYtech">lesswrong</a>, <a href="https://mastodon.mit.edu/@jefftk/110135699224357614">mastodon</a></i></p>

