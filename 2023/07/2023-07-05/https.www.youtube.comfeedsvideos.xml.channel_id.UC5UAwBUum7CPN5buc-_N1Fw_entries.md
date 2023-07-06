# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## The LINUX DISTRO model is BROKEN
 - [https://www.youtube.com/watch?v=8yAo9Bc6iOI](https://www.youtube.com/watch?v=8yAo9Bc6iOI)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-07-05T15:39:20+00:00

Stream any OS, desktop, or app to your browser, now with translations: https://kasmweb.com/docs/develop/developers/builds.html

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

#Linux #linuxdistro #operatingsystem 

00:00 Intro
00:35 Sponsor: Stream any OS, desktop or app to any PC
01:29 The Classic Linux Distro Model
02:57 Why it's broken
04:25 Distros are moving away
05:52 The new model isn't perfect, but still better
08:31 All other OSes do this
09:22 Why distros package apps in the first place
10:14 Universal Packages
11:40 You don't have a choice
13:32 Sponsor: Get a PC made to run Linux
14:27 Support the channel


This video was inspired by the following blog post, which echoed my sentiment and ideas exactly: https://www.ypsidanger.com/the-distribution-model-is-changing/

The distro packages the software for their users. Not the developers of the software, the distro itself. So the distro has a decent amount of control over what they offer, but the users of the distro don't, and the developers of the apps also don't. And this model doesn't really work.

On the surface, for users, it does work. You get a lot of applications from a central repo, and the system is generally pretty stable, depending on the distro you pick.
But in the background, you have the thousands of orphaned packages that are still in the repos but aren't maintained. The old apps that can't be packaged at all anymore. The maintainers spending a lot of time repackaging and recompiling software that has already been packaged.

One might not like Ubuntu's snap packages, or Flatpak, or AppImages, but it's undeniable that most distros are moving towards them.

When Ubuntu moves Firefox and Chromium from a deb package to a snap, it's a GOOD THING. For Ubuntu. Because instead of having to package each new version of Firefox or CHromium for all currently supported versions of Ubuntu, they only have to package them once.

Same thing when Red Hat drops the LibreOffice RPM in favor of the Flatpak. Not having to package that behemoth of an app will free up time for Red Hat developers to work on HDR, improving Wayland, and supporting color management.

And moving the packaging of an app from the distro to the app developer means less time spent debugging stuff, and more time spend on improving the app.

So why did Linux distros start packaging software instead of app developers?

It was because there were so many different systems using the same packaging formats, deb or RPM or whatever else, but different libraries, kernels, drivers, and everything else, that app developers simply did not have a way to distribute their own software to every distro.

But nowadays, we DO have formats that let you distribute applications everywhere with one single package.

They lack some features, especially due to the sandboxing they tend to use, that limits how they can interact with other apps. Thing is, these formats are still under heavy development.

But the real question is: do you prefer staying on the current model where we stagnate, duplicate work, and where developers and users have no control over which version of the software is used, or would you rather face a few teething issues, but let developers improve their apps, and the whole of the Linux software ecosystem?

I know what I choose, and it's not these old packages. And presumably, if you stick to mainstream distros, like Fedora, Ubuntu, or their main derivatives, chances are you're not going to have a choice either. Because whether you like it or not, we're moving to Flatpak or Snap on most distros.

It's more efficient, and their current problems can and will be fixed. The duplication of work that legacy packaging creates is unfixable, it's a structural problem.

And of course, if you hate these universal packaging formats, I'm sure you'll still be able to find a lot of distros that will not move to them even in the future. You'll just be running the non official version of an app, just like what you're doing right now when using a distro's package.

