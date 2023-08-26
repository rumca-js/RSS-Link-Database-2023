# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## 10 great GNOME extensions & tools you didn’t know about!
 - [https://www.youtube.com/watch?v=KtjYPMCvQ7Y](https://www.youtube.com/watch?v=KtjYPMCvQ7Y)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-08-25T16:08:45.276597+00:00

Stream any OS, app or desktop straight to your browser: Kasm Workspaces Community Edition – https://www.kasmweb.com/community-edition

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
Discord: https://discord.gg/mdnHftjkja

#Linux #GNOME #ricing 

00:00 Intro
00:33 Sponsor: Stream any app, desktop, or OS to your browser
01:29 Fly Pie: system menu
03:01 Forge: Tiling window manager
04:02 Gradience: colorful desktop
05:59 Just Perfection: tweak everything
07:27 Advanced Alt Tab Window Switcher
08:39 Custom Hot Corners Extended
09:47 Login Manager
10:34 Pano: visual clipboard
11:32 Misc Extensions
12:59 Sponsor: Get a PC made to run Linux
13:56 Support the channel


FLy Pie is a circular menu you invoke with the mouse. And as you get familiar with it, you end up memorizing these gestures: you move your mouse in specific patterns to launch specific things.

By default, you can press control + space to open that, but you can change that shortcut. It also works on Wayland, you just need to create a custom keyboard shortcut that launches the command:

gdbus call --session --dest org.gnome.Shell --object-path /org/gnome/shell/extensions/flypie --method org.gnome.Shell.Extensions.flypie.ShowMenu 'YOURMENU'

If you like tiling your windows, but GNOME's options are too limited, there Forge. Each new window opens in a new tile, and you can either drag and drop them using the mouse to reposition them and create your layout, or use a long list of keyboard shortcuts to do the same thing.

Gradience lets you apply color palettes to the default Adwaita theme of GNOME: it won't change the shape of buttons and controls,  but it will tint everything with colors of your choosing. It lets you either pick each color yourself, or you can let it create a color palette from an image. It will apply all these changes to all your GTK4, and GTK3 apps, provided you have the adw-gtk3 theme installed. 


Just Perfection comes with a few profiles to reduce the size of the top bar, or get rid of it entirely, but you can also have complete control over everything. It lets you change a lot of various variables, like the panel size, the panel icon size, the padding between indicators, the position of the clock menu, the sped of animations, the size of dash icons, the position of notification banners, the on screen display elements position, and more.

If the default Alt tab window switcher doesn't work for you, then there's AATWS, for Advanced Alt Tab Window switcher.

This thing is the just perfection of ALt tab. It changes how the window switcher AND the app switcher works. You can choose the position of each, at the center, bottom, or top of the screen, choose on which monitor this switcher appears, and how everything looks.

But if you prefer using your mouse to do stuff, then maybe you're lamenting the lack of hot corner functionality in GNOME. Thankfully you have CHC E, for Custom Hot Corners Extended. It lets you define actions for pushing your mouse in any corner of the screen, including with modifiers: you can define an action for when you just place your mouse in the top right corner, of when you do that while holding COntrol, or while clicking any of the buttons, or while scrolling the mouse wheel.

Another app, not an extension, is Login Manager settings. This one lets you tweak, as its name implies, the login screen of GNOME. 

If you need a clipboard manager, to keep track of everything you copy, Pano is probably the best looking one. it's an extension that lets you display all the elements you copied in a visual manner, as a strip at the bottom of your screen.

Search light gives you a launcher / spotlight equivalent. 

Then you have Rounded window corners, which will round every corner of every window, even for apps that aren't GTK4 and aren't natively round.

If you're missing these awful desktop icons, you can also add them back, with Desktop Icons NG. it's super customizable, and it restores that functionality if that's something you enjoy.

