# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Lightweight minimal speech recognition?
 - [https://www.jefftk.com/p/lightweight-minimal-speech-recognition](https://www.jefftk.com/p/lightweight-minimal-speech-recognition)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-07-12T08:00:00+00:00

<p><span>

I currently control my </span>

<a href="https://www.jefftk.com/news/jammer">rhythm stage setup</a>
with a USB keyboard. This works, except that my hands are often busy
playing instruments when I want to change something.  I already have a
microphone in front of my mouth running to a computer, which I use for
my whistle-controlled bass synthesizer: could I use speech
recognition?



<p>

Another way to look at this is that a lot of my exploration here has
been finding some way to play bass and mandolin at the same time:
<a href="https://www.jefftk.com/whistle-synth">whistle bass</a>, <a href="https://www.jefftk.com/p/chording-bass">bass pedals</a>, <a href="https://www.jefftk.com/p/simultaneous-footbass-and-footdrums">bass and drum
pedals</a>.  With speech recognition I could <a href="https://www.jefftk.com/p/calling-chords">call chords</a> to the computer!

</p>

<p>

I'm currently running on a <a href="https://www.raspberrypi.com/products/raspberry-pi-3-model-b/">Raspberry
Pi 3B</a>. I tried <a href="https://github.com/openai/whisper">OpenAI's Whisper</a> and then
<a href="https://github.com/ggerganov/whisper.cpp">the C++ port</a>
(which <a href="https://github.com/ggerganov/whisper.cpp/discussions/166">should
work on the 4B), and then the much older software </a><a href="https://github.com/julius-speech/julius">Julius</a> but my Pi 3B
couldn't handle real time with any of these. Is there some existing
software that would be a good fit for this?  People were running
speech recognition back when this computer would have been top of the
line.

</p>

<p>

I'm also considering giving up on the idea of using speech: all I
really need is some sound I can make consistently enough that the
computer can recognize.  I'm already running a system that can mostly
decode whistling, so maybe I should figure out how to phrase my
commands as simple whistle patterns?  I'm a bit nervous about doing
this while playing, though, since unless I choose patterns that can
sound musical in any key it's going to be pretty hard to combine with
playing something else.  Maybe alternating low and high notes, but I
can choose which notes in response to the key?

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid02XcB6U96Yk1EfT9aE2QSooQ2JwMRsgGfQgbhZq1HJd2rRxbDChxo8DUY4a8B8FE74l">facebook</a>, <a href="https://mastodon.mit.edu/@jefftk/110700988967477273">mastodon</a></i></p>

