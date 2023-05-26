# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## The END of DISTRO HOPPING? All Linux distros in one single system with VanillaOS
 - [https://www.youtube.com/watch?v=tOm_zATjgqU](https://www.youtube.com/watch?v=tOm_zATjgqU)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-05-25 15:55:12+00:00

Try out Kasm Workspaces to stream desktops, OSes & apps to your browser: https://www.kasmweb.com/community-edition

Or you can use KasmVNC, the best open source remote desktop solution on Linux: https://github.com/kasmtech/KasmVNC

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
PeerTube: https://tilvids.com/c/thelinuxexperiment_channel/videos

This video is distributed under the Creative Commons Share Alike license.

#Linux #linuxdistro #vanillaos

00:00 Intro
00:28 Sponsor
00:55 What makes VanillaOS special?
02:59 Install and First Run: user friendly to the max
05:08 What are containers?
06:19 How do you install software?
10:11 How are updates applied??
11:18 Issues with VanillaOS
12:54 Is it the end of distro hopping?
14:12 Sponsor: Get a PC that runs Linux perfectly
15:07 Support the channel

It's one of the very few Ubuntu based distributions that is immutable, and atomic. 
Apart from that, VanillaOS uses GNOME, the most Vanilla GNOME they could ship on Ubuntu, and if you're looking for all the apps, you have access to containers that run other distros at native speeds, and give you access to all their packages.

The installer is something I had never seen before, it looks super good, just like a GNOME app, and will take you through the basic steps, and it even has a nice legible GUI to set up your disk layout. 

After installing and rebooting, you're right into your user session, and you can pick between dark and light mode, if you want to enable support for Flatpak and AppImages, you also get to pick the apps you want to install: you have 3 sets of apps, the core ones, Office apps, and common utilities.

After that, you get the GNOME 43 desktop, which doesn't have any customization or extension.

Now the main point of VanillaOS is to offer the ability to run multiple distros on just one system, with distro containers, using Distrobox. And to manage that, you have the VanillaOS control center.

You can add an Arch subsystem to get access to the AUR, a Fedora subsystem with DNF as the package manager, you get an OpenSUSE container, plus a VOid Linux one, and one for Alpine. Or you can create your own with any other distro you want.

APX is VanillaOS all in one package manager. It lets you install applications for any source that you have access to, including all your distro containers.

The syntax is pretty easy: you just type apx install, followed by the package manager that will perform the actual install, and the package name.

For example, if I wanted to install davinci Resolve from the AUR, I could type:

apx install --aur davinci-resolve

And APX will automatically start my Arch container, and use the arch package manager to install Davinci Resolve from the AUR.

And on top of that, apps installed this way will still show up in your GNOME overview and app grid, just like if they were installed on the base system itself.

And, if you absolutely need to install something to the base system, you can, there's a preinstalled tool called ABRoot, that lets you execute a command, like running apt, since the system is Ubuntu based.

Now for updates, Vanilla OS is not a rolling release, it has fixed releases that follow the Ubuntu release convention. 

Flatpaks you installed through GNOME software or the command line will be updated through the same methods. System updates are handled by VSO, for Vanilla System Operator.

This does mean you'll need more disk space: at least 50 gigs to install the system, and the root partition you don't use. Containers and applications installed in them can be updated by running apx update in a terminal.

But there are issues: as I mentioned, if you need more software from multiple sources, then you need multiple containers. This takes up a lot of space. And if your container dies, so do all your installed applications, and related user data.

The second problem is the disk space usage of the main system: sure having 2 root partitions is great for stability, but it also consumes a LOT of disk space you'll never use.

I also noticed that apps installed from containers sometimes don't show up in the GNOME app grid, and you have to run an APX command to actually add them.

