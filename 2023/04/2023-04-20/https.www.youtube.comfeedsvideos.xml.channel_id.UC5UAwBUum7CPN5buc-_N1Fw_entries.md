# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## NVIDIA on Linux is WAY BETTER than everyone says, but...
 - [https://www.youtube.com/watch?v=9f4B8uIPqcE](https://www.youtube.com/watch?v=9f4B8uIPqcE)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-04-20 16:02:19+00:00

Download the free report on managing cyber threats using the MITRE ATT&amp;CK framework and live patching: https://bit.ly/41zVI5O

Grab a brand new laptop or desktop running Linux: https://www.tuxedocomputers.com/en#

👏 SUPPORT THE CHANNEL:
Get access to a weekly podcast, vote on the next topics I cover, and get your name in the credits:

YouTube: https://www.youtube.com/@thelinuxexp/join
Patreon: https://www.patreon.com/thelinuxexperiment
Liberapay: https://liberapay.com/TheLinuxExperiment/

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

#nvidia #linux #gpu 


00:00 Intro
00:46 Sponsor: Free report on cybersecurity with the MITRE ATT&amp;CK framework
01:26 Nvidia Drivers
03:27 Screen Tearing
06:04 Multi Monitor support
07:34 Hybrid graphics
10:10 Wayland Support
11:48 Power Management
13:04 It's not the whole story
14:09 Why would anyone pick Nvidia, though?
15:26 Sponsor: Get a PC that runs Linux perfectly, from Tuxedo
16:19 Support the channel


Drivers are a one click install from the graphical app store. DO NOT install them manually from the nvidia website, and don't mess with kernels that your distro doesn't officially pack.

So, a first big issue people report with nvidia drivers is Screen tearing. I plugged my desktop's RTX 3070 into a basic 1080p monitor. That desktop uses X11, and  tearing just isn't a thing here.

Now, if I launch a game to see how well things go, for example Darktide, with v sync off, we can clearly see some big tearing happening. With vsync on, it disappears.

If you still have tearing, you can auto start a command when your computer starts, with the following command line:
 
nvidia-settings --assign CurrentMetaMode="nvidia-auto-select +0+0 {ForceFullCompositionPipeline=On}"

Add that command to your startup applications, and you're done.

But how about multi monitor support? I plugged my laptop running Wayland, into the same external monitor, the basic 1080p one, using the hdmi port that's connected to the nvidia dedicated GPU.
Nothing to say here, it just works.

I also plugged in 2 displays onto my desktop, the 1080p one, and my usual 1440p ultrawide, straight into the RTX3070.

No problems here, both displays are detected immediately. Same experience with KDE Plasma, no issues to report here, multi monitor support works normally.

Now, another thing people tend to hold against nvidia drivers is the hybrid graphics support, as in you have a laptop with a dedicated GPU from Nvidia, and an AMD integrated chip, or an Intel one.

On Wayland, it seems that hybrid mode is the default, and the only mode you can use, I could not find a way to move it back to the intel GPU only, or Nvidia only. Hybrid mode works perfectly.

On X11, the experience is pretty much the same. Hybrid mode is the default, and you do get a bunch more options in the nvidia control panel.

Nvidia has the reputation of not working with Wayland, but that's not true anymore. Everything works as it would on a normal wayland session: touchpad gestures, no screen tearing, fractional scaling support, screen sharing and recording, and running any application. Same experience on KDE with Wayland, it just works.

On my laptop, closing the lid will suspend the laptop. But very regularly, opening the lid doesn't wake the laptop back up, and I get a black screen.

I can get out of it by just getting into a TTY, then moving back to TTY1, and I'm good, but it's not what I'd call a smooth experience.

On my desktop, running Fedora also but with X11, suspend works perfectly, and resuming also happens without any issues.

All my tests are done using the latest nvidia drivers available on Fedora 37 with GNOME, and on Ubuntu 22.10 with KDE 5.25, and all these devices have relatively recent Nvidia GPUs. So it's only 2 distros, 2 desktop environments, and 3 different cards from the same generation.

Support for older GPUs, like the RTX10 series, or older ones, might not be as good, and might require you to use older legacy drivers, which very probably won't support Wayland, and might have more issues.

