# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Prevalence to Relative Abundance
 - [https://www.jefftk.com/p/prevalence-to-relative-abundance](https://www.jefftk.com/p/prevalence-to-relative-abundance)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-04-25 08:00:00+00:00

<p><span>

Back in September </span>

<a href="https://www.jefftk.com/p/case-rates-to-sequencing-reads">I
wrote</a>:



<p>

</p>

<blockquote>
In thinking about how you might <a href="https://www.naobservatory.org/">identify future pandemics by
sequencing wastewater</a>, you might have a goal of raising an alert
before some fraction of people were currently infected.  What you're
actually able to observe, however, are <a href="https://www.jefftk.com/p/sequencing-intro">sequencing reads</a>, several steps removed
from infection rates.  Can we use covid data to estimate how the
fraction of people currently infected with some pathogen might
translate into the fraction of wastewater sequencing reads that match
the pathogen?
</blockquote>



<p>

In that post I looked at a single pathogen (SARS-CoV-2) in a single
metagenomic sequencing dataset (<a href="https://journals.asm.org/doi/full/10.1128/AEM.01448-21">Rothman
et al 2021</a>) and got a very rough point estimate (2.3e-8 relative
abundance at 0.1% prevalence).  What fraction of sequencing reads
might come from a novel pathogen at some level of prevalence continues
to be a key question, however, and this quarter I'm working with
several other people at the <a href="https://www.naobservatory.org/">NAO</a> in trying to get a
better understanding here.

</p>

<p>

Specifically, we'd like to understand how relative abundance (fraction
of sequencing reads matching an organism) varies with of prevalence
(what fraction of people are currently infected) and organism (ex:
since we're sampling wastewater you'd expect disproportionately more
gastrointestinal than blood pathogens).

</p>

<p>

Here's the current plan:

</p>

<ol>

<li><p>Gather wastewater metagenomic sequencing data, mostly by
looking at papers that published it in the <a href="https://www.ncbi.nlm.nih.gov/sra">Sequencing Read Archive</a>.
I'd love it if we could also include our own data here, but we aren't
far enough along to have much yet.

</p></li>
<li><p>Process the sequencing data (<a href="https://github.com/naobservatory/mgs-pipeline">code</a>) to
clean it (remove adapters, trim low-quality bases, collapse paired-end
reads) and identify the reads (assign them to taxonomic nodes).

</p></li>
<li><p>Gather corresponding estimates for the prevalence of various
human viruses in the populations contributing to the metagenomic
data. (<a href="https://github.com/naobservatory/p2ra">code</a>)

</p></li>
<li><p>Build and fit a model for relative abundance as a function of
prevalence, sequencing method, and the type of organism.

</p></li>
</ol>



<p>

Overall, this would be a big step forwards towards estimating the
feasibility of this kind of detection: cost should be inversely
proportional to relative abundance.

</p>

<p>

We're reasonably far along on (1) and (2), and if you're curious you
can <a href="https://www.jefftk.com/mgs-counts/">poke around</a>.
That shows the counts for human-infecting viruses across samples.
It's rough (ex: <a href="https://github.com/naobservatory/mgs-pipeline/issues/3">we're
not</a> doing any correction for PCR duplication yet) so don't
take it too seriously and <a href="https://github.com/naobservatory/mgs-pipeline/issues/new">let us
know</a> if you see something suspicious.  On (3) and (4) things are
much earlier: we currently have prevalence estimates for <a href="https://github.com/naobservatory/p2ra/tree/main/pathogens">five
viruses</a> and I'd like to get at least ten times this many.

</p>

<p>

(If you're curious why I haven't been talking more about writing a
book since my <a href="https://www.jefftk.com/p/write-a-book">post</a> a month ago, this is
a lot of it.  Right around when I posted that I moved from mostly
doing individual work to leading this project, and the opportunity
cost of taking time away became much higher.  I do still want to write
something summarizing the advice I got from people around making a
book, though, and it's possible I'll come back to the book project.)

</p>

<p>
<br />

<i>This post describes in-progress work at the <a href="https://www.naobservatory.org/">NAO</a> and covers work from a
team including <a href="https://www.simongrimm.com/">Simon Grimm</a>
and Asher Parker-Sartori estimating prevalences, <a href="https://dp-rice.github.io/">Dan Rice</a> modeling,
Will Bradshaw evaluating sequencing methods, and <a href="https://mikemc.cc/">Mike McLaren</a> identifying relevant
papers and providing general technical guidance.</i>

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0eAHxY6d22qrzxRaZo65GmyZyUYsT7jZEDShzXLZVHoNmFdt3nX5m5qmk64iLP9tHl">facebook</a>, <a href="https://lesswrong.com/posts/TJ5KsfmE8q7FLd85v">lesswrong</a>, <a href="https://forum.effectivealtruism.org/posts/QhZPrN2kkFv4S3YSg">the EA Forum</a>, <a href="https://mastodon.mit.edu/@jefftk/110261139518910726">mastodon</a></i></p>

