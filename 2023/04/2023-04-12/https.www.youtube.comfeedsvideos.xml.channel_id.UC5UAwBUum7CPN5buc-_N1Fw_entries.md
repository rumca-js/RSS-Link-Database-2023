# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## APPS & TOOLS to improve LINUX PRIVACY & SECURITY
 - [https://www.youtube.com/watch?v=0LxUF5bcRXI](https://www.youtube.com/watch?v=0LxUF5bcRXI)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-04-12 15:56:56+00:00

Get 100$ credit for your own Linux and gaming server: https://www.linode.com/linuxexperiment 

Grab a brand new laptop or desktop running Linux: https://www.tuxedocomputers.com/en#linux 

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

#linux #privacy #security 

00:00 Intro
00:31 Sponsor: 100$ Free credit for your Linux or Gaming server
01:31 Encrypt your system or specific folders
03:36 Anti-virus
05:23 Sandboxing and application permissions
07:28 Web monitoring and blocking, & VPNs
10:08 Portable private Operating system
11:08 Web browsers & search engines
12:58 Other tools
14:40 Sponsor: Get a PC that runs Linux perfectly, from Tuxedo
15:37 Support the channel

A lot of Linux distributions will offer to encrypt your hard drive when you install them. Ubuntu, PopOS, elementary OS, and a lot more, they all have this option. If you didn't enable encryption when installing your system, you can encrypt your home folder or partition after the fact using ecrypt-utils, a command line utility.

ENCRYPTION TUTORIAL: https://jumpcloud.com/blog/how-to-encrypt-ubuntu-20-04-desktop-post-installation

KDE has something called Plasma Vaults, that lets you create encrypted folders with a nice graphical interface, with the ability to set different passwords for each folder. 

You probably also have an anti virus, your best option will be ClamAV (and ClamTK, it's graphical interface). it detects trojans, viruses, malware and the like, it's open source, and it's completely free of charge.

But if you want to restrict permissions for Flatpak apps, then you need Flatseal. It's an application that will list all your flatpak apps and let you grant, or remove permissions to them.

If you want the benefits of a sandbox but without using Flatpak apps, you can also run any app installed from a regular package or an AppImage in a sandbox, using Firejail, and Firetools, its graphical interface.

If what you want is to make sure that the apps or services you run don't do anything weird with your internet connection, then there's Safing's Portmaster. It's open source, free of charge, and it lets you monitor every network request every part of your system makes, and restrict them as you see fit. Oh, and it also has a system wide ad and tracker blocker.

VPNs are a tool you can use to be more private online. I don't have any specific recommendations, but you can check the link I left in the description to TechLore's VPN chart to find one that is suitably private:  https://techlore.tech/vpn.html

If you regularly use public computers, or someone else's, you might want to use TAILS, a live USB, but with persistent storage that is encrypted. 

Your web browser will also be a big part of how private you are on the internet. If you prefer to stick to Chrome's rendering engine, then something like Brave will be way less intrusive and well configured by default, and if you don't want to encourage Google's monopoly on the internet, then Firefox is also very private, once you disable the opt-out telemetry in the Privacy and Security settings.

You also have LibreWolf, which is Firefox without the telemetry and with privacy focused search engines out of the box.

Speaking of which, your search engine is also something you should look at for privacy. Google or Bing are just NOT what you want for that. I personally use Ecosia as my default search engine. When Ecosia falls short, I use startpage, which is basically Google's results, but with complete anonymization of all queries, so Google doesn't know who or from where the query has been made.

VIDEO ON SEARCH ENGINES: https://www.youtube.com/watch?v=x9q3qPxrTqg

Bleachbit will let you delete cache files, cookies, internet history, temporary files, logs and more.

If you want to just completely delete any single file, then there's GNOME File Shredder.

If you need to share certain images but hide some information on it, blurring it with a gaussian blur isn't enough, as it's now relatively easy to deblur an image. Obfuscate is a simple tool that lets you hide information.

