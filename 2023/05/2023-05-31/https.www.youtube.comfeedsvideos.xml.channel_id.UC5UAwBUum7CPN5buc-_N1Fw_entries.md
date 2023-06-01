# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## Windows, macOS & Linux PRIVACY compared: why do they need ALL THIS DATA?!
 - [https://www.youtube.com/watch?v=MMc5zgALLiY](https://www.youtube.com/watch?v=MMc5zgALLiY)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-05-31 15:23:27+00:00

Try out Proton Mail, the secure email service that protects your privacy: https://proton.me/mail/TheLinuxEXP

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

#Linux #macos #windows 

00:00 Intro
00:34 Sponsor: Try Proton Mail, the secure & private email service
01:48 Windows Data collection
04:33 Windows 3rd party requests
06:07 How bad is Windows?
07:05 Disable Windows data collection?
07:58 macOS data collection
09:37 Disable macOS data collection
10:34 How bad is macOS?
11:23 Linux Distributions
13:52 Sponsor: Get a PC that runs Linux perfectly
14:52 Support the channel

So if you've installed Windows 11 recently, you're familiar with the very lengthy setup process where you can uncheck a lot of toggles to try and limit what the OS collects.

What the OS will collect is the following:
- Microsoft Store Logs
- Network data
- Hardware information
- Accessory data
- Application-related data
- Event metrics

You'll also send complete words that you typed or wrote, not just statistics. You'll also send speech recognition data, and activity history, so every document you opened, website you visited...

But that's just what Microsoft tells you about. Recently, a youtuber called "The PC Security channel" analysed a completely fresh Windows install, using Wireshark, and what they found was is that Windows makes a few connections to third parties it never really told you about.

THEIR VIDEO: https://www.youtube.com/watch?v=IT4vDfA_4NI&amp;t=271s

- trustedsource.org.

- scorecardresearch.com

- Bing and msn.com

- privacyportal.onetrust.com

So what exactly can Microsoft do with all this data?

Well, they have more than enough to completely fingerprint your device, they can reliably tell what you use in terms of apps, and what type of content you watch, and they also basically can have a keylogger on your computer. And finally, Windows sends some data to third parties.

Fortunately, you can disable all the option stuff straight from the settings.You can go to the privacy and security options, and go into each category and disable everything there.

You can also completely disable the telemetry service. Just hit Windows + R, and in the run dialog, type services.msc. In there, look for something called "Connected user experiences and telemetry", double click that, and in the "General tab", you can set "startup type" to "disabled".


Apple talks a big game when it comes to privacy, but in the end, is it really true?
Out of the box, macOS sends to Apple your IP address, location, and some usage patterns, like all the apps you run, and when you run them. Other telemetry data, out of the box, includes browsing history, search history, crash data, performance and diagnostic data, location information, health information if you use that on an iPhone for example, all the info you entered in your AppleID, the device serial number, payment information, everything you bought using that Apple ID, and potentially your government ID.

Fortunately, macOS lets you disable virtually everything that's being collected. You can just head over to the Security and Privacy settings, and in analytics and improvements, uncheck everything. 

Now, how about Linux? Well, Linux based operating systems, or at least desktop Linux distributions don't collect any data out of the box, with a few exceptions.

The first one is Ubuntu, who will collect telemetry data out of the box, with no personal information at all. It's just hardware data, but it could still be used to fingerprint your device. Canonical doesn't currently have any ad server that I know about, so they probably only really use this to know what their users actually use and focus their efforts on that, but if you're uncomfortable with that, you can disable it at install.

Some Ubuntu derivatives that use the same installer might also have that kind of telemetry. On top of that, you have the ability to turn some entirely optional telemetry on in KDE's settings; and GNOME also has a telemetry tool that you have to install manually.

