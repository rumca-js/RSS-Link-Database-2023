# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## How Cardioid Are Cardioids?
 - [https://www.jefftk.com/p/how-cardioid-are-cardioids](https://www.jefftk.com/p/how-cardioid-are-cardioids)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-02-12 08:00:00+00:00

<p><span>

Dynamic cardioid microphones are one of the most common types of mic
for live sound.  The best known is probably the SM-57, but there are
many others.  They're called "cardioid" mics because their pickup
pattern is somewhat heart-shaped:

</span>

<p>

<a href="https://www.jefftk.com/cardioid-mic-pattern-big.png"><img class="mobile-fullwidth" height="550" src="https://www.jefftk.com/cardioid-mic-pattern.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

The idea is they pick up well in the direction you point them,
reasonably well off to the sides, but very little in the direction
they're pointed away from.  This is valuable in a live sound context
where you have 'monitor' speakers that point back at the performers:
if you put the mic right between the monitor and instrument, pointing
away from the monitor and towards the instrument, you should pick up
much more "instrument" than "monitor".

</p>

<p>

Why do we want that?  Because the more of the monitor you pick up both
the muddier it will sound and the quieter the instrument has to be in
the monitor before you get feedback.

</p>

<p>

According to the <a href="https://commons.wikimedia.org/wiki/File:Polar_pattern_cardioid.png">Wikipedia
diagram</a> above, this effect would be ~20dB if you got the mic angle
within 30deg of correct.  But how does real life compare, where
rejection might not be as good and some sound could be bouncing around
the room?

</p>

<p>

I took two common dynamic mics, a <a href="https://www.shure.com/en-US/products/microphones/sm57?variant=SM57-LC">Shure
SM-57</a> and a <a href="https://en-us.sennheiser.com/live-performance-microphone-vocal-stage-e-835">Sennheiser
e835</a> and connected them to a <a href="https://www.qsc.com/solutions-products/loudspeakers/portable/powered/portable-pa/k2-series/k102/">QSC
K10.2</a> powered speaker through a <a href="https://www.soundcraft.com/en/products/epm8">Soundcraft
EPM-8</a> mixer.  Each time the mic was on a stand, pointed directly
towards or away from the tweeter, with the capsule 55" from the
speaker's grille.

</p>

<p>

<a href="https://www.jefftk.com/off-axis-rejection-setup-big.jpg"><img class="mobile-fullwidth" height="295" src="https://www.jefftk.com/off-axis-rejection-setup.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

I set the mixer gain to 100% and slowly turned up the fader until I
could hear the beginning of feedback. I tracked the difference in
fader settings, and while this isn't perfect&#8212;the faders are not
precisely calibrated tools&#8212;it lets us get a sense of how much of
an effect we're talking about.

</p>

<p>

Here's an example with the e835. Pointed at the speaker:

</p>

<p>

<a href="https://www.jefftk.com/mixer-settings-pointing-at-speaker-big.jpg"><img class="mobile-fullwidth" height="472" src="https://www.jefftk.com/mixer-settings-pointing-at-speaker.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

And away from the speaker:

</p>

<p>

<a href="https://www.jefftk.com/mixer-settings-pointing-away-from-speaker-big.jpg"><img class="mobile-fullwidth" height="455" src="https://www.jefftk.com/mixer-settings-pointing-away-from-speaker.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Comparing the positions across a few trials it was consistently around
5dB better.  The SM-57 was also very similar, which makes sense since
my impression is the e835 was inspired by the SM-57/SM-58 family.

</p>

<p>

While 5dB isn't nothing, it's very different from the diagram
above. What's going on?

</p>

<p>

Our first problem is that we should be looking at the specs for these
specific mics instead of a random diagram from Wikipedia. If you look
at the <a href="https://assets.sennheiser.com/global-downloads/file/10874/SP_1209_v1.0_e_835_e_835-S_Product_Specification_EN.pdf">e835
specs</a> the rejection pattern is frequency-dependent:

</p>

<p>

<a href="https://www.jefftk.com/cardioid-polar-pattern-e835-big.png"><img class="mobile-fullwidth" height="393" src="https://www.jefftk.com/cardioid-polar-pattern-e835.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Same for the SM-57:

</p>

<p>

<a href="https://www.jefftk.com/sm57-typical-polar-patterns-big.png"><img class="mobile-fullwidth" height="399" src="https://www.jefftk.com/sm57-typical-polar-patterns.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Here's the frequency spread I was seeing for feedback with the SM-57
pointed directly away from the speaker:

</p>

<p>

<a href="https://www.jefftk.com/feedback-frequencies-big.jpg"><img class="mobile-fullwidth" height="254" src="https://www.jefftk.com/feedback-frequencies.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

This peak corresponds to around where the mics should have the worst
rejection, ~125Hz.  Looking at the charts, I think the SM57 should be
managing 10dB and the e835 3dB, which isn't exactly what I saw, so my
guess is the rest of the difference comes from sound bouncing around
the room or manufacturing differences.

</p>

<p>

Overall, it's still worth pointing mics away from speakers: even 5dB
is enough to make a worthwhile difference in how loud you can get a
quiet instrument in the monitor before running into feedback issues.

</p>

<p>

(If you wanted to go farther you could notch out the feedback-prone
frequencies from the monitor mix, but this is rarely worth doing in
the contra dance live sound contexts I'm usually in.  Monitors that
loud start to be a problem for getting good sound in the hall.)

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0EfXc8Jmo33PXct2NfheDNVYaS5W3hMZ9HmxvHWNL5KCNx3nXWtaTfhS6wqDRDfnDl">facebook</a>, <a href="https://mastodon.mit.edu/@jefftk/109852660191992722">mastodon</a></i></p>

