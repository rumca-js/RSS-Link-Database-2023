# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## FLATPAK EXPLAINED: Theming, permissions, command line, browser installs...
 - [https://www.youtube.com/watch?v=IYXlgzrZRIE](https://www.youtube.com/watch?v=IYXlgzrZRIE)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-08-09T16:03:53+00:00

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
Discord: https://discord.gg/XMuQrcYd

#Flatpak #Linux #software 

00:00 Intro
00:33 Sponsor: Regain control of your network connection
01:31 Flatpak explained
03:30 Installing and setting up Flatpak
04:57 Theming Flatpak applications
08:41 Managing Permissions
10:43 Installing from the browser
11:21 Command Line basics
13:54 Sponsor: Get a PC that was made to run Linux
14:52 Support the channel

Flatpak is a method of packaging applications for ALL linux distros with one single package. 
Flatpaks mostly don't use your shared libraries, they ship their own.

Flatpak also brings better security with a sandbox that doesn't let the app access all your system when it doesn't need to, and a permissions system.

Flatpak also uses repositories, called remotes, the biggest one is of course Flathub.

So, most distros out there should have flatpak preinstalled, but if you run Ubuntu or an official Ubuntu flavor, Debian, or Arch, you might want to install it yourself.

On Ubuntu or Debian:
sudo apt install flatpak

For any distro:
https://flathub.org/setup

But this only gives you command line access to flatpak. If you're a more graphical sort of person, you might want to add support for your app store:

FOr GNOME software, the package is often called gnome-software-plugin-flatpak, and for Discover on KDE, it's generally plasma-discover-flatpak.

Next, you'll need to add a repo to be able to install flatpaks easily, without downloading a file manually each time. The biggest one everyone should use is FLathub, it has virtually every flatpak ever made.

sudo flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo

THEMING:

There are a bunch of themes available on Flathub, that you can find typing

flatpak search theme

If the theme you use is in there, you can just install it from here, then, you select it in GNOME Tweaks, and you run:

flatpak update

If your theme isn't available from Flathub, though, you'll need to tell flatpak it needs to use your specific theme. To do this, you can either run a command, or use a graphical application.

sudo flatpak override --env=GTK_THEME=NAME OF YOUR THEME.

But that's not enough, we also need to give flatpak access to the directory where your themes are located, namely the .themes directory:

sudo flatpak override --filesystem=$HOME/.themes

For GTK4/Libadwaita apps, open your .bash-profile file in your home directory. At the end, add this line:

export GTK_THEME=NAMEOFYOURTHEME

Save the file, and then log out and log back in for all the changes we made to be applied. All your GTK apps should now use the right theme, whether they're using libadwaita, flatpak, or both.

PERMISSIONS

Now let's see how you can change permissions. To manage them, you can use Flatseal on GNOME and KDE, but KDE also has a permissions page in the settings.

Generally, permissions are correctly set, but if you feel an app shouldn't have access to something, you can toggle that thing off, and if you feel an app SHOULD have access to something, you can toggle it ON.

BROWSER INSTALL

Installing flatpaks is just a one click operation from your graphical app store, but if you like to browse for apps in your web browser, you can also start an install straight from there.

There's an extension for Firefox and CHromium based browsers called Flatline. 

https://addons.mozilla.org/en-US/firefox/addon/flatline-flatpak/?ref=itsfoss.com

https://chrome.google.com/webstore/detail/flatline/cpbniogoilfagmcoipghkgnpmdglfmjm

COMMAND LINE BASICS:

install:  flatpak install APPNAME

Uninstall: flatpak remove APPNAME

Update: flatpak update

Cleanup: flatpak uninstall --unused

List installed flatpaks: flatpak list

Search for flatpaks: flatpak search

Run an app: flatpak run COMPLETE_APPNAME

Kill an app: flatpak kill COMPLETE_APPNAME

Repair: flatpak repair

