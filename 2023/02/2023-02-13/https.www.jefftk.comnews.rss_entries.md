# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Does the AGPL Work?
 - [https://www.jefftk.com/p/does-the-agpl-work](https://www.jefftk.com/p/does-the-agpl-work)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-02-13 08:00:00+00:00

<p><span>

It might be important to you that users of software you write are able
to modify it, in which case you might release it with a </span>

<a href="https://en.wikipedia.org/wiki/Copyleft">copyleft</a> license
like the 

<a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GPL</a>.  For
example, imagine someone's making a device that will run Linux.  They
need to tweak Linux so it will work on this particular device, and
they do that and sell you a copy.  Because Linux is under the GPL,
however, they also need to publish the source code for their tweaks.



<p>

<a href="https://www.jefftk.com/anti-agpl-proxy-1-big.png"><img class="mobile-fullwidth" height="149" src="https://www.jefftk.com/anti-agpl-proxy-1.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>


Then along comes the web, and people no longer send out copies of their
programs.  Instead, the programs live on their server, and you talk to
them with your browser:

</p>

<p>

<a href="https://www.jefftk.com/anti-agpl-proxy-2-big.png"><img class="mobile-fullwidth" height="160" src="https://www.jefftk.com/anti-agpl-proxy-2.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

This means that even if a program is under the GPL, the people
interacting with it have no right to the source code.  This was called
the "application service provider loophole", and the <a href="https://www.gnu.org/licenses/agpl-3.0.en.html">AGPL</a> was
created to fix it.  <a href="https://en.wikipedia.org/wiki/Mastodon_(social_network)">Mastodon</a>
is an example of AGPL software, and if you visit an instance you'll
see a little "view source code" link.  This isn't just something your
instance is doing to be nice&#8212;it's required by the AGPL.

</p>

<p>

Or is it?  A few months ago I read an <a href="https://news.ycombinator.com/item?id=30495647">interesting
argument</a> that you can easily bypass the AGPL: stick a "proxy"
between the AGPL code and the user, which removes the source code
offer:

</p>

<p>

<a href="https://www.jefftk.com/anti-agpl-proxy-3-big.png"><img class="mobile-fullwidth" height="295" src="https://www.jefftk.com/anti-agpl-proxy-3.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

How is this compliant with the license?  The AGPL tells you that when
you modify the program you must preserve its "offer the source to
anyone who asks" behavior:

</p>

<p>

</p>

<blockquote>
if you modify the Program, your modified version must prominently
offer all users interacting with it remotely through a computer
network (if your version supports such interaction) an opportunity to
receive the Corresponding Source of your version by providing access
to the Corresponding Source from a network server at no charge,
through some standard or customary means of facilitating copying of
software.
</blockquote>



<p>

The modified software still offers everyone the option to download the
source, but then a different piece of software that isn't covered by
the license runs a <code>sub_filter 'source_url' ''</code> and the
user doesn't actually receive the offer.

</p>

<p>

Courts do care about intent and this is, of course, not what the AGPL
authors intended, but it's not clear to me that what they intended is
coherent?  They mechanism they chose, a license that controls what
you're allowed to do when making changes to the AGPL-covered software,
doesn't seem like it would be able to prevent someone from making
user-hostile changes to other systems between this software and the
user.

</p>

<p>

(Not a lawyer, just an engineer interested in this sort of thing. Over
time I've <a href="https://www.jefftk.com/p/moving-away-from-the-gpl">moved to non-copyleft
licenses</a>, including for server-side software.)

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid02K8nvsTFhPo2eMEvisRQMUo23ah2TG9EJdxugiaZfdJX4Ct25ZAVuYFeFtaZZd995l">facebook</a>, <a href="https://mastodon.mit.edu/@jefftk/109857845325510802">mastodon</a></i></p>

