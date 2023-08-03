# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## Access your PCs from ANYWHERE with REMOTE DESKTOPS (Linux, Mac, and Windows)
 - [https://www.youtube.com/watch?v=hjnsVpodkUM](https://www.youtube.com/watch?v=hjnsVpodkUM)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-08-02T15:54:44+00:00

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

#remotedesktop #vnc #rdp 

How does a remote desktop work? Essentially, it mirrors the contents of one PC onto the display of another PC, either through a dedicated app, a web browser, or the native capabilities of your operating system. There are two primary protocols: RDP, or Remote Desktop Protocol, and VNC, or Virtual Network Computing.

Let's start with KasmVNC. It's open source, free of charge, and you can download the server component from their GitHub page. It's packaged for various Linux distributions including Alpine Linux, Debian, Ubuntu, Fedora, OpenSUSE, Kali Linux, or Oracle Linux, all for ARM or x86 CPUs. It doesn’t have a server component for Windows or macOS though, so it’s Linux only.

Once the server component is installed on the PC you want to remote into, you'll need to use the command line. Simply run 'vncserver', and you'll be prompted to create a user that you’ll use to login to your remote desktop.

Then, add your user to the ssl-cert group with the command displayed in your terminal.

Then go to your client PC, open a web browser, type the IP address of the server followed by the port number indicated when you ran the 'vncserver' command.

You'll be asked to enter your login and password for the user you created, then you're in. You'll get a nice sidebar with options to tailor performance, frame rate, compression, and more. And if you want to really get into the details, there’s a YAML configuration file you can edit either in /etc/kasmvnc, or you can have your own config file for your user in .vnc.

If you want to remote into a Linux PC, most desktop environments have settings that let you enable remote desktop. In GNOME, for example, you go to the sharing page, then 'remote desktop', and enable remote control. KDE has the 'krfb' app that allows you to share your desktop.
On the client side, all you need is either an RDP or VNC client. The 'Connections' app in GNOME and 'KRDC' in KDE are probably the best integrated apps, or you can use 'Remmina'.

"If you want to remote into a Windows PC, your best bet is the in-built Remote Desktop Protocol or RDP. To enable it on Windows 11 Pro (home doesn't support it), simply open the Settings app, click 'System', then 'Remote Desktop', and toggle it on. A pop-up will ask for confirmation, just click 'Confirm', and voila - you're done with the server-side setup.

On the client, you'll need an RDP client. For Windows, macOS, iOS, and Android, you have Microsoft's Remote Desktop app. And for Linux users, there's Remmina - a free, open source tool available on any distro through Flathub.

If your server is a Mac, the process is quite similar. First, open System Settings, navigate to General, and then to the 'Sharing' page. Here, enable 'Remote Management'.

Next up, you need a VNC client on the client PC. Just input the IP address and the username of your Mac's user. However, one thing to keep in mind is that performance can vary. Since the resolution on Macs can be quite high, you might find it's not as fast as you'd like.

Some virtual machine clients can let you remote into a VM, for example, in Virtualbox, you have a remote display tab in the “display settings” of your VM. Now to make sure this works, you’ll need to install the Virtualbox Extension pack, which you can download for free from Virtualbox’s website.

https://download.virtualbox.org/virtualbox/7.0.8/Oracle_VM_VirtualBox_Extension_Pack-7.0.8.vbox-extpack

Then, in Virtualbox, you can click the tools tab, the the little list button, and then extensions. Here, click install, then select the extension pack, and you’re done. Now you can enable remote display in the VML’s Display settings.

