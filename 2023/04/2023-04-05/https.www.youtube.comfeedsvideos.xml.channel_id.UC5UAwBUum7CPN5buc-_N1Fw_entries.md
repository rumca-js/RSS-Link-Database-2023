# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## The BEST PDF TOOLS for Linux: merge, edit, create, annotate, OCR...
 - [https://www.youtube.com/watch?v=ie7Jb1KiIBM](https://www.youtube.com/watch?v=ie7Jb1KiIBM)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2023-04-05 16:04:12+00:00

Try KasmVNC, the smoothest remote desktop out there: https://www.kasmweb.com/kasmvnc

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
Twitter : http://twitter.com/thelinuxEXP
PeerTube: https://tilvids.com/c/thelinuxexperiment_channel/videos

This video is distributed under the Creative Commons Share Alike license.

#pdfeditor #linux #pdf 

00:00 Intro
00:26 KasmVNC: the best remote desktop option on Linux
01:21 The Default tools kinda suck
02:22 Editing a PDF
05:14 Manual Signature of a PDF
06:47 Digitally Signing a PDF
08:49 Optical Character Recognition of a PDF
10:17 Hand Written Annotations on a PDF
11:08 Modifying pages and merging PDFs
11:53 Creating a PDF
13:05 Parting thoughts
13:39 Sponsor: Get a PC designed to run Linux with Tuxedo
14:29 Support the channel

How to edit a PDF document:

One tool that is probably already on your Linux desktop is LibreOffice Draw. It can open PDF documents, and edit them, as long as it's not an image.

If you're familiar with vector drawing programs, then Inkscape can also edit PDF documents. For more robust solutions, you have proprietary commercial solutions, including PDF Studio, Master PDF, Foxit PDF Editor, or WPS Office, but you'll have to pay for them.

How to manually sign a PDF:

Okular can actually do that. You can use the manual drawing tool to write your signature, or you can add the ability to paste an image on top of a document, but it's convoluted. You have to go to settings, toolbars shown, enable the quick annotations toolbar, then click the "configure button", click "Add", select the type "Stamp", and click the little button next to the "stamp symbol" field, to pick your own hand drawn signature that you previously saved as an image. Afterwards, you can just add that to any document in one click from that quick annotations toolbar.

You can also open the PDF document in LibreOffice Draw or the GIMP, and add your image signature this way.


How to digitally sign a PDF:

The easiest way is to use LibreOffice. Open the LibreOffice suite, click File, then digital signatures, and then "sign existing PDF", then the "sign document" button at the top. It will list all the available existing signatures and certificates you have installed on your device, and you can pick the one you want.

By default, LibreOffice will look into Mozilla Firefox's certificates list, so you'll have to put your certificate file there. To do so, open FIrefox, then the main menu, Preferences, Privacy and Security, and then "View Certificates". Then click on "authorities" and "Import", and then the "OK" button, and you're done.

Optical Character Recognition (OCR)!

A simple option is GImageReader, an open source app that will let you import a document or image, and will recognize all the text inside, in a very large variety of languages. It can take a while to do its thing, but it works reliably, and it was able to extract text from scanned PDFs and images like a PNG.

If you prefer doing these tasks from the command line, then you have Tesseract OCR, which is actually what GImageReader uses in the background.

How to annotate a PDF:

Your best option is probably Xournal++. It lets you open PDF documents, and draw all over them. You can highlight text, add hand drawn notes, shapes, type some text. It can even handle equations and graphs, and has a very customizable interface.

How to modify pages, split and merge PDF documents:

If all you need is modifying the pages in a PDF document, like reordering them, or deleting them, then you have PDF Arranger, a simple GNOME app that will run on any Linux desktop, and is available on Flathub.

