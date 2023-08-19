# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## What are immutable distros, and are they the future of Linux?
 - [https://www.youtube.com/watch?v=9hiPFEUoUyI](https://www.youtube.com/watch?v=9hiPFEUoUyI)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-08-18T15:53:27+00:00

Head to https://squarespace.com/thelinuxexperiment to save 10% off your first purchase of a website or domain using code thelinuxexperiment

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
Discord: https://discord.gg/XMuQrcYd

#Linux #immutable #linuxdistro 

00:00 Intro
00:33 Sponsor: 10% off your first website with Squarespace
01:26 What is an Immutable Distro?
03:30 Advantages
05:16 Installing software
07:44 Updating software
10:48 The Complexity problem
12:01 Are they the future?
13:26 Sponsor: Get a PC made to run Linux
14:29 Support the channel

They are linux based operating systems that are designed to be read-only and not easily modifiable.

Most of these immutable distros still let you install apps and packages on top of the system, through flatpaks, snaps or appimages, or with a specific layer of packages, that is kept when rebooting and updating. Some immutable distros give you easy access to containers so you can still use a full system with full write access.

And there are a BUNCH of immutable distros: Fedora Silverblue, and Fedora Kinoite are basically Fedora Workstation, with GNOME or KDE, but with an immutable base. Vanilla OS is an Ubuntu based, soon to be debian based immutable distro that gives you access to any packaging format through containers. BLendOS does the same thing, but based on Arch. SteamOS, the linux distribution that powers the steam deck, and also my Linux gaming console / PC is also immutable.

You could also say that NixOS is an immutable distribution, since you only install things and modify configurations through a declarative config file that is used to build the system. And there are a lot more, like microOS from openSUSE, endlessOS, and more!

So in terms of advantages, immutable distros are just way more secure. Since you, the user can't modify the base system, and since the super user can't do it either, it also means any third party programs also can't modify that base system.

Another advantage is reliability. Since you can't tinker with the system files, you also have a much smaller chance of actually destroying your system.

And in terms of maintenance, since you only use an updated system after a reboot, there is no risk of breaking something by updating it while it's running.

But how do I install anything if I can't write to the system? Most immutable distros work around that using universal packaging formats like flatpaks, snaps and appimages.

But that's not the only way to install stuff to an immutable distro. A lot of them actually still let you install packages to the system, in a dedicated layer. That's called "layering".

WHat this means is that you still have access to the distro's repos of packages, and you can still elect to install some, but you won't use the usual package manager, but another dedicated tool. 

Some immutable distributions also use containers, generally with something like distrobox.

Another difference that can be considered a drawback is updating. Updates on immutable distros are never applied in place. When an update is available, they'll build another system image. So you end up with 2 systems; the one you're currently using, and the updated one, which is not currently active.
And you only get the updates after you reboot onto that new system image.

Another drawback is the complexity of these systems. Everything you try to do is different: installing a package doesn't use your usual package manager. Applying updates isn't the same command, or requires you to reboot to actually use the updated system.

Immutable distros are a different sort of system, with different tools to interact with things you might already know how to do.

Are they the future? Probably not. For servers, they make a lot of sense. For regular users, they do have a lot of advantages, but they also have a bunch of limitations that require the use of workarounds.

And so I don't think immutable distros will replace regular distros. They'll grow, and occupy a space next to let's call them "mutable" systems, but they'll probably never be the default thing most people use.

