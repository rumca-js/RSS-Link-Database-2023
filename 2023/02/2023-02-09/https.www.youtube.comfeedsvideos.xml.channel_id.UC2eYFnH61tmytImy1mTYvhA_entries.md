# Source:Luke Smith - YouTube, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC2eYFnH61tmytImy1mTYvhA, language:en-US

## Install Artix or Arch Linux (Encrypted system)
 - [https://www.youtube.com/watch?v=dI3bGeT31Bo](https://www.youtube.com/watch?v=dI3bGeT31Bo)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC2eYFnH61tmytImy1mTYvhA
 - date published: 2023-02-09 20:09:03+00:00

Here's how you set up Artix and Arch Linux with an encrypted root/home drive. I cover not just encryption, but installation for legacy BIOS and UEFI machines, but also what differences you'll encounter on Artix's different init systems. I also talk about automatic logons and such.

https://artixlinux.org/
https://wiki.artixlinux.org/Main/Installation
https://archlinux.org/
https://wiki.archlinux.org/title/Installation_guide

Note that the only thing different between Arch and Artix are renamed commands (pacstrap vs. basestrap and genfstab vs. fstabgen and artix-chroot vs. arch-chroot). Artix can come with either runit, openrc, s6 or dinit as an init system and setup for all is the same except for the desired package is installed initially as is the command to enable the network interface.

If you want to lazily copy, the programs I installed with basestrap were:
base base-devel runit elogind-runit linux linux-firmware grub networkmanager networkmanager-runit cryptsetup lvm2 lvm2-runit neovim vim

00:00 Intro and Background
01:26 Download and Create and ISO
05:05 On the Artix and Arch Install Scripts in the Repositories
07:28 Reboot and Boot from the ISO
08:26 UEFI vs Legacy Boot
09:38 Formatting the Drive and Partitions
14:34 Making an Encrypted Partition (luksFormat)
17:37 Mount Partitions
18:24 Choosing Mirrors for Speed (Optional)
19:02 Install the Operating System and Programs
22:06 Chrooting into the New Operating System
23:03 Settings: Timezone, locale, LANG, hostname
26:13 Enable NetworkManager and internet/wifi
27:17 Passwords and users (optional autologin)
29:30 Preparing decryption on boot, mkinitcpio.conf
30:59 Grub configuration with UUIDs to decrypt
32:08 Generating an fstab file
32:28 Finishing up the GRUB configuration
36:32 Grub installation and grub-mkconfig
39:13 Finalizing
39:47 Checking our work
41:44 On graphical environments
42:30 LARBS
45:45 On xinit and starting desktop environments or window managers

My website: https://lukesmith.xyz
Classical books reprinted by me: https://lindypress.net
Get all my videos off YouTube: https://videos.lukesmith.xyz
or Odysee: https://odysee.com/$/invite/@Luke:7

Please donate: https://donate.lukesmith.xyz
BTC: bc1qd20r7phdct3t0e0z6jqs55ulectg25pngt7hyl
XMR: 89yML3AtqnTNdo3wNuoaW44D94Zx1kBZNSBc9SyNxGdaKEZwZNdVzvy9zpbzJMzysiWZEU3b5LwjQ3XwWuQsknCF8JK73yv

OR affiliate links to things l use:
https://www.vultr.com/?ref=8384069-6G Get a VPS and host a website or server for anything else.
https://www.epik.com/?affid=we2ro7sa6 Get a cheap and reliable domain name with Epik.

