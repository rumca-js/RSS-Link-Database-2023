# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Abusing Snap Circuits IC
 - [https://www.jefftk.com/p/abusing-snap-circuits-ic](https://www.jefftk.com/p/abusing-snap-circuits-ic)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-03-05 08:00:00+00:00

<p><span>

The kids got a </span>

<a href="https://www.amazon.com/Snap-Circuits-SC-100-Electronics-Exploration/dp/B00008BFZH">Snap
Circuits Kit</a> a while ago, and enjoy it.  In terms of learning,
however, it's been a bit mixed.  The basic circuits (light, motor) are
good: they understand they need to connect the parts the right way
around and that they need a complete circuit.  On the other hand, most
of the projects in the kit rely on the three audio chips, and just doing
the projects isn't enough to really understand how they work.



<p>

They had a friend over yesterday, and after building one of the projects
together wandered off to do something else.  I decided to see if I
could experimentally determine how one of the chips worked, so that
maybe we could do something interesting together later.
There turned out to be a lot more combinations that did something
interesting than I expected, however, so instead this is just
cataloging them.  So: here are 13 more snap circuits projects you can
make that abuse the music IC to do things it wasn't intended to do.

</p>

<p>

Since none of this is what was intended, you may get different results
from these than I did.  I <i>think</i> you won't break anything,
because as a modern kids toy I'd expect this to be robust to hooking
it up 'wrong', but no guarantees.

</p>

<p>

First, though, here's the basic correct operation of the Music IC:

</p>

<p>

<a href="https://www.jefftk.com/music-ic-correct-big.jpg"><img class="mobile-fullwidth" height="302" src="https://www.jefftk.com/music-ic-correct.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

The pinout of the chip is:

</p>

<p>

</p>

<pre>
trigger +--+--+ hold
        |     |
      - +-----+ out
</pre>



<p>

The idea is you connect positive voltage to the <code>+</code> pin,
negative to the <code>-</code> pin, run the speaker between
<code>out</code> and <code>+</code> and you'll get "happy birthday".
It plays one time through the song when it first gets power, and
repeats if you connect <code>trigger</code> to power momentarily or
<code>hold</code> to power in a sustained way.

</p>

<p>

Despite my picture above being the simplest correct use of the chip,
it's not one of the projects.  Instead the first project with an audio
IC (#3) also includes the "whistle chip" sensor on the trigger pin to
allow you to make it start over.  Then they follow up (#4) by putting a
resistor in series with the speaker to make it quieter.

</p>

<p>

Here are some other arrangements that demonstrate other modes the chip
has:

</p>

<p>

</p>

<ol>

<li><p>Instead of connecting <code>+</code> directly to positive
voltage, put the resistor in the way.  It plays the same song at a
slightly lower pitch.

</p></li>
<li><p>Don't connect anything to <code>+</code>.  Instead, connect
positive voltage to <code>hold</code>.  It plays something kind of of like a
distorted version of the first line.

</p></li>
<li><p>Same as (2) but use the resistor instead of a jumper.  It
makes an annoying electronic alarm noise.

</p></li>
<li><p>Put the LED from positive to <code>hold</code> and the
momentary switch from positive to <code>+</code>.  Tapping the switch
gives a ray gun sort of chirp.

</p></li>
<li><p>Same as (3) but add the momentary switch from positive to
<code>+</code>.  Initially it plays the annoying alarm, but when you
tap the switch it plays a cross between the song and the alarm noise.

</p></li>
<li><p>Same as (1) but also add a jumper from positive voltage to
<code>hold</code> and the LED from <code>-</code> to negative
voltage.  It plays a quiet buzzer sound.

</p></li>
<li><p>Same as (6) but use the lamp instead of the LED.  It plays the
song in a stuttery uneven staccato way.

</p></li>
<li><p>Same as (2) but put the resistor from <code>-</code> to
negative voltage.  It sometimes plays a quiet chirping like a phone
that has been left off the hook, other times more like a robotic bird
call.

</p></li>
<li><p>Same as (8) but put the jumper from positive to <code>+</code>
instead of positive to <code>hold</code>.  It moves through a range
of annoying buzzing at different pitches.

</p></li>
<li><p>Same as (2) but with the resistor in series with the speaker.
It plays something very similar to (7).

</p></li>
<li><p>Same as (10) but without the jumper from positive to
<code>hold</code> and with the photoresistor from positive to
<code>+</code>.  Makes a range of annoying squeals.  ("Like an alien
invasion attacking our house")

</p></li>
<li><p>Make a circuit from the positive terminal through the speaker
through the <code>+</code> to <code>-</code> and then the negative
terminal.  It plays happy birthday very quietly.  Same thing if you
put the speaker on the negative side, or even in parallel with the
battery!

</p></li>
<li><p>Make a circuit from the positive terminal through the speaker
through <code>hold</code> to <code>out</code> to the negative
terminal. Plays something quiet and distorted that seems like it might
have been music once.

</p></li>
</ol>



<p>

For example, here is (11):

</p>

<p>



</p>

<p>

Most of these combinations, and the ones that make the most
interesting sounds, are essentially adding resistance in places where
it wasn't designed for.  The 100&#8486; resistor, LED, light, and
diode all provide different amounts of resistance.  This is clearest
with the photoresistor, where by shining a bright light on the sensor
and then dimming it you can move it through all of these modes.  I
think this would be even better with an adjustable resistor, but
while the manufacturer does <a href="https://shop.elenco.com/consumers/adjustable-resistor-500k-2.html">make
one</a> it's not included in the starter kit.

</p>

<p>

<a href="https://www.jefftk.com/snap-circuits-adjustable-resistor-big.jpg"><img class="mobile-fullwidth" height="262" src="https://www.jefftk.com/snap-circuits-adjustable-resistor.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

After writing the above, Anna (7y) and I went through most of
these combinations.  She especially liked using a flashlight to move
between states with the photoresistor.  We tried to build variable
resistors out of household objects, but didn't have much success: a
pencil cut in half was too low resistance, a thick line drawn with
pencil was too high, slightly salted water wasn't close to linear.

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0oaRYMeZ5icAp2Ed8P2WcCy4xZBLA1mm7Df5MxVgTfcMbdr28MGtSP3bcjT8LTMTEl">facebook</a>, <a href="https://lesswrong.com/posts/3dcfeXCBQvrMnMiGA">lesswrong</a>, <a href="https://mastodon.mit.edu/@jefftk/109971743066070916">mastodon</a></i></p>

