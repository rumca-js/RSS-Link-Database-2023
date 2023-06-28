# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## SteamOS CONSOLE: the BEST gaming experience, but not worth it
 - [https://www.youtube.com/watch?v=TUiDQjWMJB4](https://www.youtube.com/watch?v=TUiDQjWMJB4)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-06-27 15:42:48+00:00

Download Safing's Portmaster and take control of your network traffic: https://safing.io

👏 SUPPORT THE CHANNEL:
Get access to a weekly podcast, vote on the next topics I cover, and get your name in the credits:

YouTube: https://www.youtube.com/@thelinuxexp/join
Patreon: https://www.patreon.com/thelinuxexperiment
Liberapay: https://liberapay.com/TheLinuxExperiment/

Or, you can donate whatever you want: https://paypal.me/thelinuxexp

👕 GET TLE MERCH
Support the channel AND get cool new gear: https://the-linux-experiment.creator-spring.com/

🎙️ LINUX AND OPEN SOURCE NEWS PODCAST:
Listen to the latest Linux and open source news:  https://podcast.thelinuxexp.com

🏆 FOLLOW ME ELSEWHERE:
Website: https://thelinuxexp.com
Mastodon: https://mastodon.social/web/@thelinuxEXP
Pixelfed: https://pixelfed.social/TLENick
PeerTube: https://tilvids.com/c/thelinuxexperiment_channel/videos
Discord: https://discord.gg/mdnHftjkja

#steamdeck #steam #linuxgaming 

00:00 Intro
00:45 Sponsor: Secure your internet connection
01:43 What I wanted from this SteamOS Console
02:48 Console in name only
04:39 The specs
06:03 SteamOS / HoloISO: not easy
11:40 Performance: top notch
14:10 Not worth it, but I love it!
15:51 Support the channel

Fix for AMD GPU bad performance https://bbs.archlinux.org/viewtopic.php?id=271286

I went for a Micro ATX PC, which means that, yes, it doesn't look like a console, but it was easy to install the GPU, it has ample room for cooling, and it sort of fits in my TV cabinet, so who cares. It's a Tuxedo Cube.

So here I have an intel core i7 12700,. I have 32Gigs of 3200Mhz RAM, I have a 1TB PCIE4 SSD, with a 750W modular power supply. For the GPU, I got a Radeon 6650XT off Amazon for 300 euros.
The total cost is a bit less than 1400€, which isn't cheap.

On it, I installed HoloISO, which had issues:
First, the default kernel they pick doesn't work with a lot of hardware, it lacks support for a bunch of things, so I had no Wifi and no Bluetooth support. Fortunately, they also ship with the holoiso kernel, which is more mainline, and does support a lot more things. You can select it during boot, with GRUB.

So I turned to the controversial Grub customizer, that's a graphical app that lets you tweak your grub boot options. HoloISO, like SteamOS, is based on Arch, but they don't really ship a correct pacman config with the correct repos, so I had to manually edit the pacman config to add the necessary repos to it, and then run a full system update, followed by the install of Grub Customizer.

And it flat out didn't work, it couldn't open the grub config file. That's because that file is preconfigured with conditions to boot with specific options on certain devices. I just commented all these conditions, and then Grub Customizer managed to open the file, and I could set the HoloISO kernel as the default boot option.

All games ran at 720P max. Of course, a simple web search gave me the answer, it's because SteamOS is meant for the steam deck, but you can change all that in the game's properties to select the max resolution you'll allow.

Then, the performance was horrible. I couldn't manage 1080p60 in Spiderman at medium details, Jedi Fallen Order had to run at 768p on medium to even get close to 60FPS, it was a mess, and this system should have been able to give me a lot more.

After a few hours of looking online, I found a solution: some AMD cards on Linux run in low power mode by default, and don't move to full power when you need them to.

But how's the performance then? Well, I can play virtually everything at least at 1440P, max settings at a smooth 60FPS.

I've completed a full playthrough of Spiderman, also running at 1440p high settings, upscaled to 4K through in game FSR. I've played about 13h of Cyberpunk at max details, 1440p upscaled to 4K through the in game FSR, with sharpness turned to the max, and it maintains 60FPS no problem, even when driving around in the city.

I played about a third of Red Dead Redemption 2, also running at 1440p, high settings, upscaled to 4K through HoloISO, at a smooth 60 fps as well. Everything can run at 4K High details, from 50 to 60 FPS.

And so this makes this console a better performer than a PS5, because PS5 rarely runs AAA games at 4K60, generally, if you want 4K high details, you're using quality mode, and you're running at 30FPS, not 60.

The performance mode on PS5 generally runs games at 1440p, and either medium or high details.

Cost wise, compared to a PS5, it's very expensive for a marginal visual improvement. And yet, I love it, and I plan to play everything I can on this and not on the PS5.

Because it runs Linux, and I love Linux. It also works with an Xbox controller, which I prefer to the dualsense 5. Also, my game library is mostly in Steam these days. I can also start a playthrough on my TV, and then pick up my Steam Deck, make sure my saves are synced, and go play on that outside, or in bed, or on holidays.

