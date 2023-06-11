# Source:PC world, URL:https://www.pcworld.com/index.rss, language:en-US

## The best virtual machine tools for Windows: Run a PC inside your PC
 - [https://www.pcworld.com/article/1936055/the-best-virtualization-tools-for-windows.html](https://www.pcworld.com/article/1936055/the-best-virtualization-tools-for-windows.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-06-10 13:00:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>Windows users have several virtualization platforms at their disposal, allowing them to run simulated (or virtualized) systems within a single PC, each acting as a completely independent PC environment: Microsoft Hyper-V, which is part of Windows 10/11 Pro and Enterprise, as well as Oracle VirtualBox, VMware Workstation Pro, and Workstation Player. As Qemu is aimed at Linux systems, we&rsquo;ll leave it out of this list. The virtualization programs presented below all function as runtime environments under Windows and create one or more virtual machines as hypervisors on the main PC, emulating a complete computer with all relevant hardware components.</p>



<p>You&rsquo;ll find that Windows virtualizers differ significantly in terms of orientation, features, operation, and costs. This can actually be a good thing as it means that pretty much all programs are continually patched in order to keep up-to-date with the latest versions of operating systems such as Windows, Linux, or MacOS.</p>



<p><em>This article was translated from German to English, and originally appeared on pcwelt.de.</em></p>



<h2 class="toc" id="oracle-virtualbox-7-x">Oracle VirtualBox 7.x</h2>



<p>Due to its extensive features and good user guidance, the open-source software VirtualBox is a great option for private users, freelancers, and even companies. VirtualBox is also the only truly cross-platform virtualizer, which is offered free of charge for Windows, Linux, and Mac OS with an almost identical scope of services.</p>



<p>Since version 7, VirtualBox significantly revised its interface with improved menus and buttons making it easier to use. In addition, window contents are easier to recognize on high-resolution monitors. Further optimizations concern 3D graphics support when using Windows and Linux as guest systems as well as surround speaker systems. VirtualBox&rsquo;s file manager allows you to look into a guest computer&rsquo;s file system and conveniently copy files and folders between the host and guest PC.</p>



<p>VirtualBox supports 32- and 64-bit computers as both host and guest, as well as utilizing USB 2.0 and USB 3.0 ports, allowing you to mount USB drives as virtual data storage and encrypted hard disk images. The special features of SSD drives as storage for virtual PCs are also taken into account. Bidirectional drag-and-drop from and to the guest system is available for machines with Windows and Linux. </p>



<p>The software&rsquo;s wizard for creating new machines is particularly easy to use&mdash;you can directly select the medium for booting PCs. When setting up, you have the options of Windows 3.1, 95/98/ME, NT 4, 2000, XP, Vista, Windows 7, 8, 10 and 11, Linux distributions from kernel 2.4, Mac OS X, and Open BSD as guest systems. The settings for virtual PCs are saved as an XML file and can be easily exported and adapted as required or used for new PCs.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="VirtualBOX" class="wp-image-1940746" height="583" src="https://b2c-contenthub.com/wp-content/uploads/2023/06/VirtualBox.png" width="1016" /><figcaption><p>Hardware as desired: A virtual machine set up in VirtualBox can be reconfigured at any time, for example, for more RAM or an additional hard disk as data storage.</p> </figcaption></figure><p class="imageCredit">Sam Singleton</p></div>



<p>VirtualBox also offers a useful snapshot function that allows you to freeze the current state of a virtual machine. This allows you to undo all subsequent changes later and reset the virtual machine to its current state. Furthermore, VirtualBox recognizes most of the USB hardware connected to the real PC and can also make it available to the virtual PC if desired.</p>



<p>Thanks to VirtualBox&rsquo;s shared folders, data can be exchanged between the main and guest PCs, and via seamless mode the user can freely place the window of a guest system on the desktop of the main computer (host). And the exchange of finished machines between hosts with different operating systems works reliably.</p>



<h2 class="toc" id="vmware-workstation-player-17">VMware Workstation Player 17</h2>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Ein neuer virtueller PC kann im Vmware Workstation Player auf Basis einer Setup-DVD oder &uuml;ber ein ISO-Image eingerichtet werden." class="wp-image-1667321" height="884" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/vm-im-vmwareplayer-einrichten.png?w=1200" width="1200" /><figcaption><p>A new virtual PC can be set up in VMware Workstation Player via a setup DVD or with an ISO image.</p> </figcaption></figure><p class="imageCredit">IDG</p></div>



<p><a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://store-us.vmware.com/workstation_buy_dual#GS&amp;xcust=2-1-1936055-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">VMware Workstation Player</a> is the consumer version of VMware&rsquo;s professional virtualization software. Priced at $149, it&rsquo;s $50 less than the Pro version, and as you&rsquo;d expect, lacks some of Pro&rsquo;s functionality&mdash;it also lacks some of the features of VirtualBox. The Workstation Player can open set-up machines and create new virtual PCs. The software supports almost all Windows versions and many Linux variants, but is limited to a few settings for newly created virtual PCs. New in version 17 are updated system profiles for Windows 11, Windows Server, and current Linux kernels.</p>



<p>The biggest limitation compared to VirtualBox and Workstation Pro (below) is the lack of snapshots, which can be used to save the state of a virtual PC in order to access it again later. As a workaround, virtual hard disks can be saved to another drive. However, anyone who wants to repeatedly record intermediate states probably won&rsquo;t find the player adequate. Workstation Player also lacks the management and remote control functions for virtual computers via the network from VMware Workstation Pro.</p>



<p>The quick installation method for creating virtual machines with current Windows and Linux operating systems is practical and takes just a few clicks. In the player window, go to <em>Create a New Virtual Machine</em> on the right and select an ISO file as the installation source. The player analyzes the file, usually recognizes the operating system used, and takes care of entering default settings such as the user name.</p>



<h2 class="toc" id="vmware-workstation-pro-17">VMware Workstation Pro 17</h2>



<p><a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.vmware.com/products/workstation-pro.html&amp;xcust=2-1-1936055-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">VMware Workstation Pro</a>, which costs around $199, is the big brother of VMware Player. The software surpasses VirtualBox and the Player variant in terms of features, settings options, hardware support, saving and managing snapshots, copying and cloning virtual machines, and network configuration. For most virtualization tasks on private PCs, Workstation Pro, which is tailored to corporate users, seems unnecessary due to the sheer number of settings and menu functions that will probably never be used. </p>



<p>VMware Workstation Pro creates a networked virtual platform in which other operating systems are set up as guest systems and run in windowed mode or full-screen. The snapshot manager is absolutely first-class. It can freeze intermediate states of a virtual computer, nest them, and later return to the desired state. In conjunction with the powerful cloning of machines and the extended option of saving storage space with linked copies (a kind of incremental backup), various application scenarios can be created from a single system at the touch of a button. This is helpful for extensive experimentation with software, for example.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="VVmware Workstation Pro gl&auml;nzt mit einer umfassenden Hardwareunterst&uuml;tzung, einem durchdachten Einrichtungsassistenten und vielf&auml;ltigen Einstellm&ouml;glichkeiten beim Anlegen neuer Maschinen." class="wp-image-1660912" height="525" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/5-6.jpg?quality=50&amp;strip=all" width="934" /><figcaption><p>VMware Workstation Pro shines with comprehensive hardware support, a well thought-out setup wizard, and a wide range of setting options when creating new machines.</p> </figcaption></figure><p class="imageCredit">IDG</p></div>



<p>Major innovations in version 17 include support for Windows 11 host systems and Windows 11 guest systems with TPM and vTPM. On Linux and Windows virtual machines, VMware Workstation Pro now supports graphics rendering via OpenGL 4.3, and you can configure local virtual machines to start automatically when the host machine boots.</p>



<p>From Workstation Pro, virtual machines can be shared with other users and made available for joint use in the network, which primarily benefits business users. For this purpose, VMware also offers the administration environment Vsphere, in which systems can be stored centrally.</p>



<p>VMware Workstation Pro has some solid security features as well. Virtual hard disks can be encrypted with 256-bit AES crypto algorithms to protect against unauthorized access and PC settings can be password-protected against changes. The Workstation Pro version supports the exchange of virtual hard disks between different PCs and in the network as well as via the OVA/OVF format. As with VirtualBox, remote access to virtual systems is possible, whereby VMware Player relies on the free VNC protocol.</p>



<h2 class="toc" id="microsoft-hyper-v">Microsoft Hyper-V</h2>



<p>With the on-board function Hyper-V, you can create virtual machines in Windows 10 and 11, provided you use the Pro or Enterprise version (64 bit) as host. Hyper-V must be installed separately as an additional function under: Click the Windows button at the bottom left of your screen, select <em>Programs and Features &gt; Turn Windows Features on or off</em>, and select <em>Hyper-V</em> in the menu, and click <em>OK</em>.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Hyper-V" class="wp-image-1940760" height="370" src="https://b2c-contenthub.com/wp-content/uploads/2023/06/enable_role_upd.png" width="417" /><figcaption><p>Hyper-V from Microsoft is part of Windows 10 and 11 Pro and Enterprise, but must be installed separately in the Control Panel.</p> </figcaption></figure><p class="imageCredit">Windows</p></div>



<p>Hyper-V is optimized for Windows as a guest system and has a minimalist user interface called Hyper-V Manager. The program dispenses with technical wizards and hand-holding in favor of straightforward handling that might take some getting used to. Microsoft has limited the range of possible operating systems to Windows XP and higher. As far as Linux distributions are concerned, Hyper-V officially supports only Suse Linux Enterprise Server, Red Hat Enterprise Linux, and Cent OS&mdash;although some other distributions can be set up as virtual guest systems.</p>



<p>The advantage of Hyper-V over the virtualization platforms from Oracle and VMware is the dynamic memory management. When a virtual PC is started, the allocated working memory is not immediately occupied in one piece, but only enough of the real working memory is used as the virtual PC actually needs. In this way, several VMs can run in parallel without any noticeable drop in performance.</p>



<div class="wp-block-idg-base-theme-box-text inline-box">
<h2 id="comparison-hyper-v-and-virtualbox">Comparison: Hyper-V and VirtualBox</h2>



<p>Oracle VirtualBox as well as VMware Workstation Pro and Player are virtualizers tailored to desktop PCs, while Hyper-V comes from the server area of Microsoft. Accordingly, some functions that are useful on the desktop and found with VirtualBox and VMware Workstation Pro are missing, such as support for sound and access to USB devices. The exchange of files between the desktop of the main computer and a virtual PC is also missing, as is a shared clipboard for transferring data.</p>



<p>Some older operating systems cannot cope with the hardware emulated by Hyper-V because the corresponding drivers are missing. Windows from Vista onwards and newer Linux packages come with the appropriate system and graphics card drivers for the Hyper-V environment. With older Linux distributions it is advisable to look for a newer distribution version if necessary.</p>
</div>



<h2 class="toc" id="hardware-emulation">Hardware emulation</h2>



<p>The computers emulated by VirtualBox, VMware, and Hyper-V use older hardware. This is to ensure the best possible compatibility of virtual hardware and guest operating system. Guest extensions for Oracle and VMware&rsquo;s software allow the guest operating system to be optimized for the hardware and to work together with the main operating system. You&rsquo;ll first need to install the supplied add-ons for the smooth switching of the mouse pointer between the main operating system and the virtual machine. However, in Hyper-V, no such driver package is available.</p>



<h2 class="toc" id="virtual-pc-bios">Virtual PC BIOS</h2>



<p>Like a real computer, a virtual PC has its own BIOS that handles basic communication with the hardware for the guest operating system. When a machine is started, you can click the F12 key (VirtualBox) or the F2 key (VMware) to access the BIOS setup as with a real PC.</p>



<h2 class="toc" id="adapting-guest-pcs">Adapting guest PCs</h2>



<p>Virtual machines can be reconfigured in VirtualBox, VMware, and Hyper-V at any time, to increase or decrease the main memory provided and to add interfaces or further drives. As for the convenience of configuration changes, VMware Workstation Pro and VirtualBox are superior.</p>



<p>VirtualBox, VMware, and Hyper-V store the hard disks of the virtual computers in container files on the real hard disk. You specify the maximum size of the disk, which then grows dynamically. The file therefore only occupies approximately as much space as the guest system needs, including installed applications, data, and temporary files.</p>



<div class="wp-block-idg-base-theme-box-text inline-box">
<h2 id="moving-virtual-computers">Moving virtual computers</h2>



<p>VirtualBox, VMware, and Hyper-V store virtual hard disks in container files. For each system that&rsquo;s set up, there are also one or more configuration files and possibly backup files for snapshots. Normally, these files are located in a common folder. This makes it easy to move a system to another drive or to move it to another computer.</p>



<p>It&rsquo;s enough just to move the folder with all the files to the destination drive. To move the virtual machine, copy the folder to an external hard drive, for example, and then on to the hard drive or SSD on the destination PC.</p>



<p>On the target PC, start the virtualization software you are using and open the configuration file of the VPC via the corresponding menu command&mdash;for example, <em>File &gt; Open</em> for VMware Workstation Pro and <em>Player &gt; File &gt; Open</em> for Player. In VirtualBox, select <em>File &gt; Export Appliance</em> on the source PC and then <em>File &gt; Import Appliance</em> on the target PC.</p>
</div>



<h2 class="toc" id="conclusion-from-all-rounder-to-professional">Conclusion: From all-rounder to professional</h2>



<p>With its intuitive user guidance, the free software VirtualBox 7.x from Oracle is the best all-rounder for private users. The program combines good features with intuitive use. </p>



<p>The VMware Workstation Player is particularly recommended if you want to use ready-made virtual PCs in VMware format. The player is also extremely reliable in combination with the Vcenter Converter from VMware. </p>



<p>The VMware Workstation Pro shines with broad hardware support, a network editor, group functions, and many extras that are especially interesting for corporate users. But it&rsquo;s likely too much for private users.</p>



<p>Those who are willing to accept a significant reduction in ease-of-use and only want to set up virtual computers with Windows should try the Hyper-V that comes integrated in Windows 10 and 11 Pro and Enterprise.</p>

Windows</div>

## These JBL true wireless earbuds are just $60 for Father’s Day
 - [https://www.pcworld.com/article/1948541/these-jbl-true-wireless-earbuds-are-just-60-for-fathers-day.html](https://www.pcworld.com/article/1948541/these-jbl-true-wireless-earbuds-are-just-60-for-fathers-day.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-06-10 08:00:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>Your dad loves music, but he has a hard time keeping it to himself. Help Dad get into the 21st century by getting him a set of true wireless earbuds this Father&rsquo;s Day. You don&rsquo;t have to break the bank because now through June 11, you can get the <a href="https://shop.pcworld.com/sales/jbl-live-free-nc-true-wireless-in-ear-noise-cancelling-bluetooth-headphones?utm_source=pcworld.com&amp;utm_medium=referral&amp;utm_campaign=jbl-live-free-nc-true-wireless-in-ear-noise-cancelling-bluetooth-headphones&amp;utm_term=scsf-572639&amp;utm_content=a0x1P000004IlsIQAS&amp;scsonar=1" rel="noreferrer noopener" target="_blank">JBL Live Free NC+ True Wireless in-Ear Noise-Canceling Bluetooth Earbuds</a> for 60% off. Just make sure to order by June 6 to get them in time for Father&rsquo;s Day.&nbsp;</p>



<p>These true wireless earbuds offer JBL Signature Sound in a completely wireless and feature-rich package. The earbuds have Active Noise Cancelling, as well as TalkThru and Ambient Aware modes so Dad can switch between being fully immersed in his music and being aware of his surroundings.</p>



<p>With the included charging case, Dad can listen for up to 21 hours and get a quick recharge on the go. They&rsquo;re suitable for wearing while working out and offer a Voice Assistant and intuitive touch controls to take and make calls, change the track, adjust the volume, and more.</p>



<p>This Father&rsquo;s Day, get Dad a tech gift everyone could use. Now through June 11, the <a href="https://shop.pcworld.com/sales/jbl-live-free-nc-true-wireless-in-ear-noise-cancelling-bluetooth-headphones?utm_source=pcworld.com&amp;utm_medium=referral&amp;utm_campaign=jbl-live-free-nc-true-wireless-in-ear-noise-cancelling-bluetooth-headphones&amp;utm_term=scsf-572639&amp;utm_content=a0x1P000004IlsIQAS&amp;scsonar=1" rel="noreferrer noopener" target="_blank">JBL Live Free NC+ True Wireless in-Ear Noise-Canceling Bluetooth Earbuds</a> are 60% off $149 at just $59.97.</p>



<p><a href="https://shop.pcworld.com/sales/jbl-live-free-nc-true-wireless-in-ear-noise-cancelling-bluetooth-headphones?utm_source=pcworld.com&amp;utm_medium=referral-cta&amp;utm_campaign=jbl-live-free-nc-true-wireless-in-ear-noise-cancelling-bluetooth-headphones&amp;utm_term=scsf-572639&amp;utm_content=a0x1P000004IlsIQAS&amp;scsonar=1" rel="noreferrer noopener" target="_blank">&nbsp;</a></p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image"><img alt="" src="https://cdnp3.stackassets.com/653e06e5d5b08a6a90f1bf8badc6996c706ef03e/store/0d854f1c74a5aa2182f7f79ec75880b7944d0965c0cfba82cfb3f09b2c9b/sale_313088_primary_image.jpg" /></figure></div>



<p><strong>JBL Live Free NC+ True Wireless in-Ear Noise-Canceling Bluetooth Earbuds &ndash; $59.97</strong></p>



<p><a href="https://shop.pcworld.com/sales/jbl-live-free-nc-true-wireless-in-ear-noise-cancelling-bluetooth-headphones?utm_source=pcworld.com&amp;utm_medium=referral-cta&amp;utm_campaign=jbl-live-free-nc-true-wireless-in-ear-noise-cancelling-bluetooth-headphones&amp;utm_term=scsf-572639&amp;utm_content=a0x1P000004IlsIQAS&amp;scsonar=1" rel="noreferrer noopener" target="_blank">See Deal</a></p>



<p>Prices subject to change.</p>

Headphones</div>

