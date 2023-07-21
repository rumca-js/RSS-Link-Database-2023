# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Growth of Publicly Available Genetic Sequencing Data
 - [https://www.jefftk.com/p/growth-of-publicly-available-genetic-sequencing-data](https://www.jefftk.com/p/growth-of-publicly-available-genetic-sequencing-data)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-07-20T08:00:00+00:00

<p><span>

The largest source of publicly available genetic sequencing data is
the </span>

<a href="https://en.wikipedia.org/wiki/Sequence_Read_Archive">Sequence
Read Archive</a> (SRA), a joint project of the US (

<a href="https://en.wikipedia.org/wiki/National_Center_for_Biotechnology_Information">NCBI</a>),
Europe (

<a href="https://en.wikipedia.org/wiki/European_Bioinformatics_Institute">EBI</a>),
and Japan (

<a href="https://en.wikipedia.org/wiki/DNA_Data_Bank_of_Japan">DDBJ</a>).
Most relevant funding agencies and journals require sequencing
data to be deposited in the SRA.  I was curious how quickly it has
been growing, so I ran some queries.



<p>

The metadata for the SRA is available <a href="https://www.ncbi.nlm.nih.gov/sra/docs/sra-cloud-based-examples/">in
the cloud</a> and we can access it through <a href="https://cloud.google.com/bigquery">BigQuery</a>.  I ran:

</p>

<p>

</p>

<pre>
  SELECT EXTRACT(YEAR from releasedate),
         EXTRACT(MONTH from releasedate),
         SUM(mbases),
         SUM(mbytes)
    FROM `nih-sra-datastore.sra.metadata`
GROUP BY EXTRACT(YEAR from releasedate),
         EXTRACT(MONTH from releasedate)
</pre>



<p>

This gave me how much new data there was each month, in terms of both
genetic bases and (compressed) bytes on disk.

</p>

<p>

<a href="https://www.jefftk.com/sra-data-by-month-big.png"><img class="mobile-fullwidth" height="306" src="https://www.jefftk.com/sra-data-by-month.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Note the logarithmic y-axis.

</p>

<p>

This is reminiscent of another chart, the cost to sequence 1M bases:

</p>

<p>

<a href="https://www.jefftk.com/sequencing-cost-over-time-may-2022-big.png"><img class="mobile-fullwidth" height="305" src="https://www.jefftk.com/sequencing-cost-over-time-may-2022.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

(This is a pretty amazing chart, with the huge drop around 2008 coming
from <a href="https://en.wikipedia.org/wiki/Massive_parallel_sequencing">NGS
Sequencing</a>)

</p>

<p>

We could combine these, to get a rough estimate for how much
money is being spent to sequence the data going into the SRA, but to
do this we need to know how long a delay there is between sequencing
and releasing: if it cost $400/Mb in 2007-10, $100/Mb in 2008-01, and
$15/MB in 2008-04, then which cost should we use for interpreting data
released in 2008-06?  Here's a plot showing models 0-, 6-, 12-, and
24-month delays:

</p>

<p>

<a href="https://www.jefftk.com/cost-of-sra-data-by-month-big.png"><img class="mobile-fullwidth" height="339" src="https://www.jefftk.com/cost-of-sra-data-by-month.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

It looks like maybe ~9m is the initial delay, and with costs changing
more slowly in recent years it doesn't matter much for more recent
data.

</p>

<p>

Looking just at the last five years, after it has leveled out some, it
looks like a steady ~1.2e16 bases annually:


<a href="https://www.jefftk.com/sra-data-new-by-month-linear-big.png"><img class="mobile-fullwidth" height="336" src="https://www.jefftk.com/sra-data-new-by-month-linear.png" width="550" /><div class="image-vertical-spacer"></div></a>

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0BVvekfDaMQrmXfvHJPMBa1Pq1xG63f9WCAbNzS6dwc1twGBQLRgtNU2L31Mf5ngBl">facebook</a>, <a href="https://mastodon.mit.edu/@jefftk/110748131015350735">mastodon</a></i></p>

