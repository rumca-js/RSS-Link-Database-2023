# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## Is NOBARA really better than FEDORA? benchmarks, experience, apps, controllers...
 - [https://www.youtube.com/watch?v=5eKSQT5mV-c](https://www.youtube.com/watch?v=5eKSQT5mV-c)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-05-11 15:59:20+00:00

Download Safing's Portmaster and take control of your network traffic: https://safing.io

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

#nobara #fedora #linux 

00:00 Intro
00:38 Sponsor: Secure and monitor your internet connection with Safing
01:36 What changes does Nobara bring?
03:56 Post-Install experience
06:12 Default layout and look
07:28 Gaming Performance comparison
10:20 Package manager & repos
10:54 Controller support
11:24 Davinci Resolve install comparison
13:03 Is Nobara Better than Fedora?
15:17 Sponsor: Get a PC that runs Linux perfectly, from Tuxedo
16:15 Support the channel

Nobara is created by Glorious Eggroll, the creator of Proton GE, which is a more up to date version of Proton to run your games through Steam. Nobara takes Fedora, and adds the Wine dependencies, Steam, all necessary codecs for video playback, 3rd party drivers, like their own packages for the Nvidia drivers, which need a separate repo on Fedora, and a LOT of fixes to various packages.

So, let's compare the post-install process for Nobara and Fedora.
Nobara gives you a welcome app that's actually useful, and will offer to download codecs needed for video decoding and encoding. You can also install drivers there, like the nvidia or amdgpu pro drivers.

It’s not a HUGE timesaver, if I'm honest. Maybe something like 5 minutes after the install.

You can also change the layout and accent colors straight from the welcome app, with layouts based on Windows, Windows 11, macOS, GNOME, GNOME 2, or Unity.

The default experience on Nobara on the "official" version uses a heavily modified GNOME. You get a taskbar, windows style, with Dash 2 panel, and the Arc Menu GNOME extension, for a more traditional menu. You have the APpIndicators as well for notification tray icons, you get BLur My Shell, for blurred translucent elements here and there, you get desktop icons, accent colors that can also be applied to GTK3 and flatpak apps, Pop Shell, for the auto tiling capabilities, and Wireless HID to display the battery level of controllers, keyboards and mice in the battery indicator. Window buttons also include minimize and maximize here.

The laptop uses a 12th gen i7 12700H, with 16 gigs of RAM, and an RTX 3060, and everything runs from an SSD. 

With shadow of the tomb raider, running the game at the native 1440p resolution, on high details, Nobara got 87 FPS on average, with a minimum of 72, and a maximum of 144.

On Fedora, using the same settings, and resolution, I got 83 FPS, with a minimum of 67. 

Running Horizon Zero Dawn, at 1440p, on high details, Nobara got an average of 64 FPS, with a min FPS of 22, and a max of 161, with a score of 11591.

Fedora got an average of 63 FPS at the exact same settings, with a score of 11281, a high of 159 and a low of 21.

And in Total War Warhammer 3, at 1440p, on medium settings and ultra unit size, Nobara reached 71.6 FPS on average, with highs up to 86 and lows down to 58. Fedora, with the same settings, got 69 FPS, nice, with a max of 84 and a low of 59.

Nobara comes with its own graphical package manager, on top of GNOME Software. This thing show everything that is installed, or the available updates. It lets you install flatpak packages, and it has a graphical repo manager.

Just to see if there was any difference between distros, I also tried to connect various bluetooth controllers, namely an XBox Series controller, and a PS5 dualsense.

On Fedora all controllers connected immediately, and worked as intended, without any noticeable input latency. On Nobara, same experience.

On Nobara, installing resolve didn't require anything specific. All the dependencies were already there, the nvidia drivers they package are perfectly good for it. You download it, you run the installer, and it works. Nobara even uses the cuda drivers, which has never been necessary for me on Fedora, I just install the cuda related libraries from the repos, or rpmfusion.

