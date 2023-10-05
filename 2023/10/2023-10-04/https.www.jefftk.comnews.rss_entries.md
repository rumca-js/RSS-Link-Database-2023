# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## PortAudio M1 Latency
 - [https://www.jefftk.com/p/portaudio-m1-latency](https://www.jefftk.com/p/portaudio-m1-latency)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-10-04T08:00:00+00:00

<p><span>

I recently tried to get my </span>

<a href="https://www.jefftk.com/whistle-synth">whistle-controlled
bass synthesizer</a> working on my Mac, as a backup to my 

<a href="https://www.jefftk.com/p/whistle-synth-pi">Raspberry Pi version</a>. [1] It's written
on top of 

<a href="https://www.portaudio.com/">PortAudio</a>, a
cross-platform audio library, so getting it to compile and run was
mostly a matter of getting the library installed, which went quickly.
Unfortunately, the latency was far too high to be useful as a
real-time musical instrument.



<p>

Testing with PortAudio's demo <a href="https://portaudio.com/docs/v19-doxydocs/paex__read__write__wire_8c_source.html">paex_read_write_wire.c</a>
[2] with <code>suggestedLatency</code> changed from
<code>defaultHighOutputLatency</code> to
<code>defaultLowInputLatency</code> I see:

</p>

<p>

</p>

<pre>
Input device # 2.
    Name: MacBook Pro Microphone
      LL: 0.0528542 s
      HL: 0.0621875 s
Output device # 3.
   Name

