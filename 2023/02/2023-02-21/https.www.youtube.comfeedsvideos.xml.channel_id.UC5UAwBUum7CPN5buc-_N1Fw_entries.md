# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## LINUX vs WINDOWS: complete performance test!
 - [https://www.youtube.com/watch?v=a5YQ8xvQPSc](https://www.youtube.com/watch?v=a5YQ8xvQPSc)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-02-21 16:36:15+00:00

Download Safing's Portmaster and take control of your network traffic: https://safing.io

Grab a brand new laptop or desktop running Linux: https://www.tuxedocomputers.com/en#

👏 SUPPORT THE CHANNEL:
Get access to a weekly podcast, vote on the next topics I cover, and get your name in the credits:

YouTube: https://www.youtube.com/@thelinuxexp/join
Patreon: https://www.patreon.com/thelinuxexperiment

Or, you can donate whatever you want: https://paypal.me/thelinuxexp

👕 GET TLE MERCH
Support the channel AND get cool new gear: https://the-linux-experiment.creator-spring.com/

🎙️ LINUX AND OPEN SOURCE NEWS PODCAST:
Listen to the latest Linux and open source news, with more in depth coverage, and ad-free!  https://podcast.thelinuxexp.com

🏆 FOLLOW ME ELSEWHERE:
Website: https://thelinuxexp.com
Mastodon: https://mastodon.social/web/@thelinuxEXP
Pixelfed: https://pixelfed.social/TLENick
Twitter : http://twitter.com/thelinuxEXP
PeerTube: https://tilvids.com/c/thelinuxexperiment_channel/videos

This video is distributed under the Creative Commons Share Alike license.

#linux #windows #benchmark 

00:00 Intro
00:42 Sponsor: monitor and secure your internet connection
01:46 The benchmark setup
03:04 Resource Usage
06:52 Internet Speeds
08:32 CPU Benchmark
09:17 GPU + Gaming Benchmarks
13:35 Battery Life
14:34 Conclusions?
16:25 Sponsor: Get a device that runs Linux perfectly
17:19 Support the channel


I'll use a Stellaris 15,  with an i7 12700H, 16GB of RAM, 1TB of SSD + an RTX 3060. It has a 1440p screen that I'll run at 60hz.

In terms of operating systems, I'll run default windows 11 with all of its updates and the nvidia game ready drivers, and the latest Ubuntu 22.10 with the proprietary nvidia drivers, on X11, and no other specific customization to the default. 

Ubuntu uses up 25 gigs. On Windows, the install uses 29 Gigs.

Ubuntu's System Monitor reports 1.9 gigs of RAM used after a cold boot. On Windows, the system reports 3.3 Gigs of RAM being used, after a fresh boot.
Although it does report 4.7 Gigs of RAM being cached, which should represent that preemptive memory usage, while Ubuntu reported about 3.9 gigs of cached RAM. If we add used RAM and cached RAM, Ubuntu uses around 5.8 Gigs, where Windows uses 8 Gigs.

I used Kdiskmark on Ubuntu, which reported read speeds of 3360 MBps, and write speeds of 2706. On Windows, I used Crystal Disk Mark, and got read speeds of 3505 MBps, and write speeds of 2782 MBps. 

I ran a speedtest both in Wifi and plugged in using ethernet.

Using Wifi, Windows 11 got a download speed of 108 Mbps and an upload speed of 196 Mbps.
On Ubuntu, the same speedtest over wifi got 154 Mbps for download speed, and 201 for upload. 

Using ethernet, Windows got 512 Mbps down, and 483 Mbps up. Ubuntu, plugged with the same cable, got 508 Mbps down, and only 123 Mbps up.

On to the CPU benchmarks, namely Geekbench 6. On Windows, it gave me a score of 2216 in single core, and 10805 in multi core.

On Ubuntu, the same geekbench 6 got scores of 2494 in single core, and 10138 in multi core.

We're going to run Unigine heaven on both operating systems, at High settings, in fullscreen, at the native 2560x1440p resolution, with tesselation and anti aliasing disabled.

On Ubuntu, I got 114 FPS average, with a score of 2878, minimum FPS was around 20, and max at around 202.

On WIndows, running the same benchmark using openGL with the exact same settings, I got 105 FPS average, with a score of 2665, 7.5% lower, and a minimum FPS of 14, and max of 219.

Running the same benchmark using DirectX 11 on Windows resulted in better performance, with an average of 139FPS, and a score of 3513, but minimum FPS dropping even lower at 10, and much higher max FPS as well, at 283.

For Shadow of the Tomb raider, running the in game benchmark at high details, at the native resolution, I got 80 FPS on average on Ubuntu. On windows, I got an average of 87 FPS, with more stable frame times.

Horizon doesn't have an in game benchmark, but playing the same sequence of fighting this thunderjaw, with the game running at the native 1440p resolution, at high settings, with an uncapped framerate, I got a little less than 60 FPS on Ubuntu. It mostly stayed at around 55 FPS for the whole fight.

On Windows, using the exact same settings, and playing the same fight, I got more around 65 to 70 FPS. Although for some reason the game didn't have any audio, not that I would have heard it over the fan noise that went into overdrive on Windows.

Now, for battery life, I used Firefox on both operating systems, and played youtube videos in a loop until the battery died, over wifi, at mid brightness, in battery saving mode, with nothing else running in the background and Both devices running in hybrid graphics mode.

On Ubuntu, the laptop lasted for 6 Hours and 52 minutes before it died, a little bit lower than what I got when using it with Fedora when I reviewed it.

On Windows, it only endured for 5 hours and 36 minutes.

