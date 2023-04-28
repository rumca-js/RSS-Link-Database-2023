# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## OpenSUSE Tumbleweed is the best rolling release, but it's not perfect
 - [https://www.youtube.com/watch?v=RSaUj_Okbnw](https://www.youtube.com/watch?v=RSaUj_Okbnw)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-04-27 15:59:43+00:00

Check out AlmaLinux and TuxCare's support services: https://bit.ly/3EuSwPU 

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

#Linux #opensuse #linuxdistro 

00:00 Intro 
00:47 Sponsor: Check out AlmaLinux and TuxCare's support services
01:54 OpenSUSE Tumbleweed
02:53 Installer: not the best
05:47 Default desktop experience
06:42 Yast: managing software
08:39 Yast: configuring the system
12:50 Interesting things
14:40 Conclusion
16:13 Sponsor: Get a PC that runs Linux perfectly, with Tuxedo
17:12 Support the channel

It's a rolling release Linux distro, but they test everything thoroughly through their own build service. 

Lets talk about the installer. First, you get a licence agreement.Y ou get very complete network settings, but they're not user friendly at all. Then you get to pick the role of your system: do you need a desktop, with GNOME, Plasma, or XFCE, a generic desktop for a minimal install, or a server. You can also get other desktop environments from the repos afterwards, like Cinnamon, MATE, LXQt, or even just a window manager, like i3.

OpenSUSE tumbleweed is one of the rare distros I installed using all its defaults that did NOT manage to give me a bootable system. I reinstalled it, this time carefully picking my partition layout, and this time it worked.

Once I managed to boot the system, I got a very vanilla GNOME experience, with GNOME 44. No extensions, no themes, it's the default experience, and that's great.

On KDE, there's a tiny bit more customization applied, with an OpenSUSE logo as the menu, and the titlebars defaulting to the breeze classic look, instead of the cleaner "regular" color scheme. It doesn't depart from the base KDE layout, it's still super vanilla.

Tumbleweed comes with a lot of preinstalled software, like Evolution, GIMP, LibreOffice, a few games, Tiger VNC, Transmission, and of course, the Yast utility. Flatpak is preinstalled, and flathub is enabled, which is really good.

Yast is a control center and setup utility that's been the mainstay of OpenSUSE for years, basically since its first version. It lets you configure your system in depth, way more than what the default settings in GNOME or KDE let you do.

So, first, Yast lets you manage software. You can add, remove or edit software repositories, and their GPG keys, and you can install packages or apply patches.

This opens a very complete graphical package manager that reminded me of Synaptic. You can install libraries, drivers, whatever is not available in GNOME Software or Discover. It's all RPM packages.

But YAST is also a super complete tool if you want to configure a lot of advanced settings graphically. Yast lets you configure the boot loader entirely, you also get a services manager, to let you enable, or disable various services that run in the background. There's a sysconfig graphical editor, to set various variables related to your desktop. And then there are security settings, for AppArmor, configuring the firewall, hardening the system by disabling or enabling various features and settings, and you can consult the logs, all graphically.

You can also manage printers and scanners, but, the built in tools for this are... not great. 

And then there are things I don't think are really needed anymore in a separate tool, like the date and time settings, the language settings, the network settings, the partitioning tool, all of these have equivalents in the Plasma or GNOME desktops, and as far as I can tell, the Yast utilities don't do more than the built in tools.

Once I used it, I started to wonder why desktop environments don't give users access to these configs, or why there isn't a third party tool to manage these.

Tumbleweed also comes with a graphical btrfs snapshot manager: It lets you create or delete snapshots, which you'll be able to restore to revert your system to a usable state.

OpenSUSE also has a web portal to find and install applications.

