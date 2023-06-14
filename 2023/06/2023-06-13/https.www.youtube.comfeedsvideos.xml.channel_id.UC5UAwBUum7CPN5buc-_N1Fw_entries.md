# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## LINUX vs WINDOWS: the graphical gap is still there
 - [https://www.youtube.com/watch?v=5-DD4AvtuyU](https://www.youtube.com/watch?v=5-DD4AvtuyU)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-06-13 16:04:11+00:00

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
PeerTube: https://tilvids.com/c/thelinuxexperiment_channel/videos
Matrix: https://matrix.to/#/#the-linux-experiment:mozilla.org
Discord: https://discord.gg/XMuQrcYd

#Windows #Linux #apps 

00:00 Intro
00:42 Sponsor: Take back control of your internet connection
01:39 Managing Devices
04:20 Managing Services
06:15 Firewall Configuration
07:18 Device Security
08:41 Backup and Versioning
09:45 Advanced Configuration
11:15 Command line: not enough
12:53 Sponsor: Get a PC that runs Linux perfectly
13:55 Support the channel

GNOME Dconf video: https://www.youtube.com/watch?v=dLsj8plxBn0&amp;t=901s

Device manager lets you see all the components of your PC, and the devices plugged into it. It lets you check for drivers, fix various problems, set some options, and view some logs related to your devices.

On Linux, this thing has no equivalent. We do have a third party app called HardInfo, but it's not an actionable application. In KDE, you have the same thing, with the Info Center.

Device manager is an important tool on Windows, and it would have a LOT of uses on Linux as well. I wish we had something like that.


Linux runs services in the background, for printing, bluetooth, network, virtualization, the graphical server or compositor, and a lot more things, generally managed by systemd on most distros.

And almost no Linux desktop has a complete graphical user interface to manage these services, turn them on or off, enable one at startup or not, or view logs related to this service.

On GNOME, you have an extension called systemd-manager, but no way to configure them, or select options, or enable autostart. On KDE, you have a services page in the settings, but you can basically just start and stop them, no other action is available.

As far as I know, only OpenSUSE has a decent services manager, that is baked into YAST, their configuration tool.

On Windows, the services app might look like it's 20 years old, which it probably is, but it lets you start and stop services, select if you want to start them manually, or at boot, or completely disable them, and it lets you set policies for various services failures, like restarting the computer, restarting the service, or opening another program.


Another thing that is not entirely available in our desktop environments is a graphical tool to configure the firewall, and general system security.

KDE has a config module in their settings, so that's handled. And yet again, OpenSUSE has a firewall config tool in Yast, which works really well.

For GNOME, there are third party tools you can install, depending on the firewall the distro uses, like firewall-config for firewalld, but these are rarely provided by default.

Linux desktops also don't really have an equivalent to the Windows "security center". GNOME has the basics of such an implementation, with their device security page, but it's not actionable.

Anyway, we could add here some information depending on certain libraries, apps, and kernels we use, if vulnerabilities have been detected, we could have access to the firewall settings, apps that have incorrect permission...

And then we have backups. A lot of distros ships with a third party backup tool, like Déja Dup, or Timeshift, but they generally only ship one or the other. We sort of need a complete solution that works ideally for both.

What I'd want is to right click on a file in my file manager, and have a "versions" menu item. What I'd like is a system settings option, native to the desktop environment, that lets me configure a backup, and restore it.


The windows registry is a horrible, horrible thing. It's illegible, it's super messy, modifications can result in a horrendously broken system, and generally it's better left alone. 
But it does surface a LOT of options for applications and the system. And not all Linux desktops have an equivalent. 

GNOME has dconf, which has a lot of various settings you can tweak. KDE doesn't have that.
Yast has a bunch of additional configurations available graphically.

