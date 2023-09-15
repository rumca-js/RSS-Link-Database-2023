# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Inline Plotting in iTerm2
 - [https://www.jefftk.com/p/inline-plotting-in-iterm2](https://www.jefftk.com/p/inline-plotting-in-iterm2)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-09-14T08:00:00+00:00

<p><span>

I spend most of my working time in the terminal: I run my text editor
there, run programs there, etc. I usually have my iTerm2 set up to
display </span>

<a href="https://www.jefftk.com/p/terminal-preferences">many narrow full height
terminals</a>.  When I'm working with plots, however, I normally do
something like:



<p>

</p>

<pre>
$ ./some-cmd.py plot.png &amp;&amp; open plot.png
</pre>



<p>

Which pops up a Preview window with my plot, and then I close it and
go back to my coding. What I'd really like, though, is for this to be
directly in my terminal. And this is possible!

</p>

<p>

The iTerm2 terminal supports an <a href="https://iterm2.com/documentation-images.html">inline images
protocol</a>, and <a href="https://github.com/daleroberts/itermplot">itermplot</a> provides
a matplotlib backend that speaks this protocol. Which means after
updating my <code>.bashrc</code> to have:

</p>

<p>

</p>

<pre>
export MPLBACKEND="module://itermplot"
export ITERMPLOT="rv"


