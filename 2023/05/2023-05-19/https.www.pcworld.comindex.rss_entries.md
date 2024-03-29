# Source:PC world, URL:https://www.pcworld.com/index.rss, language:en-US

## An exploit can reveal your KeePass master password in plaintext
 - [https://www.pcworld.com/article/1923963/an-exploit-can-reveal-your-keepass-master-password-in-plaintext.html](https://www.pcworld.com/article/1923963/an-exploit-can-reveal-your-keepass-master-password-in-plaintext.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-05-19 21:13:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p><a href="https://www.pcworld.com/article/1668328/keepass-password-manager-review.html">KeePass password manager</a> users may want to be extra vigilant for the next several weeks or so. A <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-32784&amp;xcust=2-1-1923963-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">newly discovered vulnerability</a> allows retrieval of of the master password in plaintext, even when the database is locked or the program is closed. And while a fix is in the works, it won&rsquo;t arrive until early June at the soonest.</p>



<p>As reported by <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.bleepingcomputer.com/news/security/keepass-exploit-helps-retrieve-cleartext-master-password-fix-coming-soon/&amp;xcust=2-1-1923963-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Bleeping Computer</a> (which covers the issue in full technical detail), a security researcher known as vdohney published a proof-of-concept tool that demonstrated the exploit in action. An attacker can perform a memory dump to gather most of the master password in plaintext, even when a KeePass database is closed, the program is locked, or the program is no longer open. When pulled out of the memory, the first one or two characters of the password will be missing, but can then be guessed to figure out the entire string.</p>



<p>For those unfamiliar with memory dumping vulnerabilities, you can think of this scenario a bit like KeePass&rsquo;s master password as loose change in a pants pocket. Shake out the pants and you get nearly the whole dollar (so to speak) needed to buy entry into the database&mdash;but those coins shouldn&rsquo;t be floating around in that pocket to begin with.</p>



<p>The proof-of-concept tool demonstrates this issue in Windows, but Linux and macOS are believed to be vulnerable, too, as the problem exists within in KeePass, not the operating system. Standard user accounts in Windows aren&rsquo;t safe, either&mdash;dumping the memory does not require administrative privileges. To execute the exploit, a malicious actor would need either access to the computer remotely (gained through malware) or physically.&nbsp;</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="" class="wp-image-1923969" height="498" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/image-6.png" width="1024" /><figcaption>KeePass comes in two editions, 2.x and 1.x. They are both still maintained, though 2.x is the newer edition with  more available features.</figcaption></figure></div>



<p>All existing versions of KeePass 2.x (e.g., 2.53.1) are affected. Meanwhile, KeePass 1.x (an older edition of the program that&rsquo;s still being maintained), KeePassXC, and Strongbox, which are other password managers compatible with KeePass database files, are not affected according to vdohney.</p>



<p>A fix for this vulnerability will come in KeePass version 2.54, which is likely to launch in early June. Dominick Reichl, the developer of KeePass, gave this estimate in a <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://sourceforge.net/p/keepass/discussion/329220/thread/f3438e6283/?limit=25#8a4a&amp;xcust=2-1-1923963-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">sourceforge forum</a> along with the caveat that the timeframe is not guaranteed. An <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://keepass.info/filepool/KeePass_230507.zip&amp;xcust=2-1-1923963-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">unstable test version of KeePass</a> with the security mitigations is available now. Bleeping Computer reports that the creator of the proof-of-concept exploit tool cannot reproduce the issue with the fixes in place.</p>



<p>However, even after upgrading to the fixed version of KeePass, the master password may still be viewable in the program&rsquo;s memory files. To fully protect against that, you&rsquo;ll have to wipe your PC completely using the mode that overwrites existing data, then freshly reinstall the operating system.</p>



		<div class="wp-block-product-widget-block product-widget is-half-width is-float-right">
			<div class="product-widget__block-title-wrapper">
				<h4 class="product-widget__block-title" id="our-top-antivirus-pick">
					Our top Antivirus pick				</h4>
			</div>

			<div class="product-widget__content-wrapper">
									<div class="product-widget__title-wrapper">
						<h3 class="product-widget__title" id="norton-360-deluxe">Norton 360 Deluxe</h3>
					</div>
				
									<div class="product-widget__image-outer-wrapper">
						<div class="product-widget__image-wrapper">
							<img alt="Norton 360 Deluxe" class="product-widget__image" height="864" src="https://b2c-contenthub.com/wp-content/uploads/2022/04/norton.png" width="1536" />
						</div>
					</div>
				
									<div class="review product-widget__review-details">
						<img alt="Editors' Choice" class="product-widget__review-details--editors-choice-logo" src="https://www.pcworld.com/wp-content/uploads/2021/09/PC-ED-CHOICE.png" />							<div class="product-widget__rating-and-review-link">
								<div class="product-widget__review-details--rating">
											<div class="starRating"></div>
										</div>									<a class="product-widget__review-link" href="https://www.pcworld.com/article/393283/norton-360-deluxe-antivirus-review.html" target="_blank">Read our review</a>
									
							</div>
											</div>
				
				<div class="product-widget__information">
												<div class="product-widget__information--rrp-wrapper">
									<span class="product-widget__information--rrp-label">
																	</span>
									<span class="product-widget__information--rrp-value">
																		</span>
								</div>
								
											<div class="product-widget__pricing-details  ">
															<span class="product-widget__pricing-details--label">
									Best Prices Today:
								</span>
														<span class="product-widget__pricing-details--links-wrapper">
								<a class="product-widget__pricing-details--link" href="https://software.pcworld.com/p37061-norton_360_deluxe_2022_3-d_1-yr" rel="nofollow" target="_blank">$17.99 at  PCWorld Software Store</a>							</span>
						</div>
									</div>
			</div>
		</div>

		


<p>That&rsquo;s a pretty drastic move, however. More reasonably, don&rsquo;t let untrusted individuals access your computer, and don&rsquo;t click any unknown links or install any unknown software. A good antivirus program (like one of those <a href="https://www.pcworld.com/article/407277/best-antivirus-for-windows-pc.html">among our top recommendations</a>) helps, too. You can also reduce your exposure by restarting your PC, clearing your hibernation and swap files, and temporarily accessing your KeePass database in a safe alternative like KeePassXC instead. <a href="https://www.pcworld.com/article/549444/how-to-encrypt-files-in-windows.html">Device encryption</a> can also help against a physical attack on your PC (or if you think someone could mine this info after you donate or junk the PC). There are ways to stay protected&mdash;and fortunately, this appears to be only a proof-of-concept concern, rather than an active exploit.</p>

Internet, Security</div>

## How to upgrade to Windows 11: Every option explained
 - [https://www.pcworld.com/article/542194/how-to-upgrade-to-windows-11.html](https://www.pcworld.com/article/542194/how-to-upgrade-to-windows-11.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-05-19 18:00:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>Since Microsoft has said that Windows 10 won&rsquo;t receive any new features from now until it ends support in 2025, it&rsquo;s a good time to consider upgrading from Windows 10 to Windows 11. It&rsquo;s a free upgrade for your Windows 10 PC.</p>



<p>Downloading Windows 11 is very much like <a href="https://www.pcworld.com/article/394764/how-to-get-the-windows-11-beta.html">downloading the original Windows 11 beta</a>, but there&rsquo;s an additional tool that Microsoft has added to facilitate the process. In fact, there are four ways to download Windows 11, each with its own unique advantages. We&rsquo;ll show you all four, after explaining what you should know <em>before </em>upgrading.</p>



<p>You can always consult our <a href="https://www.pcworld.com/article/1471886/why-we-want-you-to-switch-to-windows-11-and-why-you-shouldnt.html">reasons to upgrade to Windows 11 (and reasons not to!)</a> if you&rsquo;re still on the fence and want to examine the question from all sides.</p>



<blockquote class="wp-block-quote"><p><em>Editor&rsquo;s Note: This story originally appeared on Oct. 11, 2021. We&rsquo;re updating the story now that Microsoft has said it would end new feature updates for Windows 10.</em></p></blockquote>



<h2 id="what-youll-need-to-download-windows-11">What you&rsquo;ll need to download Windows 11</h2>



<p>Before you begin downloading Windows 11, make sure you have the right PC hardware. While we don&rsquo;t think there&rsquo;s much risk to downloading and installing Windows 11 in general, there&rsquo;s always the outside possibility that something will go wrong. Take a moment and <a href="https://www.pcworld.com/article/407021/best-windows-backup-software.html">back up critical files</a> to an external hard drive or <a href="https://www.pcworld.com/article/407149/online-cloud-backup-services-carbonite-idrive-backblaze-livedrive.html">the cloud</a> before proceeding. Our <a href="https://www.pcworld.com/article/540165/the-windows-11-upgrade-checklist.html">Windows 11 upgrade checklist</a> can help you ensure all your ducks are in a row.</p>



		<div class="wp-block-product-widget-block product-widget is-half-width is-float-right">
			<div class="product-widget__block-title-wrapper">
				<h4 class="product-widget__block-title" id="our-favorite-windows-backup-software">
					our favorite windows backup software				</h4>
			</div>

			<div class="product-widget__content-wrapper">
									<div class="product-widget__title-wrapper">
						<h3 class="product-widget__title" id="r-drive-image-7">R-Drive Image 7</h3>
					</div>
				
									<div class="product-widget__image-outer-wrapper">
						<div class="product-widget__image-wrapper">
							<img alt="R-Drive Image 7" class="product-widget__image" height="1358" src="https://b2c-contenthub.com/wp-content/uploads/2022/01/r-drive-78.jpg?quality=50&amp;strip=all" width="1692" />
						</div>
					</div>
				
									<div class="review product-widget__review-details">
						<img alt="Editors' Choice" class="product-widget__review-details--editors-choice-logo" src="https://www.pcworld.com/wp-content/uploads/2021/09/PC-ED-CHOICE.png" />							<div class="product-widget__rating-and-review-link">
								<div class="product-widget__review-details--rating">
											<div class="starRating"></div>
										</div>									<a class="product-widget__review-link" href="https://www.pcworld.com/article/605046/r-drive-image-review.html" target="_blank">Read our review</a>
									
							</div>
											</div>
				
				<div class="product-widget__information">
												<div class="product-widget__information--rrp-wrapper">
									<span class="product-widget__information--rrp-label">
																	</span>
									<span class="product-widget__information--rrp-value">
																		</span>
								</div>
								
											<div class="product-widget__pricing-details  ">
															<span class="product-widget__pricing-details--label">
									Best Prices Today:
								</span>
														<span class="product-widget__pricing-details--links-wrapper">
								<a class="product-widget__pricing-details--link" href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.drive-image.com/&amp;xcust=2-3-542194-5-605618-17180&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">$44.95 at  R-tools Technology</a>							</span>
						</div>
									</div>
			</div>
		</div>

		


<p>Also make sure you understand that <a href="https://www.pcworld.com/article/394833/only-windows-11-pro-will-let-you-install-windows-11-with-a-local-account.html">Windows 11 Home will require a Microsoft account</a> to administer. If you own a Windows 10 Pro account and upgrade to Windows 11 Pro, you&rsquo;ll be able to use a local (or as Microsoft now calls it, &ldquo;offline&rdquo;) account. To upgrade to <a class="product-link" href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/product/B00ZSHDJ4O&amp;xcust=2-3-542194-1-389670-10994&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Windows 10 Pro</a> and then to Windows 11 Pro, the simplest way is to go to the Microsoft Store and upgrade to Windows 10 Pro before kicking off the upgrade. You&rsquo;ll pay full price going that route though; to save some cash, check out our guide on <a href="https://www.pcworld.com/article/397575/how-to-get-windows-cheap-or-even-for-free.html">how to get Windows for cheap (or maybe even free)</a>. You can also upgrade to Windows 11 Pro after first upgrading to from Windows 10 Home to Windows 11 Home, though you&rsquo;ll need to enter a Microsoft account to do so.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Windows Store upgrade to Windows 11 Pro or Windows 10 Pro" class="wp-image-542245" height="932" src="https://b2c-contenthub.com/wp-content/uploads/2021/10/Windows-10-or-11-Pro-upgrade.png?w=1200" width="1200" /><figcaption>There&rsquo;s no need to upgrade to Windows 10 Pro or Windows 11 Pro unless you love Windows Sandbox or local accounts.</figcaption></figure><p class="imageCredit">Mark Hachman / IDG</p></div>



<p>The time that downloading and installation of Windows 11 will require will vary, due to your PC&rsquo;s speed and your available broadband bandwidth. We&rsquo;d say that allocating 30 minutes to an hour sounds about right, but it may be very variable. Plan on having at least 9 GB of free space available to download Windows 11, and make sure your PC is up to date, with the latest version of Windows 10 installed. Simply run Windows Update on your computer before installing Windows 11 to make sure it&rsquo;s properly patched.</p>



<p>You&rsquo;ll need a PC that meets the<a href="https://www.pcworld.com/article/3622940/windows-11-system-hardware-requirements.html"> minimum hardware specifications of Windows 11</a>.  We would also very much encourage you to read our earlier story on the <a href="https://www.pcworld.com/article/3622940/windows-11-system-hardware-requirements.html">Windows 11 minimum hardware specifications</a>, download Microsoft&rsquo;s Health Check app, and check to see if your PC is eligible to upgrade to Windows 11. You&rsquo;ll need a PC with a least a TPM (Trusted Platform Module) 1.2 to qualify. The easiest and safest way to qualify for Windows 11 is simply to have a PC that meets Microsoft&rsquo;s restrictions.</p>



<p>If you own a PC with a TPM 1.2 but not a TPM 2.0 installed, there is <a href="https://www.pcworld.com/article/542121/microsoft-reveals-how-to-bypass-windows-11s-strict-hardware-requirements.html">an &ldquo;official&rdquo; way around the restrictions</a>. You&rsquo;ll need to open the Registry Editor, though, which is the foundation of your PC. Microsoft would like you to know that there are <em><a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://support.microsoft.com/en-us/windows/installing-windows-11-on-devices-that-don-t-meet-minimum-system-requirements-0b2dc4a2-5933-4ad4-9c09-ef0a331518f1&amp;xcust=2-3-542194-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">serious risks</a></em> to doing so, and recommends upgrading to Windows 11 on supported hardware via Windows Update (our first option, below) instead. To proceed using the Registry Editor and install Windows 11 on unsupported hardware, follow these steps. (If you&rsquo;re uncertain about what to do or don&rsquo;t want to risk your PC, don&rsquo;t do this!)</p>



<ul><li>In Windows 10, open the Registry Editor by tapping the Windows key and then entering &ldquo;Registry Editor&rdquo; or <strong>regedit</strong> in the search box.</li><li>Go to HKEY_LOCAL_MACHINE\SYSTEM\Setup\MoSetup. If the folder isn&rsquo;t there, right-click the Setup folder and create the MoSetup subfolder.</li><li>Within the MoSetup folder, right-click and select New &gt;DWORD (32-bit) Value</li><li>Name the new registry entry AllowUpgradesWithUnsupportedTPMOrCPU. Double-click it, then change the registry value to 1.</li></ul>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Windows 11 registry editor" class="wp-image-542246" height="751" src="https://b2c-contenthub.com/wp-content/uploads/2021/10/Windows-11-registry-editor.png?w=1200" width="1200" /><figcaption>The Registry Editor. If the required entry doesn&rsquo;t exist, you&rsquo;ll have to create it.</figcaption></figure><p class="imageCredit">Mark Hachman / IDG</p></div>



<p>This method allows your PC to bypass the check for TPM 2.0, as well as the required CPU family and model. You can also directly apply an image installation of Windows 11 to the disk, too. Doing this via the Microsoft DISM command-line tool will also bypass the TPM/CPU check, Microsoft says.</p>



<h2 id="windows-11-clean-install-vs-updating-in-place">Windows 11: Clean install vs. updating in-place</h2>



<p>Installing Windows 11 via Windows Update is an &ldquo;in-place&rdquo; or &ldquo;incremental&rdquo; installation, where the Windows 11 code is essentially added to a PC with existing apps and documents. It&rsquo;s a safe approach, provided you&rsquo;ve backed up your existing files. (Again: Back up your computer before upgrading your operating system!) Windows 11 should also allow you to &ldquo;roll back&rdquo; to Windows 10 within a period of time (typically 10 days) if you simply don&rsquo;t like it.</p>



<p>A &ldquo;clean install&rdquo; offers you the option of starting fresh, and typically that&rsquo;s what the other installation options below offer. In Windows 11&rsquo;s case, you should strongly consider this option. A clean install helps eliminate any bugs that may crop up.</p>



<p>A clean install typically means wiping your documents, apps, and settings from your PC and starting fresh. That&rsquo;s where the cloud helps. If your documents are stored on OneDrive (or in Box, Dropbox, an external drive, whatever) you&rsquo;ll be able to simply copy them back over. You&rsquo;ll need to download and re-install apps and games, however, as well as patch them. Take some care here&mdash;saved games might not be in the games directory, but inexplicably stored in the Documents folder instead.</p>



<p>Keep in mind that if you upgrade to Windows 11, let the 10-day grace period expire, and <em>then</em> decide to go back to Windows 10, you can&mdash;you&rsquo;ll just have to download and install a clean copy of Windows 10 instead. (If you own a valid Windows 10 or Windows 11 license, this is all free.)</p>



<p>You can always reset your PC&mdash;Windows 10 <em>or</em> Windows 11&mdash;at any time to make things tidy. Just make sure you have everything backed up.</p>



<p>Now that you know everything you need to know before upgrading, let&rsquo;s get to the nitty-gritty. There are four different ways you can install Windows 11.</p>



<h2 id="how-to-install-windows-11-via-windows-update">How to install Windows 11 via Windows Update</h2>



<p>Now that Microsoft has released Windows 11, there&rsquo;s no need to be part of the Windows Insider program, which was the original way to download the Windows 11 Insider beta.</p>



<p>At some point, you&rsquo;ll be asked to download Windows 11, via an option that looks something like the screen below. If you don&rsquo;t see this &ldquo;choice&rdquo; screen and &ldquo;check for updates&rdquo; doesn&rsquo;t offer Windows 11 to you, you can try our next suggestion below.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Windows 11 choice screen from Microsoft Windows 10" class="wp-image-539096" height="713" src="https://b2c-contenthub.com/wp-content/uploads/2021/09/Windows-11-choice-screen-from-Microsoft.png" width="999" /><figcaption>Simply click &ldquo;Download and install&rdquo; to begin downloading Windows 11.</figcaption></figure><p class="imageCredit">Mark Hachman / IDG</p></div>



<p>Downloading Windows 11 via Windows Update is the easiest way forward. You&rsquo;ll likely be asked for confirmation that you&rsquo;ve backed up critical apps and documents, then the installation will proceed.  </p>



<p>Some people prefer to upgrade to Windows 11, then later do a clean refresh of their PC. It might be overkill, but it&rsquo;s an option nevertheless.</p>



<h2 id="how-to-download-windows-11-via-the-windows-11-installation-assistant">How to download Windows 11 via the Windows 11 Installation Assistant</h2>



<p>The Windows 11 Installation Assistant and the Create Windows 11 Installation Media tool (described later) are quite similar: If you&rsquo;ve tried running Windows Update and Windows 11 isn&rsquo;t being offered to you, you can jumpstart the process via the Windows 11 Installation Assistant. If have more than one PC that you&rsquo;d like to upgrade, the Installation Media tool can be reused on multiple PCs.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Windows 11 Installation Assistant" class="wp-image-542247" height="861" src="https://b2c-contenthub.com/wp-content/uploads/2021/10/Windows-11-Installation-Assistant.png?w=1200" width="1200" /><figcaption>The opening screen of the Windows 11 Installation Assistant.</figcaption></figure><p class="imageCredit">Mark Hachman / IDG</p></div>



<p>Using the <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://go.microsoft.com/fwlink/?linkid=2171764&amp;xcust=2-3-542194-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Windows 11 Installation Assistant</a> (clicking the link will download the assistant) simply provides you with a way to download and install Windows 11 on a single PC. We haven&rsquo;t tested this method all the way through, but it appears that the Installation Assistant will download Windows 11 while you wait, instead of in the background as Windows Update does. There shouldn&rsquo;t be any substantive differences, though you may be simply stuck waiting for the process to complete.</p>



<h2 id="how-to-download-windows-11-via-the-create-windows-11-installation-media-tool">How to download Windows 11 via the Create Windows 11 Installation Media Tool</h2>



<p>The Create Windows 11 Installation Media Tool is perfect if you have to upgrade more than one Windows 10 PC in your home. The difference here is that you can use the tool to download to and burn a DVD, if your PC still has a DVD drive, or simply to a USB key. (Don&rsquo;t use an external hard drive for this, as the tool requires you to format, or erase, the entire drive first. Downloading an image ISO, the next option, solves that problem.)</p>



<p>For this, you&rsquo;ll need a DVD and DVD burner, <em>or</em> a USB key that&rsquo;s at least 8GB or more. You may need to use a dual-layer DVD. You can then tell Windows to download the file to the USB key, or as an ISO file for burning to the DVD. You&rsquo;ll be able to select the language, edition, and architecture (choose the 64-bit option) and then the procedure will begin.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Create Windows 11 Installation Media" class="wp-image-542248" height="1038" src="https://b2c-contenthub.com/wp-content/uploads/2021/10/Windows-11-Create-Windows-11-Installation-Media.png?w=1200" width="1200" /><figcaption>What you&rsquo;ll see as you install Windows 11 using the Create Windows 11 Installation Media tool.</figcaption></figure><p class="imageCredit">Mark Hachman / IDG</p></div>



<p>Once the media tool has been created, you&rsquo;ll either need to burn it to a DVD using your existing DVD burning tools, or you&rsquo;ll have a USB key with Windows 11 on it. To install Windows 11, you&rsquo;ll need to reboot your PC with the DVD or USB key installed. If everything goes according to plan, your PC should automatically begin installing Windows 11.</p>



<p>If it doesn&rsquo;t, you&rsquo;ll need to follow the instructions for entering your PC&rsquo;s BIOS or UEFI settings in its preboot environment. Consult your PC&rsquo;s documentation in how to do this. Typically, it requires you to press a key (such as the <strong>Esc</strong> or <strong>Delete</strong> key) immediately after tapping your PC&rsquo;s power button. You&rsquo;ll want to set your PC to either boot from a USB/DVD, or else simply check to see if it <em>can</em> boot from either drive before booting normally.</p>



<h2 id="how-to-download-windows-11-with-a-iso-disk-image">How to download Windows 11 with a ISO disk image</h2>



<p>This is my preferred way of installing a new OS, if I&rsquo;ve committed to upgrading the operating system. Downloading an .ISO file allows you to simply tuck it away like any other document on an external hard drive. If you&rsquo;d like, you can burn it to a DVD or save it on a USB key, too. With Windows 10 or Windows 11, though, you don&rsquo;t need to. Simply right-click the .ISO file, select &ldquo;Mount,&rdquo; and Windows will simply treat the file like a virtual DVD in a disc drive. You&rsquo;ll be able to kick off the installation process in one easy step.</p>



<p>You should treat an ISO file like you would a strange, random USB key that you&rsquo;ve picked up off the street, though&mdash;if <em>you</em> didn&rsquo;t download it from Microsoft, be wary. Microsoft&rsquo;s <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.microsoft.com/en-us/software-download/windows11&amp;xcust=2-3-542194-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">installation page</a> provides instructions for verifying the &ldquo;hash&rdquo; or identity of the ISO at the bottom of the page. If you&rsquo;ve downloaded the ISO itself, you should be fine; the hash check is just for the paranoid.</p>

Windows</div>

## This Raspberry Pi-powered BlackBerry beeper parties like it’s 2009
 - [https://www.pcworld.com/article/1923539/this-pi-powered-blackberry-beeper-parties-like-its-2009.html](https://www.pcworld.com/article/1923539/this-pi-powered-blackberry-beeper-parties-like-its-2009.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-05-19 15:35:45+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>The heydey of mobile devices with built-in keyboards is long past, eclipsed by bigger and bigger touchscreens that are now flipping and folding. But if your heart still burns for BlackBerry, the smartphone for anyone who sent more emails than text messages before the iPhone came along, there&rsquo;s a new DIY project you might want to check out. It&rsquo;s called the Beepberry, and though it isn&rsquo;t actually reviving the form factor, it&rsquo;s trying to give your thumbs the sweet, sweet feel of a tiny phone keyboard. </p>



<p>The <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://beepberry.sqfmi.com/&amp;xcust=2-2-1923539-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Beepberry</a> is a custom PCB with a teeny-tiny 2.7-inch black and white LCD screen, a Raspberry Pi Zero W &rsquo;round back covering the basic OS and wireless duties, a battery, and what looks like a genuine BlackBerry keyboard, including the company logo button and a tiny built-in touchpad. The gadget runs Pi OS Lite, but that&rsquo;s merely a means to an end, that end being <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.beeper.com/&amp;xcust=2-2-1923539-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">the Beeper app and service</a>. The Beepberry is meant to replace your phone&rsquo;s chat apps, and only chat apps, hooking into standard SMS, WhatsApp, Facebook Messenger, Telegram, Signal, Slack, Discord, and (with a bit of custom home server magic) Apple&rsquo;s iMessage. </p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Beepberry and Watchy" class="wp-image-1923702" height="783" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/beepberry-edc.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">SQFMI</p></div>



<p>As the showman says, that&rsquo;s all there is, there isn&rsquo;t any more. While the Pi Zero W can hook into local Wi-Fi or Bluetooth, the Beepberry can&rsquo;t connect to mobile networks without extra hardware, and if you want a case <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://beepberry.sqfmi.com/docs/enclosures&amp;xcust=2-2-1923539-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">you&rsquo;ll need to 3D print one yourself</a>. (Though they do look pretty snazzy!) As noted by <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://arstechnica.com/gadgets/2023/05/its-a-raspberry-pi-a-blackberry-keyboard-and-a-battery-its-the-beepberry/&amp;xcust=2-2-1923539-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Ars Technica</a>, one of the gadget&rsquo;s demo videos has the hobby-grade, 3.7-volt battery <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.youtube.com/watch?v=fIgzybDcvYk&amp;xcust=2-2-1923539-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">attached with a rubber band</a>. This disconnected-but-still-reachable concept is strictly for the DIY tinkerer crowd, and it&rsquo;s not intended as a retail product. Even though you can buy it &mdash; $79 on its own, $99 with a Pi Zero W in the box, delivery expected in August. </p>



<figure class="wp-block-embed is-type-video is-provider-youtube wp-block-embed-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">

</div></figure>



<p>The Beepberry project comes from <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://sqfmi.com/&amp;xcust=2-2-1923539-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">SQFMI</a>, a small-time studio focused on weird little gadgets like this one, founded by Pebble Watch creator Eric Migicovsky. More serious products include the Watchy, an open-source e-ink watch that&rsquo;s basically the Pebble&rsquo;s spiritual successor, and the Franky, a barebones portable gaming gadget that the Beeper is based on. Like SQFMI&rsquo;s previous projects, the Beepberry is fully open source and supported by both its creators and users on GitHub and Discord. </p>



<p>Happy texting. </p>

Smartphones</div>

## Setting up a local account in Windows 11 is tricky. Here’s how to do it
 - [https://www.pcworld.com/article/1921608/how-to-set-up-a-local-account-in-windows-11.html](https://www.pcworld.com/article/1921608/how-to-set-up-a-local-account-in-windows-11.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-05-19 14:30:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>Microsoft might want everyone on an active internet connection while setting up Windows 11, but that&rsquo;s not always possible. Some people have limited internet connections, while others may find Windows doesn&rsquo;t recognize their ethernet and/or wireless hardware.</p>



		<div class="wp-block-product-widget-block product-widget is-half-width is-float-right">
			<div class="product-widget__block-title-wrapper">
				<h4 class="product-widget__block-title" id="get-windows-11-for-120-off-in-pcworlds-software-store">
					get windows 11 for $120 off in pcworld's software store				</h4>
			</div>

			<div class="product-widget__content-wrapper">
									<div class="product-widget__title-wrapper">
						<h3 class="product-widget__title" id="windows-11-pro">Windows 11 Pro</h3>
					</div>
				
									<div class="product-widget__image-outer-wrapper">
						<div class="product-widget__image-wrapper">
							<img alt="Windows 11 Pro" class="product-widget__image" height="1330" src="https://b2c-contenthub.com/wp-content/uploads/2022/05/Windows-Insider-search-bar.png" width="2368" />
						</div>
					</div>
				
				
				<div class="product-widget__information">
												<div class="product-widget__information--rrp-wrapper">
									<span class="product-widget__information--rrp-label">
																	</span>
									<span class="product-widget__information--rrp-value">
																		</span>
								</div>
								
											<div class="product-widget__pricing-details  ">
															<span class="product-widget__pricing-details--label">
									Best Prices Today:
								</span>
														<span class="product-widget__pricing-details--links-wrapper">
								<a class="product-widget__pricing-details--link" href="https://software.pcworld.com/p43833-windows_11_professional" rel="nofollow" target="_blank">$79.99 at  PCWorld Software Store</a>							</span>
						</div>
									</div>
			</div>
		</div>

		


<p>Having no internet can seem like a big problem, too, since Microsoft doesn&rsquo;t want people creating local accounts during Windows 11 setup. Even when disconnected from the internet, the setup screen insists you sign into a Microsoft account.</p>



<p>Fortunately, you can get around this restriction. Turns out local accounts <em>are</em> still available during Windows 11 setup if you put in a little bit of keyboard work.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Windows 11 Command Prompt input for unlocking local account option" class="wp-image-1921666" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/bypass.png?w=1200" width="1200" /></figure><p class="imageCredit">PCWorld</p></div>



<p>During setup, when you reach the <em>Let&rsquo;s connect you to a network</em> screen, it will appear as if you can&rsquo;t go further without an internet connection. But you can&mdash;start by typing <code>Shift + F10</code> to open a Command Prompt window.</p>



<p>Next, type <code>OOBE\BYPASSNRO</code> into the Command Prompt window. (This command is not case sensitive, so you can enter it in lowercase and it will still work.) Your PC should reboot, then show the start of the Windows 11 setup again. Go through the same steps as before to reach <em>Let&rsquo;s connect you to a network</em> screen once more.</p>



<div class="wp-block-jetpack-slideshow aligncenter"><div class="wp-block-jetpack-slideshow_container swiper-container"><ul class="wp-block-jetpack-slideshow_swiper-wrapper swiper-wrapper"><li class="wp-block-jetpack-slideshow_slide swiper-slide"><figure><img alt="Windows 11 local account setup option unlocked" class="wp-block-jetpack-slideshow_image wp-image-1921686" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/i-dont-have-internet-copy.png" /></figure></li><li class="wp-block-jetpack-slideshow_slide swiper-slide"><figure><img alt="Windows 11 Continue with limited access" class="wp-block-jetpack-slideshow_image wp-image-1921664" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/limited-setup.png" /></figure></li></ul><a class="wp-block-jetpack-slideshow_button-prev swiper-button-prev swiper-button-white"></a><a class="wp-block-jetpack-slideshow_button-next swiper-button-next swiper-button-white"></a><a class="wp-block-jetpack-slideshow_button-pause"></a><div class="wp-block-jetpack-slideshow_pagination swiper-pagination swiper-pagination-white"></div></div></div>



<p><span style="color: initial;">You should now have a new option at the bottom right of the screen: </span><em style="color: initial;">I don&rsquo;t have internet</em><span style="color: initial;">. Choose it, then select </span><em style="color: initial;">Continue with limited setup</em><span style="color: initial;">. A screen with Microsoft&rsquo;s terms and conditions will appear. Accept to move on to the next screen, which lets you pick a name for your PC. After you create a password and security reminder questions, you&rsquo;ll finally arrive at the desktop.</span></p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Windows 11 local account user name" class="wp-image-1921663" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/user-account.png?w=1200" width="1200" /></figure><p class="imageCredit">PCWorld</p></div>



<p>By the way, if Windows 11 didn&rsquo;t recognize your ethernet and/or wireless hardware, you likely need to install their drivers. For prebuilt PCs, head to the product page for your specific model on the vendor&rsquo;s website (e.g., dell.com, hp.com, etc) to find a link to related downloads. For a DIY PC, visit the product page for your motherboard for a link to the necessary downloads.</p>



<p>Afterward, you should probably switch to logging into Windows 11 with a Microsoft account. (You can do so in <em>Settings &gt; Accounts</em>.) This sign-in method offers extra protection against dangers like loss, theft, and ransomware&mdash;for example, you get automatic device encryption on compatible PCs, as well as automatic backup of your documents, photos, and videos to your OneDrive account. You never know when having better security and rudimentary backups will bail you out of an unexpected bad situation.</p>

Windows</div>

## First Steam Deck screen replacement promises more pixels, better color
 - [https://www.pcworld.com/article/1923399/steam-deck-gets-an-aftermarket-1080p-screen-upgrade.html](https://www.pcworld.com/article/1923399/steam-deck-gets-an-aftermarket-1080p-screen-upgrade.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-05-19 14:12:30+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>The Steam Deck&rsquo;s 7-inch, 1280&times;800 screen is nothing special &mdash; the smartphone display you&rsquo;re probably reading this on has it beat in pretty much every way. But it works for the portable machine, being both cheap and fairly low-res for PC gaming on the go. But if you absolutely must have higher resolution in this form factor&hellip;well, you should probably buy the <a href="https://www.pcworld.com/article/1796614/hands-on-the-rog-ally-is-the-steam-deck-for-gamers-who-want-more-power-and-options.html">Asus ROG Ally</a>. But if you must have it for your Steam Deck, then you might want to <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.deckhd.com/&amp;xcust=2-2-1923399-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">check out the DeckHD</a>. </p>



<p>This aftermarket replacement for the Steam Deck&rsquo;s built-in LCD panel beats it in both resolution (1920&times;1200, preserving the 16:10 aspect ratio) and color accuracy, covering 95% of the sRGB color range, about as good as a mid-range laptop. Other specs match the stock screen, including 400 nits of brightness and 60Hz refresh rate, though it does come with the anti-glare coating that Valve reserves for the more expensive models of the Steam Deck. According to FX Technology Limited, the DeckHD screen will cost an estimated $99 when it launches in&hellip;well, whenever it launches. The site doesn&rsquo;t say. </p>



<p><a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.pcgamer.com/the-first-aftermarket-steam-deck-screen-upgrade-is-here-but-it-sure-seems-like-a-bad-idea/&amp;xcust=2-2-1923399-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">As PC Gamer notes</a>, replacing the screen on the Steam Deck is no small task for a DIY enthusiast, though it might not be as extensive as you imagine. According to <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://youtu.be/4T0RZ6ustKQ?t=434&amp;xcust=2-2-1923399-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">the iFixit teardown of the Steam Deck</a>, you can get the display off the device without completely disassembling it from the rear (as you need to do to, say, replace the motherboard or battery). A heat gun, some soft pry tools, and some suction cups get it away from the body, and there&rsquo;s a single phone-style connection attaching it to the rest of the device. I wouldn&rsquo;t trust it to a novice, but it&rsquo;s certainly doable if you&rsquo;ve repaired small electronics before. </p>



<figure class="wp-block-embed is-type-video is-provider-youtube wp-block-embed-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">

</div></figure>



<p>But would you want to? Both the Steam Deck&rsquo;s hardware and software is tuned pretty finely for its 800p display. It&rsquo;s certainly capable of higher resolution &mdash; you can output its video to a 4K monitor or TV, after all. But running high-end games at a higher resolution is going to push the Steam Deck&rsquo;s efficient but low-end hardware to its limit, and maybe beyond. Those who demand a higher-res screen in the same form factor might be <a href="https://www.pcworld.com/article/1796614/hands-on-the-rog-ally-is-the-steam-deck-for-gamers-who-want-more-power-and-options.html" rel="noreferrer noopener" target="_blank">better served by the $699 Asus ROG Ally</a>. Personally, I&rsquo;d prefer a replacement of the Steam Deck&rsquo;s IPS-LCD screen at the same resolution with a nice OLED panel, like the upgraded Nintendo Switch.</p>



<p>FX Technology has a waitlist for the DeckHD available now, but there&rsquo;s no pre-order or estimated release date at the time of writing. </p>

Gaming Laptops</div>

## Snatch up this gigantic 70-inch 4K LG Smart TV for just $498
 - [https://www.pcworld.com/article/1923238/1923238.html](https://www.pcworld.com/article/1923238/1923238.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-05-19 13:50:18+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>If you&rsquo;re a self-proclaimed cinephile, you better listen up. Walmart&rsquo;s currently selling the <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.walmart.com/ip/LG-70-Class-4K-UHD-2160P-webOS-Smart-TV-70UQ7070ZUD/642419413&amp;xcust=2-2-1923238-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">LG Smart TV for $498</a>, which is a savings of $150. This TV is truly designed for the ultimate movie watching experience. It&rsquo;s an absolute beast at 70-inches, which really ups the immersion factor. The 4K resolution means sharp and colorful visuals as well. Let&rsquo;s dive into the other features.</p>



<p>This TV features instant access of up to 300+ LG channels and streaming services, which includes everything from Netflix to Disney+. The 5 Gen5 AI processor further enhances the picture and sound, too. You can also adjust your game settings on the Game Optimizer &amp; Dashboard feature. It&rsquo;s a definitely a versatile TV that&rsquo;s chock-full of cool features. </p>



<p>And did we mention it&rsquo;s <em>a gigantic 70-inch 4K TV for under $500</em>? This is an absolutely killer deal. You better hop on it now before it&rsquo;s gone.</p>


<p class="cta wp-block wp-block-button"><a class="cta__btn" href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.walmart.com/ip/LG-70-Class-4K-UHD-2160P-webOS-Smart-TV-70UQ7070ZUD/642419413&amp;xcust=2-2-1923238-7-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Get the LG Smart TV for $498 at Walmart</a></p>
Smart TVs</div>

## DLSS 3 explained: How Nvidia’s AI-infused RTX tech turbocharges PC gaming
 - [https://www.pcworld.com/article/1662185/what-is-dlss-3-nvidia-geforce-rtx-ai-feature-explained.html](https://www.pcworld.com/article/1662185/what-is-dlss-3-nvidia-geforce-rtx-ai-feature-explained.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-05-19 13:10:56+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>You might spend top dollar for fancy new graphics card hardware, but one of the key components to gaming performance is actually software. While the brute force of the hardware gets most of the glory (and is indeed essential), the software side is the magic that pieces it together. Without good software, even the ferocious <a href="https://www.pcworld.com/article/1348123/nvidia-geforce-rtx-4090-review-ada-lovelace.html">Nvidia GeForce RTX 4090</a> is reduced to a fancy paperweight&mdash;especially when running <a href="https://www.pcworld.com/article/1782490/cyberpunk-2077-overdrive-mode-benchmarks-nvidia-rtx.html"><em>Cyberpunk 2077</em>&lsquo;s glorious new path traced Overdrive mode</a>.&nbsp;</p>



<p>Software can also substantially <em>improve</em> the hardware performance. Enter Nvidia&rsquo;s DLSS 3.0, or Deep Learning Super Sampling. Including both AI-powered frame generation and <a href="https://www.pcworld.com/article/393646/tested-how-nvidia-reflex-can-make-you-a-better-esports-gamer.html">Nvidia&rsquo;s wondrous latency-reducing Reflex technology</a>, DLSS 3.0 makes for a potent recipe.&nbsp;And with the unveiling of <a href="https://www.pcworld.com/article/1921195/nvidia-unveils-3-geforce-rtx-4060-ti-gpus-dlss-3-goes-mainstream.html">affordable new GeForce RTX 4060 and 4060 Ti</a> graphics cards, this fantastic technology is about to become a lot more accessible.</p>



<p>This isn&rsquo;t the same old DLSS upsampling you&rsquo;re used to, however. We&rsquo;re going to go over some basics of what DLSS 3.0 is, and its application to Nvidia&rsquo;s RTX 40-series GPUs. We&rsquo;ll let you know how to use this feature, and tell you about optimal settings on some popular supported games. Let&rsquo;s get cracking.</p>



<blockquote class="wp-block-quote"><p><strong>Further reading: </strong><a href="https://www.pcworld.com/article/416006/the-best-graphics-cards-for-pc-gaming.html">The best graphics cards for PC gaming</a></p></blockquote>



<h2 id="how-does-dlss-3-work">How does DLSS 3 work?</h2>



<p>DLSS 3 greatly accelerates gaming frame rates using a mixture of AI tasks running on dedicated tensor cores. It has three components that make it tick.&nbsp;</p>



<figure class="wp-block-embed is-type-video is-provider-youtube wp-block-embed-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">

</div></figure>



<p><strong>Super Resolution (a.k.a. DLSS 2)</strong></p>



<p>Also known as super sampling, DLSS 3&rsquo;s core &ldquo;upscaler&rdquo; functionality is actually the DLSS 2 technology already integrated into countless games. DLSS renders game imagery at a lower resolution than your monitor runs at to increase raw gaming frame rates, then uses AI tensor cores to reconfigure the image with machine learning so that it looks sharp on your screen. This bypasses the performance penalty that your higher resolution would impose, while keeping graphics fidelity high.&nbsp;</p>



<p><strong>Frame generation</strong></p>



<p>The novel element to DLSS 3 is in the &ldquo;Optical Multiframe Generation&rdquo; AI technology. After analyzing two images from a game back-to-back, DLSS 3 uses this information to insert an extra AI-created frame that does not have to be rendered by the game itself. This result is in even higher frame rates than standard DLSS 2. It can also help dramatically increase the smoothness in CPU bottlenecked games.&nbsp;</p>



<p><strong>Nvidia Reflex low latency</strong></p>



<p>The third piece of the puzzle is in Nvidia&rsquo;s Reflex technology. Frame generation is not free. Those AI-generated frames aren&rsquo;t controlled by the player, since the game isn&rsquo;t rendering them, so it can actually add latency (read: reduce responsiveness) in games. To combat this, Nvidia Reflex helps harmonize the GPU and CPU so that latency is reduced. It helps to bypass the traditional bottlenecks presented by both the GPU and CPU by deeper integration into the game engine itself. Reflex was created years ago to <a href="https://www.pcworld.com/article/393646/tested-how-nvidia-reflex-can-make-you-a-better-esports-gamer.html">improve performance in esports games to amazing effect</a>, but Nvidia now requires it in games that support DLSS 3.</p>



<p>Speaking of&hellip;  &nbsp;</p>



<h2><strong>What do you need to run DLSS 3?</strong></h2>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Nvidia DLSS 3" class="wp-image-1662196" height="813" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/Screenshot-2022-12-06-at-3.09.37-PM.png?w=1200" width="1200" /></figure><p class="imageCredit">Thiago Trevisan</p></div>



<p><strong>An RTX 40-series graphics card</strong></p>



<p>DLSS 3 is exclusive to Nvidia&rsquo;s &ldquo;Ada Lovelace&rdquo; RTX 40-series graphics cards. It is available for both desktop and laptop offerings, but not any RTX 30-series or prior GPUs.&nbsp;</p>



<p>Nvidia says that&rsquo;s because the new Lovelace GPU architecture includes more powerful AI tensor cores and, more critically, a new &ldquo;Optical Flow Accelerator&rdquo; that provides scene movement info critical to creating those AI frames. Performance on RTX 30 or older GPUs would not provide a good experience, so for now this technology is limited to the more powerful hardware.&nbsp;Currently, four RTX 40-series graphics cards are available that meet those requirements:</p>



<ul><li>The <a href="https://www.pcworld.com/article/1348123/nvidia-geforce-rtx-4090-review-ada-lovelace.html">$1,600 RTX 4090</a></li><li>The <a href="https://www.pcworld.com/article/1379747/nvidia-geforce-rtx-4080-tested-5-things.html">$1,200 RTX 4080</a></li><li>The <a href="https://www.pcworld.com/article/1444726/nvidia-geforce-rtx-4070-ti-review.html">$800 RTX 4070 Ti</a></li><li>The <a href="https://www.pcworld.com/article/1781139/nvidia-geforce-rtx-4070-review.html">$600 RTX 4070</a></li><li>The <a href="https://www.pcworld.com/article/1921195/nvidia-unveils-3-geforce-rtx-4060-ti-gpus-dlss-3-goes-mainstream.html">$399 RTX 4060 Ti 8GB</a> (coming May 24) or <a href="https://www.pcworld.com/article/1921195/nvidia-unveils-3-geforce-rtx-4060-ti-gpus-dlss-3-goes-mainstream.html">$499 RTX 4060 Ti 16GB</a> (July 2023)</li><li>The <a href="https://www.pcworld.com/article/1921195/nvidia-unveils-3-geforce-rtx-4060-ti-gpus-dlss-3-goes-mainstream.html">$299 RTX 4060</a> (coming July 2023)</li></ul>



<p>DLSS 3 is not supported on rival AMD Radeon or Intel Arc graphics cards.</p>



<p><strong>Certain Windows settings need to be active</strong></p>



<p>You&rsquo;ll also need to turn on &ldquo;Hardware Accelerated GPU&rdquo; in your Windows display settings. (<em>Settings &gt; System &gt; Display &gt; Related Sections &gt; Graphics &gt; Change Default Graphics Settings &gt; </em>Toggle <em>Hardware-accelerated GPU scheduling</em> on)</p>



<p><strong>Certain in-game settings need to be active</strong></p>



<p>Only specific games directly support DLSS 3. You&rsquo;ll have to turn on &ldquo;Frame Generation&rdquo; settings after activating DLSS upscaling. This will also necessitate &ldquo;Nvidia Reflex&rdquo; being turned on, and most (but not all) games will do this by default. You&rsquo;ll further have the option to set Reflex to additional &ldquo;Boost.&rdquo;&nbsp;</p>



<p><strong>Supported DLSS 3 games</strong></p>



<p>There are currently over 25 games that are playable now, with many more coming. High profile titles like <em>Cyberpunk 2077</em> and <em>Forza Horizon 5 </em>have recently received DLSS 3 updates, along with new releases such as <em>Hogwarts Legacy</em>. <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.rockpapershotgun.com/confirmed-ray-tracing-and-dlss-games&amp;xcust=2-3-1662185-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Rock Paper Shotgun</a> maintains a helpful guide to all available and upcoming DLSS 3 games (they&rsquo;re after the ray traced and DLSS games in the list).</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Nvidia DLSS 3" class="wp-image-1662201" height="651" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/Screenshot-2023-03-13-at-12.02.11-PM.png?w=1200" width="1200" /><figcaption><p>Hitman 3 menu: DLSS &nbsp;on Balanced, with Frame Generation and Reflex set to On.</p>
</figcaption></figure><p class="imageCredit">Thiago Trevisan</p></div>



<h2 id="what-are-dlss-3s-drawbacks">What are DLSS 3&rsquo;s drawbacks?</h2>



<p>DLSS 3 is fantastic for increasing overall visual smoothness, but as it develops during its early days, it also has a few potential issues to be aware of.&nbsp;</p>



<p><strong>Latency</strong></p>



<p>While Nvidia Reflex addresses a lot of DLSS 3&rsquo;s latency concerns, it&rsquo;s also not the rapid response some users may expect from esports titles. That&rsquo;s why DLSS 3 is better suited for single player games such as <em>Cyberpunk 2077</em>, <em>Plague Tale Requiem</em>, <em>Microsoft Flight Simulator</em>, etc.&nbsp;Even with Reflex on, DLSS 3 can play a sort of trick on your mind if you&rsquo;re especially sensitive to how fast frame rates and responsiveness are intertwined, as PCWorld&rsquo;s Brad Chacos explained during his review of the RTX 4090:</p>



<blockquote class="wp-block-quote"><p>&ldquo;While the DLSS 3 experience shines, it doesn&rsquo;t always&nbsp;<em>feel</em>&nbsp;more responsive in your hands. Running&nbsp;<em>Cyberpunk 2077&nbsp;</em>at 138fps with every possible bell and whistle active thanks to DLSS 3 looks absolutely stunning, full stop. But one of the perks of faster frame rates is increased responsiveness, and while Reflex greatly helps with that,&nbsp;<em>Cyberpunk 2077</em>&nbsp;running at 138fps doesn&rsquo;t&nbsp;<em>feel</em>&nbsp;substantially more responsive than running it at the 77fps or so it hits in native 4K. Having twice as many frames looks fantastic but those AI frames aren&rsquo;t responding to your controls in the actual moment, though it&rsquo;s close.</p><p>This is not a negative. This is not a drawback. It can&rsquo;t be after running&nbsp;<em>Flight Sim&nbsp;</em>at 120fps, and&nbsp;<em>Cyberpunk 2077</em>&nbsp;with ultra ray tracing at 138fps (the RTX 3090 tops out at 48fps). But it&rsquo;s worth highlighting.&rdquo;</p></blockquote>



<p><strong>Visual artifacts</strong></p>



<p>Most of the DLSS 3 gaming experience looks fantastic. You won&rsquo;t notice any visual issues or quirks. That said, there are some games that showcase some onscreen &ldquo;artifacts&rdquo; or abnormalities. UI elements can also not be displayed properly in some titles, all areas that are undergoing improvement. The good news is that software updates can remedy these issues as gamers age. The Hardware Unboxed deep dive embedded below does a great job of walking through DLSS 3&rsquo;s visual quality, including highlighting potential quirks.</p>



<figure class="wp-block-embed is-type-video is-provider-youtube wp-block-embed-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">

</div></figure>



<p><strong>Needs powerful hardware</strong></p>



<p>DLSS 3 shows some of its best results on already powerful hardware, like the Nvidia RTX 4080 or 4090. It also seems to do better when it&rsquo;s boosting an already-okay frame rate to a higher one, such as 60 FPS to 120 FPS. Time will tell if upcoming weaker GPUs such as the RTX 4060 will still have the same impressive results, but it should be promising.&nbsp;</p>



<p><strong>Settings overload</strong></p>



<p>Console gamers have it easy without as much customization sometimes! PC games not only have dozens of graphics settings, but it also has different levels for each one. Add to that DLSS 3, which now has its own hierarchy of graphic settings to learn.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Nvidia DLSS 3" class="wp-image-1662202" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/Screenshot-24.png?w=1200" width="1200" /><figcaption><p>Hogwarts: Legacy has a lot of settings to tinker with, including DLSS tiers.</p>
</figcaption></figure><p class="imageCredit">Thiago Trevisan</p></div>



<h2><strong>DLSS 3 settings explained&nbsp;</strong></h2>



<p>Dozens more settings variations have entered the fray &ndash; making it confusing for gamers when choosing your graphics settings. After activating DLSS, Frame Generation, and Reflex, you have a few more choices to make.</p>



<p><strong>DLSS feature options</strong></p>



<ul><li><strong>DLSS Auto</strong>: This will try and keep the frames as best it can to your monitor&rsquo;s refresh rate</li><li><strong>DLSS Quality</strong>: The best visual performance, with modest or not much FPS uplift&nbsp;</li><li><strong>DLSS Balanced</strong>: A good combination of higher frames and maintaining graphical fidelity.&nbsp;</li><li><strong>DLSS Performance</strong>: You&rsquo;ll notice somewhat less impressive visuals, but FPS frames are considerably higher.&nbsp;</li><li><strong>DLSS Ultra-performance</strong>: Better FPS, but worse visuals &ndash; typically when you really want to overreach existing hardware or to hit a specific FPS at a higher resolution. (8K Gamers, you&rsquo;ll want to learn this one!)&nbsp;</li><li><strong>DLSS Frame Generation</strong>: This setting will just be a simple &ldquo;On or Off&rdquo; toggle in your game settings. Remember, you&rsquo;ll need Ada Lovelace RTX 40 series GPUs to work.&nbsp;</li></ul>



<h3><strong>Nvidia Reflex and Boost</strong></h3>



<p>These are often found near DLSS options, but may be elsewhere in a video menu as well (as in <em>Cyberpunk 2077</em>). Nvidia Reflex will often be turned on automatically in most games with Frame Generation being active. That&rsquo;s not always true, however, and many games let you disable Reflex manually even when running DLSS 3 Frame Gen. (We don&rsquo;t recommend doing that.) You&rsquo;ll also have the option for a &ldquo;Boost&rdquo; feature in many games. Reflex Boost overclocks your GPU so it can help in CPU limited scenarios even more.&nbsp;</p>



<p><strong>Even more options</strong></p>



<p>To make matters a bit more complicated, some games even allow you to select only <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.techpowerup.com/review/nvidia-dlaa-anti-aliasing/&amp;xcust=2-3-1662185-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Nvidia&rsquo;s DLAA</a> along with Frame Generation and Reflex. <em>Plague Tale&rsquo;s Requiem</em> is one such title. DLAA basically runs DLSS at your native monitor resolution for enhanced visual sharpness and clarity. When given this option, it offers the highest possible graphical setting you can achieve, balanced out by the obvious performance cost. You can usually choose DLSS instead if the DLAA performance is too low.&nbsp;</p>



<p>In most games, such as <em>Hogwarts Legacy</em>, DLAA will automatically be grayed out when you select DLSS.&nbsp;</p>



<p><strong>The best DLSS 3 settings</strong></p>



		<div class="wp-block-product-widget-block product-widget">
			<div class="product-widget__block-title-wrapper">
				<h4 class="product-widget__block-title" id="the-most-powerful-gpu-is-a-dlss-3-monster">
					The most powerful gpu is a dlss 3 monster				</h4>
			</div>

			<div class="product-widget__content-wrapper">
									<div class="product-widget__title-wrapper">
						<h3 class="product-widget__title" id="geforce-rtx-4090-founders-edition">GeForce RTX 4090 Founders Edition</h3>
					</div>
				
									<div class="product-widget__image-outer-wrapper">
						<div class="product-widget__image-wrapper">
							<img alt="GeForce RTX 4090 Founders Edition" class="product-widget__image" height="1667" src="https://b2c-contenthub.com/wp-content/uploads/2022/10/Nvidia-GeForce-RTX-4090-1.jpg?quality=50&amp;strip=all" width="2500" />
						</div>
					</div>
				
									<div class="review product-widget__review-details">
						<img alt="Editors' Choice" class="product-widget__review-details--editors-choice-logo" src="https://www.pcworld.com/wp-content/uploads/2021/09/PC-ED-CHOICE.png" />							<div class="product-widget__rating-and-review-link">
								<div class="product-widget__review-details--rating">
											<div class="starRating"></div>
										</div>									<a class="product-widget__review-link" href="https://www.pcworld.com/article/1348123/nvidia-geforce-rtx-4090-review-ada-lovelace.html" target="_blank">Read our review</a>
									
							</div>
											</div>
				
				<div class="product-widget__information">
											<div class="product-widget__information--rrp-wrapper">
								<span class="product-widget__information--rrp-label">
															</span>
								<span class="product-widget__information--rrp-value">
																</span>
							</div>
						
									</div>
			</div>
		</div>

		


<p>Here&rsquo;s how we use DLSS 3 settings in our own rigs. For the most powerful hardware, such as the RTX 4080 and 4090, DLSS Quality should keep respectable frames in most games, even at 4K, and doubly so with DLSS Frame Generation enabled.&nbsp; If you prefer a bit more pep in performance, DLSS Balanced would be the next ideal step.&nbsp; You can also always just set DLSS to Auto and see if you&rsquo;re happy with the results, as they will vary from game-to-game.&nbsp;</p>



<p>If you have slightly less powerful hardware, such as the RTX 4070 or some mobile RTX 40 GPUs, DLSS Balanced and DLSS Performance become good settings to make sure you&rsquo;re hitting good frames, with the nod still going to DLSS Balanced as preferred.&nbsp;We&rsquo;d typically recommend avoiding DLSS Ultra Performance, as it upscales from such a low resolution image that it degrades visual fidelity a noticeable amount.&nbsp;</p>



<p>Some games are just more demanding than others, so you&rsquo;ll be able to judge if changes are needed, especially when adding ray tracing.&nbsp;</p>



<h2><strong>DLSS 3: Let&rsquo;s play some games!&nbsp;</strong></h2>



		<div class="wp-block-product-widget-block product-widget">
			<div class="product-widget__block-title-wrapper">
				<h4 class="product-widget__block-title" id="">
									</h4>
			</div>

			<div class="product-widget__content-wrapper">
									<div class="product-widget__title-wrapper">
						<h3 class="product-widget__title" id="msi-titan-gt77-hx-13v">MSI Titan GT77 HX 13V</h3>
					</div>
				
									<div class="product-widget__image-outer-wrapper">
						<div class="product-widget__image-wrapper">
							<img alt="MSI Titan GT77 HX 13V" class="product-widget__image" height="1000" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/msi-titan-gt77-4-1.jpg?quality=50&amp;strip=all" width="1500" />
						</div>
					</div>
				
									<div class="review product-widget__review-details">
						<img alt="Editors' Choice" class="product-widget__review-details--editors-choice-logo" src="https://www.pcworld.com/wp-content/uploads/2021/09/PC-ED-CHOICE.png" />							<div class="product-widget__rating-and-review-link">
								<div class="product-widget__review-details--rating">
											<div class="starRating"></div>
										</div>									<a class="product-widget__review-link" href="https://www.pcworld.com/article/1561127/msi-titan-gt77-hx-13v-review.html" target="_blank">Read our review</a>
									
							</div>
											</div>
				
				<div class="product-widget__information">
												<div class="product-widget__information--rrp-wrapper">
									<span class="product-widget__information--rrp-label">
																	</span>
									<span class="product-widget__information--rrp-value">
																		</span>
								</div>
								
									</div>
			</div>
		</div>

		


<p>Time to put this theory to practice. We&rsquo;re going to play some particularly intense games and see how DLSS 3 can help. These games were tested at 4K, generally with Ultra or similar max settings, and ray tracing on. The hardware is an <a href="https://www.pcworld.com/article/1561127/msi-titan-gt77-hx-13v-review.html">MSI Titan GT77 laptop with a 4090 inside</a>, which is similar to an RTX 3090 Ti desktop GPU in performance.&nbsp;</p>



<p>Keep in mind that this is at 4K, so people playing at lower resolutions such as 1440p or 1080p will always see higher FPS in general. Ray tracing also substantially lowers frame rates when on, so disabling that is another way you can achieve higher numbers. The idea with DLSS 3 is that we can have our cake and eat it too! You can experience ray tracing on Ultra, then flip on DLSS 3 to achieve better performance without compromising on other visual settings.&nbsp;</p>



<h2><strong>DLSS 3: Cyberpunk 2077</strong></h2>



<p><em>Cyberpunk 2077</em> has been around for a few years now, and recently it received DLSS 3 support. This game is notorious for crushing almost any GPU when ray tracing is on Ultra so it&rsquo;s welcomed news.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Nvidia DLSS 3" class="wp-image-1662205" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/nodlssnoframegen.png?w=1200" width="1200" /><figcaption><p>Ray tracing Ultra, DLSS Off at 4K.</p>
</figcaption></figure><p class="imageCredit">Thiago Trevisan</p></div>



<p>Let&rsquo;s go over how some of the settings affect the overall performance by really pushing the system. On the MSI GT77 Titan, ray tracing on Ultra without any DLSS gives us a measly 27 FPS in this portion. That frame rate is too low to actually play, so let&rsquo;s see how DLSS 3 can help us without having to reduce any other graphics settings.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Nvidia DLSS 3" class="wp-image-1662206" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/dlssbalnoframegen.png?w=1200" width="1200" /><figcaption><p>DLSS Set to Balanced, without Frame Generation or Reflex.</p>
</figcaption></figure><p class="imageCredit">Thiago Trevisan</p></div>



<p>Next, let&rsquo;s turn on DLSS to Balanced, but without switching on Frame Generation or Nvidia Reflex. Our frame rate jumps to 61, a much better result. The game still looks great and behaves much smoother with this extra FPS boost.</p>



<p><img alt="A picture containing text, tollbooth, bus

Description automatically generated" src="https://lh5.googleusercontent.com/Sq2B21BRPU_6Q_9lz4v8e5BAvmN14M1iPPxI00vkUeSKiqSQrPHGOwarH6O9OJdx9waPqxof_7Vn7xUP-xFfNjiVNdBp9PF9p598hTdIosX9hbA-1wjTrHXMGMnaVLaRjXxJfVP2k3SCd-z7nVD4iQ" style="width: 1200px;" /></p>



<p>Our next option will have us once again setting DLSS to Balanced, but this time we&rsquo;re also going to turn on Frame Generation in the menu. Nvidia Reflex, on the adjacent &ldquo;Video&rdquo; menu, will also be on. The result here is substantially better&mdash;a whopping 87 FPS. Remember that we started with just 27 FPS before turning on any DLSS features.&nbsp;</p>



<p>How does it play with DLSS 3 Frame Gen active? Quite well, actually. It feels superior in every way to native rendering, or with just regular DLSS on. The game play is smooth, and no glaringly obvious artifacts or issues present themselves. (They can still happen, however, such as UI elements being a bit quirky at times.)&nbsp;</p>



<p>The only downside here is that you&rsquo;re increasing latency, which is somewhat by Nvidia Reflex. The latency in this game is acceptable, as it&rsquo;s mostly a single player game where you&rsquo;re exploring and occasionally engaging in faster scenes.&nbsp;</p>



<p>A faster paced game, such as an online multiplayer esports title, is not an ideal match for DLSS 3 due to this latency factor.&nbsp; In <em>Cyberpunk 2077</em>, it works beautifully. You can also turn on Frame Generation and Reflex without DLSS, giving you FPS of around 47, but here the greater benefit seems to be pairing it with DLSS so you can achieve maximum frame rates.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Nvidia DLSS 3" class="wp-image-1662209" height="1021" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/dlss3-cyberpunk.jpg?quality=50&amp;strip=all" width="1024" /><figcaption><p>From Brad Chacos&rsquo; RTX 4090 review.</p>
</figcaption></figure><p class="imageCredit">Brad Chacos</p></div>



<p>In Brad Chacos&rsquo; <a href="https://www.pcworld.com/article/1348123/nvidia-geforce-rtx-4090-review-ada-lovelace.html">RTX 4090 desktop GPU review</a>, we can see that even this ferocious flagship gets massive help from DLSS 3. Playing it at 4K resolution with ray tracing at Ultra pins the game to 42 FPS, but DLSS performance with Frame Generation brings it to 138 FPS. These are staggering numbers&mdash;with ray tracing still on!</p>



<h2><strong>DLSS 3: Hitman 3</strong></h2>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Nvidia DLSS 3" class="wp-image-1662212" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/nodflss.png?w=1200" width="1200" /><figcaption><p>Hitman 3 without DLSS at 4K, and all settings maxed out to their highest.</p>
</figcaption></figure><p class="imageCredit">Thiago Trevisan</p></div>



<p><em>Hitman 3</em> is a popular game that also taxes systems quite heavily. With ray tracing on and DLSS off, this scene gave us only around 30 FPS at maxed-out 4K settings. This game is much like <em>Cyberpunk 2077</em>, in the sense that it&rsquo;s a slower paced style game, so DLSS 3 can be a big help here.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Nvidia DLSS 3" class="wp-image-1662213" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/dlssnbalnoframegen.png?w=1200" width="1200" /><figcaption><p>Hitman 3: DLSS Balanced only, no Frame Generation or Reflex.</p>
</figcaption></figure><p class="imageCredit">Thiago Trevisan</p></div>



<p>Switching DLSS on to Balanced, but keeping Frame Generation Off, wielded 64 FPS. That&rsquo;s surely a significant boost, and makes the game feel tremendously more playable and smooth.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Nvidia DLSS 3" class="wp-image-1662216" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/dlssbalframegen.png?w=1200" width="1200" /><figcaption><p>DLSS Balanced, with Frame Generation and Reflex On.</p>
</figcaption></figure><p class="imageCredit">Thiago Trevisan</p></div>



<p>Finally, switching DLSS to Balanced, but turning on both Frame Generation and Reflex, give us truly impressive results. We&rsquo;re now around 91 FPS, a big leap from the original 30 FPS without DLSS 3. The game feels much smoother, and behaves very well. It&rsquo;s difficult to even notice the DLSS process occurring unless you&rsquo;re pixel-peeping for it.</p>



<p>Like with the other games, latency will also be increased, and helped with Nvidia Reflex. This title is one that benefits much more from the higher FPS and better performance, and any additional latency is not very noticeable. You can also select only Frame generation and Reflex without DLSS, giving you around 50 FPS. We&rsquo;d still recommend going all the way with DLSS Quality or Balanced however, so you get all of the combined DLSS 3 benefits.&nbsp;</p>



<h2><strong>DLSS 3: Hogwarts Legacy</strong></h2>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Nvidia DLSS 3" class="wp-image-1662219" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/nodlssnoframegen-1.png?w=1200" width="1200" /><figcaption><p>Hogwarts legacy: No DLSS, Ray Tracing Ultra 4K.</p>
</figcaption></figure><p class="imageCredit">Thiago Trevisan</p></div>



<p>Continuing the trend of highly taxing ray traced titles, we arrive at <em>Hogwarts Legacy</em>. Without any DLSS, and when set to Nvidia DLAA, this scene in Hogmeade netted us only 36 FPS at 4K. Ick. Ray tracing and all settings are set to Ultra.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Nvidia DLSS 3" class="wp-image-1662220" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/dlssbal.png?w=1200" width="1200" /><figcaption> DLSS Balanced, no Frame Generation or Reflex.</figcaption></figure><p class="imageCredit">Thiago Trevisan</p></div>



<p>We see better results with DLSS set to Balanced, with frame rates hitting around 59. The game feels much better already, and even the frame rate time seems more consistent. (You can also turn on just Frame Generation without DLSS, getting around 56 FPS, but your latency will also increase more that way, so better to pair it with DLSS.)</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Nvidia DLS 3" class="wp-image-1662223" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/dlssframegenbal.png?w=1200" width="1200" /><figcaption><p>DLSS Balanced, Frame Generation and Reflex On.</p> </figcaption></figure><p class="imageCredit">Thiago Trevisan</p></div>



<p>DLSS Balanced alongside Frame Generation and Reflex give us 82 FPS, a huge boost from the 36 FPS we first saw. The game plays considerably better, with much more consistent and smooth performance. Without DLSS 3, we&rsquo;d have to lower ray tracing or adjust other settings to achieve better results, so this is certainly a much more preferable option.&nbsp;Reflex kept the game feeling nice and responsive.</p>



<h2><strong>DLSS 3: Flight Simulator 2020</strong></h2>



<p>Microsoft Flight Simulator 2020 is a notoriously difficult game to max out thanks to its beautifully expansive open world. It&rsquo;s a highly CPU bottlenecked game, making a perfect pairing with DLSS 3.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Nvidia DLSS 3" class="wp-image-1662228" height="1005" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/dlss-3-flight-sim.jpg?quality=50&amp;strip=all" width="1024" /><figcaption><p>From Brad Chacos&rsquo; RTX 4090 review.</p>
</figcaption></figure><p class="imageCredit">Brad Chacos</p></div>



<p>The results here are nothing short of impressive. With the desktop RTX 4090 and a Ryzen 9 5900X processor, 4K native hits a playable 65 FPS&mdash;a standard result for this heavily CPU-bottlenecked game. Turning on Frame Generation and bypassing that bottleneck brings us to 122 FPS, almost doubling the visual smoothness by blowing past the bottleneck with AI frames. Nvidia Reflex helps to keep the latency in check, and this is a game generally well suited to DLSS 3 improvements.&nbsp;</p>



<p>This title also has numerous detailed UI and in-cabin graphics that have to be generated properly, so it&rsquo;s a great test of how DLSS 3 can render minute details in sharp clarity. While it&rsquo;s not always perfect, the boost in FPS and bypassing CPU bottlenecks are more than a win here.&nbsp;</p>



<h2><strong>DLSS 3: Final thoughts&nbsp;</strong></h2>



<p>Nvidia&rsquo;s DLSS 3 combines the great benefits of DLSS, along with Frame Generation and Nvidia Reflex. While support is still limited to select games and hardware, and there are sometimes niggling artifacting and text issues, it&rsquo;s extraordinarily promising.&nbsp;By allowing GPUs to stretch their legs well beyond traditional hardware limits, we can experience higher and better frontiers in games as developers take advantage of the technology.&nbsp;</p>



<p>Sure, you&rsquo;re getting some more latency, but Nvidia Reflex does a good job at keeping it under control. Often, it makes DLSS 3 games even <em>more</em> responsive than running at native resolution. While you&rsquo;re not likely to want to play <em>Counter-Strike</em> or the like with it on, DLSS 3 is a huge boost to games such as <em>Cyberpunk 2077</em>.</p>



<p>With everything running well, DLSS 3 feels like black magic. Games shouldn&rsquo;t run this good or look this smooth. If your PC supports it, we highly recommend checking it out.</p>



		<div class="wp-block-product-widget-block product-widget">
			<div class="product-widget__block-title-wrapper">
				<h4 class="product-widget__block-title" id="the-most-affordable-rtx-gpu-for-dlss-3">
					The most affordable rtx gpu for dlss 3				</h4>
			</div>

			<div class="product-widget__content-wrapper">
									<div class="product-widget__title-wrapper">
						<h3 class="product-widget__title" id="geforce-rtx-4070">GeForce RTX 4070</h3>
					</div>
				
									<div class="product-widget__image-outer-wrapper">
						<div class="product-widget__image-wrapper">
							<img alt="GeForce RTX 4070" class="product-widget__image" height="1667" src="https://b2c-contenthub.com/wp-content/uploads/2023/04/DSC02116.jpg?quality=50&amp;strip=all" width="2500" />
						</div>
					</div>
				
									<div class="review product-widget__review-details">
													<div class="product-widget__rating-and-review-link">
								<div class="product-widget__review-details--rating">
											<div class="starRating"></div>
										</div>									<a class="product-widget__review-link" href="https://www.pcworld.com/article/1781139/nvidia-geforce-rtx-4070-review.html" target="_blank">Read our review</a>
									
							</div>
											</div>
				
				<div class="product-widget__information">
												<div class="product-widget__information--rrp-wrapper">
									<span class="product-widget__information--rrp-label">
																	</span>
									<span class="product-widget__information--rrp-value">
																		</span>
								</div>
								
											<div class="product-widget__pricing-details  ">
															<span class="product-widget__pricing-details--label">
									Best Prices Today:
								</span>
														<span class="product-widget__pricing-details--links-wrapper">
								<a class="product-widget__pricing-details--link" href="https://bestbuy.7tiv.net/c/321564/633495/10014?prodsku=6539358&amp;u=https%3A%2F%2Fapi.bestbuy.com%2Fclick%2F-%2F6539358%2Fpdp&amp;intsrc=CATF_4831&amp;subid1=2-3-1662185-5-1781203-11566" rel="nofollow" target="_blank">$599.99 at  Best Buy</a>							</span>
						</div>
									</div>
			</div>
		</div>

		


<p><em>Editor&rsquo;s note: This article first published on April 14, 2023, but was updated to include new RTX 4060 GPUs and explicitly explain where to turn on Hardware-accelerated GPU scheduling.</em></p>

Graphics Cards</div>

## Lenovo Legion Pro 7i review: Blazing performance, good price
 - [https://www.pcworld.com/article/1816509/lenovo-legion-pro-7i-review.html](https://www.pcworld.com/article/1816509/lenovo-legion-pro-7i-review.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-05-19 10:45:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>


<div class="review" id="review-body"><img alt="Editors' Choice" class="review-logo" src="https://www.pcworld.com/wp-content/uploads/2021/09/PC-ED-CHOICE.png" /><span class="review-title">At a glance</span><h3 class="review-subTitle" id="experts-rating">Expert's Rating</h3><div class="starRating"></div>
<div><div class="review-columns"><div class="review-column"><h3 class="review-subTitle" id="pros">Pros</h3><ul class="pros review-list"><li>Strong overall performance</li><li>Display is big, bright and fast</li><li>Per-key RGB lighting</li></ul></div><div class="review-column"><h3 class="review-subTitle" id="cons">Cons</h3><ul class="cons review-list"><li>Some flex to keyboard deck</li><li>Poor battery life</li></ul></div></div></div><h3 class="review-subTitle review-subTitle--borderTop" id="our-verdict">Our Verdict</h3><p class="verdict">Armed with a 13th-gen Core i9 CPU and RTX 4070 graphics, the Lenovo Legion Pro 7i Gen 8 is mid-priced powerhouse.</p>
</div>


<p>The Lenovo Legion Pro 7i Gen 8 delivers the latest from Intel and Nvidia for a fraction of the cost of premium models that feature higher-grade RTX 40-series GPUs. We&rsquo;ve reviewed two admittedly impressive RTX 4090-based gaming monsters&mdash;the <a href="https://www.pcworld.com/article/1801763/razer-blade-16-review.html">$4,300 Razer Blade 16</a> and the <a href="https://www.pcworld.com/article/1561127/msi-titan-gt77-hx-13v-review.html">$5,300 (!) MSI Titan GT 77 HX 13V</a>&mdash;that are more show pieces than attainable objects for most. This laptop will fit into many more budgets.&nbsp;</p>



<p>You can outfit the Legion Pro 7i Gen 8 with an RTX 4080 or RTX 4090 GPU, but our test model features a RTX 4070 GPU and is roughly half the price of the Razer Blade 16 we reviewed recently. It lacks the striking design of the slab-like Razer as well as its dual-mode display, but the look and build quality is certainly appropriate for a midrange gaming laptop. And the 16-inch display is spacious, crisp, bright, and fast. After dreaming about owning a $4,000 or $5,000 next-gen gaming laptop, the next-gen Pro 7i Gen 8 is a solid choice for when you snap back to reality and your financial constraints.</p>



<blockquote class="wp-block-quote"><p>Looking for more options? If so, check out our roundup of the <a href="https://www.pcworld.com/article/407493/best-gaming-laptops.html">best gaming laptops</a> available today.</p></blockquote>



<h2 id="lenovo-legion-pro-7i-gen-8-specifications">Lenovo Legion Pro 7i Gen 8: Specifications</h2>



<p>Our Lenovo Legion Pro 7i Gen 8 test system costs $2,175 from Lenovo and features the following specs:</p>



<ul><li><strong>CPU:</strong> Quad-core Intel Core i9-13900HX</li><li><strong>Memory: </strong>32GB DDR5 5600MHz</li><li><strong>Graphics:</strong> Nvidia GeForce RTX 4070</li><li><strong>Storage: </strong>1TB PCIe NVMe M.2 SSD</li><li><strong>Display: </strong>16-inch QHD (2560&times;1600) 240Hz display</li><li><strong>Webcam: </strong>1080p with electronic kill switch</li><li><strong>Connectivity: </strong>1 x Thunderbolt 4 USB Type-C, 1 x USB-C 3.2 Gen 2, 4 x USB-A 3.2 Gen 1, HDMI 2.1, Ethernet, combo audio jack</li><li><strong>Networking: </strong>Wi-Fi 6E, Bluetooth 5.1</li><li><strong>Biometrics:</strong> None</li><li><strong>Battery capacity:</strong> 99 Watt-hours</li><li><strong>Dimensions: </strong>0.86 x 14.3 x 10.3 inches</li><li><strong>Measured weight: </strong>5.46 pounds (power brick weighs 2.65 pounds)</li><li><strong>Price</strong>: $2,175</li></ul>



<p>The Lenovo Legion Pro 7i Gen 8 starts at $2,070 for a system with the Intel Core i9-13900HX CPU, GeForce RTX 4070 graphics, 16GB of RAM, and a 512GB SSD. Our test system features two upgrades to the baseline model: 32GB of RAM that adds $55 and a 1TB SSD that adds $50. The highest-end model in the line costs $3,600 and features RTX 4090 graphics and a 2TB SSD. The Core i9-13900HX is the only CPU offered and all models feature the same 16-inch, 16:10 display with a 2560&times;1600 resolution and speedy 240Hz refresh rate.</p>



<h2 id="lenovo-legion-pro-7i-gen-8-per-key-rgb-and-full-size-arrow-keys">Lenovo Legion Pro 7i Gen 8: Per-key RGB and full-size arrow keys</h2>



<p>The Legion Pro 7i Gen 8 looks more like an overgrown corporate laptop than a gaming laptop until you fire up the RGB lighting. The aluminum chassis is dark gray throughout, and aside from a pair of small Lenovo badges and a larger Legion wordmark, there is a distinct lack of chrome accents. The large vents on the side edges and back edge are your only hints that this is a high-powered gaming laptop.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Lenovo Legion no lights" class="wp-image-1918725" height="900" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-no-lights.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>



<p>The laptop weighs 5.46 pounds, which is average for a 16-inch 16:10 laptop. The sleek Razer Blade 16 actually weighs slightly more at 5.52 pounds, while two other 16-inch 16:10 models, the Acer Predator Triton 500 SE at 5.29 pounds and the HP Victus 16 at 5.44 pounds, are a bit lighter. The Legion Pro 7i Gen 8&rsquo;s massive power brick, however, will weigh you down. The 300-watt brick weighs a hefty 2.65 pounds, making the overall travel weight a substantial eight pounds.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Lenovo Legion lid" class="wp-image-1918726" height="900" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-lid.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>



<p>The aluminum chassis feels fairly sturdy, although it does flex a bit in the middle of the keyboard. Mashing the WASD keys near the left edge felt more rigid than pressing keys closer to the middle of the keyboard, but there is definitely some flex to the keyboard deck. It lacks the rock-solid feeling of the Razer Blade 16. The keys themselves felt snappy, and I appreciate Lenovo finding room for both a number pad and four full-size arrow keys. It&rsquo;s a smart design choice to take advantage of the added space afforded by the tall 16:10 display and use it to extend the arrow keys.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Lenovo Legion RGB" class="wp-image-1918727" height="900" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-RGB.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>



<p>The Legion Pro 7i Gen 8 offers per-key RGB lighting, a fun feature that isn&rsquo;t always offered on a midrange gaming laptop. Most midrange models let you customize the look of the keyboard with various lighting patterns or perhaps with a four-zone lighting, but the Pro 7i Gen 8 provides maximum RGB flexibility with per-key lighting. You can set up to six RGB lighting profiles and you can cycle through them using the Function key and spacebar. There&rsquo;s also an LED stripe that runs along the front edge of the laptop that you can also customize with RGB lighting. It has six zones you can customize. The per-key lighting and LED stripe along the front edge go a long way to making the laptop look like a gaming model and not an overgrown ThinkPad.</p>



<h2 id="lenovo-legion-pro-7i-gen-8-big-bright-and-fast-display">Lenovo Legion Pro 7i Gen 8: Big, bright, and fast display</h2>



<p>The display is stellar, especially for a midrange model. It&rsquo;s big at 16 inches and has a 16:10 aspect ratio that&rsquo;s taller than a traditional 16:9 widescreen display. It&rsquo;s crisp with a 2560&times;1600 resolution that&rsquo;s finer than the 1920&times;1200 resolution found on many midrange 16-inch models. And it&rsquo;s fast and bright with a blazing 240Hz refresh rate and rated for 500 nits of brightness. My own measurements with a lux meter showed it was actually a bit brighter than its rating, reaching a peak brightness of 550 nits. Colors looked vivid, edges of images and text looked sharp, and games showed smooth movement.&nbsp;</p>



<p>The laptop features a modern 1080p camera that produces a crisp, well-balanced image. There&rsquo;s also a kill switch for the webcam on the laptop&rsquo;s left edge that interrupts the power to the camera to ensure your privacy when it&rsquo;s not in use.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Lenovo Legion side" class="wp-image-1918730" height="900" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-side.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>



<p>If the display has you dreaming of getting a premium gaming laptop AV system at a mainstream price, the speakers will snap you back to reality. Some higher-end 16-inch models such as the Razer Blade 16 find room for four speakers&mdash;two tweeters and two subs. You only get a pair of 2-watt speakers with the Legion Pro 7i Gen 8 and they produce muddy audio with no separation between the highs and mids. Without any subs, the bass response is predictably lacking.&nbsp;</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Lenovo Legion ports" class="wp-image-1918736" height="900" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-ports.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>



<p>The port selection is varied and well located. There are two USB-C ports, one of which offers Thunderbolt 4 support. There are four USB Type-A ports&mdash;two in the back and one of each side of the laptop. This USB-A arrangement allows left and right mousers to connect their gaming mouse to their preferred side. The audio jack is also conveniently located on the front half of the right side for each access. And with the speakers being what they are, you&rsquo;ll want to keep your headphones nearby.&nbsp;</p>



<h2 id="lenovo-legion-pro-7i-gen-8-performance">Lenovo Legion Pro 7i Gen 8: Performance</h2>



<p>Our Legion Pro 7i Gen 8 test system is based on the Core i9-13900HX CPU and GeForce RTX 4070 graphics. It also supplies a generous 32GB of RAM and a 1TB SSD. The 13th-gen Core i9-13900HX features Intel&rsquo;s hybrid architecture with performance and efficiency cores; it has eight performance cores, 16 efficiency cores, and a total of 32 processing threads. The RTX 4070 is a midrange GPU in Nvidia&rsquo;s latest GeForce 40 series behind the RTX 4080 and 4090 graphics processors. In our test system, it&rsquo;s set to run at its maximum of 140 watts. That&rsquo;s a combination of the GPU&rsquo;s maximum power draw of 115 watts and 25 watts supplied by the CPU via Dynamic Boost.</p>



<p>We started off testing with PCMark 10, which measures performance on everyday computing work including office productivity tasks, web browsing, and video chats. With a score approaching 8,000, the Legion Pro 7i Pro 8 proved itself to be overqualified as a productivity machine.&nbsp;</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Lenovo Legion PCMark" class="wp-image-1918743" height="619" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-PCMark10.jpg?quality=50&amp;strip=all" width="898" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>



<p>Our HandBrake benchmark tests how a laptop is able to handle crushing CPU loads over a lengthy period&mdash;in this case, transcoding a 30GB MKV file to a format suitable for Android tablets using HandBrake, the free video encoding utility. The Legion Pro 7i Gen 8 barely broke a sweat on the test, edging the Strix G18 as one of the fastest times we&rsquo;ve seen on the test. It can pull double duty as a gaming machine and content creation laptop.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Lenovo Legion Handbrake" class="wp-image-1918746" height="618" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-HandBrake.jpg?quality=50&amp;strip=all" width="898" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>



<p>Next up is Cinebench, another CPU-intensive test but one that renders a complex 2D scene over a short period of time. The trio of laptops with 13th-gen Core i9 chips crushed the competition, illustrating the power of Intel&rsquo;s latest generation of Core processors.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Lenovo Legion Cinebench" class="wp-image-1918747" height="619" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-Cinebench.jpg?quality=50&amp;strip=all" width="899" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>



<h2 id="lenovo-legion-pro-7i-gen-8-graphics-performance">Lenovo Legion Pro 7i Gen 8: Graphics performance</h2>



<p>Now we get to the goods&mdash;3D performance. First up are two synthetic tests, 3DMark&rsquo;s Time Spy and Port Royal. On Time Spy, the Legion Pro 7i Gen 8 trailed both RTX 4090-based laptops but edged the RTX 4070-based Asus ROG Strix G18 and a pair of laptops with previous-gen RTX 3080 Ti GPUs. On Port Royal, the results were largely the same, although the Legion Pro 7i Gen 8 finished in between the two RTX 3080 Ti laptops.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Lenovo Legion Time Spy" class="wp-image-1918755" height="619" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-3DM-Time-Spy.jpg?quality=50&amp;strip=all" width="897" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Lenovo Legion Port Royal" class="wp-image-1918756" height="619" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-3DM-Port-Royal.jpg?quality=50&amp;strip=all" width="920" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>



<p>On our real-world game benchmarks, the Legion Pro 7i Gen 8 started off with a bang, averaging 166 fps on our <em>Shadow of the Tomb Raider</em> benchmark at 1920&times;1080 resolution at the Highest quality preset. That was actually better than the RTX 4090-based MSI Titan GT 77 HX 13V and only four frames per second less than the RTX 4090-based Razer Blade 16. The two RTX 4090 machines were able to flex their muscles on the more demanding <em>Metro Exodus</em> test, and the Legion Pro 7i Gen 8&rsquo;s performance fell more in line with the other RTX 4070 laptop and the pair of RTX 3080 Ti systems.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Lenovo Legion Shadow of the Tomb Raider" class="wp-image-1918761" height="619" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-SoTR.jpg?quality=50&amp;strip=all" width="899" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Lenovo Legion Metro Exodus" class="wp-image-1918768" height="619" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-Metro-Exodus.jpg?quality=50&amp;strip=all" width="899" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>



<p>To test a laptop&rsquo;s battery life, we loop a 4K video using Windows 11&rsquo;s Movies &amp; TV app, with the laptop set to Airplane mode and earbuds plugged in. We set the screen brightness at a relatively bright 250 nits to 260 nits, which is a good brightness for watching a movie in an office with the lights on. Despite using a large, 99Whr battery, the Legion Pro 7i Gen 8 failed to last even five hours on our battery drain test. That&rsquo;s a short runtime even among gaming laptops, which rarely provide decent battery life. Then again, you are unlikely to lug this large, 16-inch laptop around with any regularity and will spend most of your time with it plugged in.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Lenovo Legion Battery Life" class="wp-image-1918779" height="618" src="https://b2c-contenthub.com/wp-content/uploads/2023/05/Legion-Pro-7-Gen-8-battery-life.jpg?quality=50&amp;strip=all" width="898" /></figure><p class="imageCredit">IDG / Matthew Elliott</p></div>



<h2 id="lenovo-legion-pro-7i-gen-8-should-you-buy-it">Lenovo Legion Pro 7i Gen 8: Should you buy it?</h2>



<p>Costs can quickly spiral out of control when shopping for a gaming laptop that offers the latest technology from Intel and Nvidia. The Lenovo Legion Pro 7i Gen 8 delivers the goods while staying on budget. It provides excellent value by pairing a powerful Core i9-13900HX CPU with not RTX 4080 or RTX 4090 graphics, but the more cost-effective RTX 4070 GPU. And its roomy, 16-inch 16:10 display is bright, sharp, and fast enough to extend the laptop&rsquo;s value even further. For a midrange gaming laptop, the rather staid design is sufficient. We&rsquo;d expect a more interesting and rigid enclosure for a higher-end gaming laptop, which is why we wouldn&rsquo;t recommend scaling up in the Legion Pro 7i Gen 8 line and choosing one of the pricier models with an RTX 4080 or RTX 4090 GPU. As configured, this machine is an excellent example of a mainstream gaming laptop that delivers for the price.</p>

Laptops</div>

## Get a lifetime of piano lessons for a special price
 - [https://www.pcworld.com/article/1919467/get-a-lifetime-of-piano-lessons-for-a-special-price.html](https://www.pcworld.com/article/1919467/get-a-lifetime-of-piano-lessons-for-a-special-price.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-05-19 08:00:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>You may have tried to learn the piano as a kid, but didn&rsquo;t like the teacher&rsquo;s musty living room and boring exercises you had to practice all the time. Fortunately, technology has advanced to make <a href="https://shop.pcworld.com/sales/skoove-premium-lifetime-subscription-2?utm_source=pcworld.com&amp;utm_medium=referral&amp;utm_campaign=skoove-premium-lifetime-subscription-2&amp;utm_term=scsf-571197&amp;utm_content=a0x1P000004IaerQAC&amp;scsonar=1" rel="noreferrer noopener" target="_blank">learning the piano</a> a lot more interesting and fun.</p>



<p>With Skoove, you&rsquo;ll join more than one million people enjoying interactive piano and keyboard lessons harnessing the power of artificial intelligence. This clever app shows you how to play your favorite songs &mdash; from John Legend to Beethoven &mdash; and adapts to give you individual feedback and a lesson plan specially designed for you. Whether you&rsquo;re just picking up notes, chords, and techniques or you&rsquo;re a more advanced player who wants to learn specific songs, Skoove lets you play your way.</p>



<p>Skoove has earned 4.4/5 stars on the Google Play Store and 4.5/5 stars on the App Store. Forbes writes, &ldquo;Unlike various other music-learning apps, Skoove&rsquo;s virtual guide takes the learner through each lesson, and provides real-time feedback that listens to the player as they practice.&rdquo;</p>



<p>Join the online piano-learning community. For a limited time, you can get a lifetime subscription to <a href="https://shop.pcworld.com/sales/skoove-premium-lifetime-subscription-2?utm_source=pcworld.com&amp;utm_medium=referral&amp;utm_campaign=skoove-premium-lifetime-subscription-2&amp;utm_term=scsf-571197&amp;utm_content=a0x1P000004IaerQAC&amp;scsonar=1" rel="noreferrer noopener" target="_blank">Skoove Premium Piano Lessons</a> for half off $300 at just $139.97.</p>



<p><a href="https://shop.pcworld.com/sales/skoove-premium-lifetime-subscription-2?utm_source=pcworld.com&amp;utm_medium=referral-cta&amp;utm_campaign=skoove-premium-lifetime-subscription-2&amp;utm_term=scsf-571197&amp;utm_content=a0x1P000004IaerQAC&amp;scsonar=1" rel="noreferrer noopener" target="_blank">&nbsp;</a></p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image"><img alt="" src="https://cdnp3.stackassets.com/1ad6ad71202f801107b0f2171004fac671228665/store/254301606a944dd211e1b71c1ce9c83309e06009354598654755a1184b46/product_323511_product_shots1.jpg" /></figure></div>



<p><strong>Skoove Premium Piano Lessons: Lifetime Subscription &ndash; $139.97</strong></p>



<p><a href="https://shop.pcworld.com/sales/skoove-premium-lifetime-subscription-2?utm_source=pcworld.com&amp;utm_medium=referral-cta&amp;utm_campaign=skoove-premium-lifetime-subscription-2&amp;utm_term=scsf-571197&amp;utm_content=a0x1P000004IaerQAC&amp;scsonar=1" rel="noreferrer noopener" target="_blank">See Deal</a></p>



<p>Prices subject to change.</p>

Entertainment</div>

