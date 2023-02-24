# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Somerville Roads Getting More Dangerous?
 - [https://www.jefftk.com/p/somerville-roads-getting-more-dangerous](https://www.jefftk.com/p/somerville-roads-getting-more-dangerous)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-02-23 08:00:00+00:00

<p><span>

In a local discussion of whether our attempts to reduce traffic
fatalities were working someone posted:

</span>

<p>

</p>

<blockquote>
I've lived in Somerville for over 40 years and have visited even
longer. The roads are more dangerous than ever.
</blockquote>



<p>

With all the <a href="https://www.somervillema.gov/departments/programs/vision-zero-somerville">Vision
Zero</a> work, and earlier traffic safety progress, this would be
surprising and disappointing if it were the case.  Is it?

</p>

<p>

Somerville is an interesting city to look at because it was mostly
built out decades ago.  The last large change was bulldozing I-93
through in the late 1960s:

</p>

<p>

<a href="https://www.jefftk.com/buldozing-i93-1969-big.png"><img class="mobile-fullwidth" height="575" src="https://www.jefftk.com/buldozing-i93-1969.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

This makes fatality rates over time comparable in a way they wouldn't
be if you were looking at a city that had expanded, contracted, or
been seriously rebuilt.

</p>

<p>

I pulled accident date from the national <a href="https://www.nhtsa.gov/research-data/fatality-analysis-reporting-system-fars">Fatality
Analysis Reporting System</a> (FARS) which goes back to 1975.  Here's
what I see for the number of fatal crashes annually (<a href="https://github.com/jeffkaufman/fars/blob/main/somerville-process.py">code</a>):

</p>

<p>

<a href="https://www.jefftk.com/somerville-annual-fatal-crashes-big.png"><img class="mobile-fullwidth" height="332" src="https://www.jefftk.com/somerville-annual-fatal-crashes.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

<i>blue bars are annual counts; red line is a 10y centered moving average</i>

</p>

<p>

Over the last 40y it's gotten about 3x better, though 2019 was a
pretty bad year.

</p>

<p>

I'd also be interested in whether our roads are becoming more
dangerous for pedestrians specifically.  Is the decrease just due to
airbags, crash testing, and cars becoming safer for their occupants?
While pedestrian data in FARS only goes back to 1991, we can still
graph what we have:

</p>

<p>

<a href="https://www.jefftk.com/somerville-annual-pedestrian-crashes-big.png"><img class="mobile-fullwidth" height="335" src="https://www.jefftk.com/somerville-annual-pedestrian-crashes.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

It does look like we're making progress specifically within pedestrian
safety as well, though 2019 now sticks out even more.

</p>

<p>

(I'm being lazy here and charting "traffic accidents with a fatality
and involving at least one pedestrian".  The FARS data does make it
possible to see whether it was a pedestrian that died, but this
requires joining CSVs in a way that's a bit awkward.  In the ones I've
spot checked the fatality was a pedestrian, which is what you'd
expect.)

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0HNMqvdXZvuwrmX4pTRjc5Jp2HxdJzbvjcd9y1rpnSiWAaxJZ8hsZoPB5m6bKCkYKl">facebook</a>, <a href="https://mastodon.mit.edu/@jefftk/109915410632233894">mastodon</a></i></p>

