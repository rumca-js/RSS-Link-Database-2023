# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Lessons From TryContra
 - [https://www.jefftk.com/p/lessons-from-trycontra](https://www.jefftk.com/p/lessons-from-trycontra)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-02-15 08:00:00+00:00

<p><span>

As I </span>

<a href="https://www.jefftk.com/p/help-update-trycontra">wrote yesterday</a>, I
recently brought my little 

<a href="https://www.trycontra.com/">contra
dance search tool</a> up to date.  I realized I've been running it for
ten years now, which seems like a good time to look back over the
experience for lessons.



<p>

When I built it <a href="https://www.jefftk.com/p/where-can-i-dance">in 2013</a> I wrote:

</p>

<p>

</p>

<blockquote>
Experienced dancers know how to use <a href="http://www.contradancelinks.com/">ContraDanceLinks.com</a>, <a href="http://www.thedancegypsy.com/">Dance Gypsy</a>, and the <a href="http://dancedb.com/DanceDB/">DanceDB</a> to find places they can
go contra dancing, but those sites are too complex and confusing for
me to want to give to a new dancer.
</blockquote>



<p>

Here's what those dance-community focused sites looked like:

</p>

<p>

<a href="https://www.jefftk.com/contradancelinks-screenshot-2013-big.png"><img class="mobile-fullwidth" height="443" src="https://www.jefftk.com/contradancelinks-screenshot-2013.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

<a href="https://www.jefftk.com/dancedb-screenshot-2013-big.png"><img class="mobile-fullwidth" height="443" src="https://www.jefftk.com/dancedb-screenshot-2013.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

<a href="https://www.jefftk.com/dancegypsy-screenshot-2013-big.png"><img class="mobile-fullwidth" height="443" src="https://www.jefftk.com/dancegypsy-screenshot-2013.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

And here's what I built:

</p>

<p>

<a href="https://www.jefftk.com/trycontra-screenshot-2013-big.png"><img class="mobile-fullwidth" height="443" src="https://www.jefftk.com/trycontra-screenshot-2013.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Almost the same as it is today:

</p>

<p>

<a href="https://www.jefftk.com/trycontra-screenshot-2023-big.png"><img class="mobile-fullwidth" height="443" src="https://www.jefftk.com/trycontra-screenshot-2023.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

I wanted to build something easy to use and was willing to give up
pretty much everything else, and I think I succeeded at that.  You put
in your location, get a list of nearby dances, and click through to
their sites for more information.

</p>

<p>

There were several other choices I made, primarily out of laziness:

</p>

<p>

</p>

<ul>

<li><p>The site is completely static: HTML, CSS, JS.  The searching
happens in your browser, since it only takes a few kB to store all the
contra dances in the country.

</p></li>
<li><p>No dependencies: vanilla JS using browser APIs only.  Not even
minified.

</p></li>
<li><p>It's just a directory.  I don't host pages for dances.

</p></li>
<li><p>No accounts.  If you want to update the listing for your dance
you can email me.

</p></li>
<li><p>Minimal information.  Just a link, city, weekday, approximate
frequency, and whether it's gender-free.  No "1st and 3rd Sundays",
pricing, addresses, hours, performers, etc.  More details would mean
more information to collect, but more importantly it would mean more
information to go stale.

</p></li>
</ul>



<p>

In retrospect I feel like these decisions turned out well: the site
requires <a href="https://www.jefftk.com/p/designing-low-upkeep-software">very little
upkeep</a>.  I can leave it alone for years and it will keep chugging
along, and every so often I get an email with a correction and make a
small change to a <a href="https://www.trycontra.com/dances.json">text
file</a>.

</p>

<p>

(This has also given me a lot of experience at reading contra dance
websites.  I <a href="https://www.jefftk.com/p/dance-website-checklist">wrote advice for
people making these sites</a> in 2013, which I think is mostly still
good, but at this point I'd also add specifying covid details and
whether your dance is gender free.)

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0URdwQLwAvFKEsBwBCDgnz8J6GJjmDoYWuTLojUpkcBD4yut15jGDtYTNx2phPwi6l">facebook</a>, <a href="https://lesswrong.com/posts/ijS2zSuqh2N5KwGje">lesswrong</a>, <a href="https://mastodon.mit.edu/@jefftk/109869399599247144">mastodon</a></i></p>

