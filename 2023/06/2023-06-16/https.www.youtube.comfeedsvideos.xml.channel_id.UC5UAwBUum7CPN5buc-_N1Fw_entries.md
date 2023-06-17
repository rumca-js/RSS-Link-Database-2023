# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## NIX OS: the BEST package manager on the MOST SOLID Linux distribution
 - [https://www.youtube.com/watch?v=DMQWirkx5EY](https://www.youtube.com/watch?v=DMQWirkx5EY)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-06-16 15:31:14+00:00

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
Discord: https://discord.gg/XMuQrcYd

#nixos #linux #linuxdistro 

00:00 Intro
00:36 Sponsor: Kasm, the best remote desktop tool
01:22 What is NixOS?
04:20 Using the configuration file
08:58 Nix Package Manager
11:03 Updating and unstable channel
12:48 Nix is way more than that
14:53 Sponsor: get a PC made to run Linux
15:58 Support the channel

NixOS is a Linux distribution that is completely and entirely reproducible. Everything you use is defined in a configuration file that is used to build your system. All the services, packages, options, partition layout, hardware, everything, is in this config file.

If you're a developer, your eyes might be sparkling right now: that's right, one config file to exactly replicate your entire development environment.

You also can never get into dependency hell. Packages all declare exactly which versions of each library they need, and these versions are all installed side by side and kept, not erased by newer versions.


To create your configuration, there's a main configuration file in /etc/nixos, called configuration.nix.

This file uses its own specific syntax, that is entirely functional: it describes everything the system uses and with which options, from the hardware, the bootloader, the services, the packages, the apps, the users, everything.

This file is then used to build your operating system. Nix will read everything in there, and install, configure, and enable or disable everything, based on what the file contains. So, if you build a nixOS system with the same config file as someone else, you'll get exactly the same system.

Once you rebuild your system, there are now multiple entries in the boot loader: one for the new build, and one for the old one: you can always roll back to the previous configuration.

Of course, all of this requires root access to edit the main config of the system. But if you don't have root access, or if you don't want to add programs to your main reproducible config, but just test them out for now, you can also install packages as a regular user, using the nix package manager. Or you can add flatpak to your config file, or run appimages. But installing programs will be mainly done using the Nix package manager.

The Nix package manager works on any Linux distro, but also on macOS, WSL, and more. It's preverytty easy to use. If I want to install, for example, OBS, I'll just type

nix-env -iA nixos.obs-studio

The -i is the argument to install, and the capital A is to tell the package manager to install using the specific name of the package, instead of looking through the whole repo, which is way slower.

If I want to remove the package, I can use nix-env -e obs-studio, and it will be removed. Note that installing packages with nix-env doesn't add them to the config file.

NixOS works with channels. By default, you'll use the Stable channel, with tested packages that get security updates only, and major feature updates when there's a new release of NixOS, every 6 months.

To update, you can just run the command

sudo nix-channel --update

This will pull all the latest package versions from the channel your system uses.

Then you run the "nix-rebuild switch --upgrade" command, and your system will grab every new version of every package, and rebuild the system based on your configuration file.

Important to note, the new version of a package is installed alongside the old one. The new versions are the ones that will be used, thanks to a simple symbolic link system that always points to the newest version of a package, but you can rollback to an older one.

To get newer packages, at the risk of having a less stable system, you can switch to the unstable channel.

