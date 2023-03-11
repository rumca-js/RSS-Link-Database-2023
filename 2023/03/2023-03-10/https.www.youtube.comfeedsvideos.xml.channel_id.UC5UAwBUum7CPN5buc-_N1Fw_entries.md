# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## Linux Packaging Formats explained: Flatpak vs Snaps vs DEB & RPM vs AppImage vs AUR
 - [https://www.youtube.com/watch?v=1lLZ-59xH3Y](https://www.youtube.com/watch?v=1lLZ-59xH3Y)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-03-10 16:30:11+00:00

Download Safing's Portmaster and take control of your network traffic: https://safing.io

Grab a brand new laptop or desktop running Linux: https://www.tuxedocomputers.com/en#

👏 SUPPORT THE CHANNEL:
Get access to a weekly podcast, vote on the next topics I cover, and get your name in the credits:

YouTube: https://www.youtube.com/@thelinuxexp/join
Patreon: https://www.patreon.com/thelinuxexperiment

Or, you can donate whatever you want: https://paypal.me/thelinuxexp

🎙️ LINUX AND OPEN SOURCE NEWS PODCAST:
Listen to the latest Linux and open source news, with more in depth coverage, and ad-free!  https://podcast.thelinuxexp.com

🏆 FOLLOW ME ELSEWHERE:
Website: https://thelinuxexp.com
Mastodon: https://mastodon.social/web/@thelinuxEXP
Pixelfed: https://pixelfed.social/TLENick
Twitter : http://twitter.com/thelinuxEXP
PeerTube: https://tilvids.com/c/thelinuxexperiment_channel/videos

This video is distributed under the Creative Commons Share Alike license.

#flatpak #linux #packages 

00:00 Intro
00:33 Sponsor: Monitor and Secure your internet connection
01:38 Regular Packages: DEBs & RPMs
04:53 Flatpaks
08:56 Snaps
11:29 AppImages
14:11 The Arch User Repository
16:35 These formats aren't important
17:40 Sponsor: Get a device that runs Linux perfectly
18:28 Support the channel

DEBs & RPMs are contained in repositories that your distribution set up or that you add yourself. 
In terms of advantages, these packages are all separate, which means that each package contains either an application or a library: you only install what is needed, nothing more. This also means they tend to use less space as time goes on.

Second, they're maintained and tested by your distributions, which means they should all work well without any issues.

Third, they're all based on a dependency system: applications declare which other packages they need to run.

You install a package as a superuser, which means you grant the package all the rights to do whatever it wants to your system as it's being installed. They also can create dependency hell.
These packages need to be made for every architecture, and for 32 bit and 64 bit, for all the currently supported versions of a distribution, and for all distributions.

And that was the main reason why Flatpaks were invented. It packages the application and everything it needs to run in a single bundle. If the application depends on a LOT of libraries that are commonly used by other applications, it can install what's called a runtime instead.

Flatpaks are only meant for graphical applications: they aren't a way to distribute libraries, or command line apps. Flatpaks are generally hosted on Flathub, but there are others repos.

Flatpaks are more secure than regular packages. They're installed as a regular user, and can't install crap that will run at the system level. They can also use a sandbox, with permissions.

Another advantage is for app developers: flatpaks run on any distribution that has flatpak installed, which is basically all of them apart from Ubuntu and its various flavors.

It also means you're not dependent on your distribution for updates: you can get the new versions of your app as soon as the developer has published them. Last advantage is no dependency hell.

Flatpaks tend to use more space, and they can''t fully replace packages: they are only for graphical programs. Finally, flatpak apps might not follow your custom themes.


You can install Snap packages on Ubuntu and all of its derivatives, or any distro that can install the snapd package. They're auto updated and containerized. Snaps also let you test future releases in advance, with "channels". While the packaging format is open source, the server component isn't.

Snaps are very slow to open at first start. They tend to clutter your mount points. Snaps also generally don't support your custom themes. Snaps do have the advantage of supporting command line utilities.

AppImages are an all in one bundle that packages the application and all its libraries in a single file.
They're very portable. They also won't create dependency hell, since they're completely independent. Appimages can be sandboxed but not a lot of them are. Appimages don't integrate with your system at all. They also use more space than any other packaging format.

Next is the AUR, it means Arch User Repository. it's available on Arch Linux and other Arch based distros like Manjaro.

The AUR is a big repository of applications and libraries packaged by individuals: they're generally not official, and not supported by the distro or the original developer.

Its main advantage is that is has virtually everything. The AUR doesn't host packages, but packagebuilds, which are scripts that will make the package.

This means that installing something might take a bit longer, and it also means that unless you read the package build scripts yourself, you completely trust an individual with the security of your system.

