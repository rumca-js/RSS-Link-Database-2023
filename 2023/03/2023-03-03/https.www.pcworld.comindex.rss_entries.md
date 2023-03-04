# Source:PC world, URL:https://www.pcworld.com/index.rss, language:en-US

## An ultra-rare Radeon driver bug is breaking PCs. This exotic fix revived mine
 - [https://www.pcworld.com/article/1529986/rare-amd-radeon-driver-bug-corrupt-windows-fix.html](https://www.pcworld.com/article/1529986/rare-amd-radeon-driver-bug-corrupt-windows-fix.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-03-03 21:22:18+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>The carefully sequestered, rock-solid-reliable PC I use to test graphics cards became completely and utterly hosed this week. I couldn&rsquo;t even get the system to boot into Windows repair mode to try to troubleshoot it. The culprit? A rare bug in the way Windows interacts with AMD&rsquo;s latest WQHL-certified Radeon drivers, Adrenalin 23.2.2. Some quick Googling revealed that <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://wccftech.com/latest-amd-radeon-graphics-drivers-reportedly-causing-pc-boot-issues-corrupting-windows/amp/&amp;xcust=2-1-1529986-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">this has been happening to a small handful of other users</a> since Adrenalin 23.2.1 landed in mid-February, with similarly devastating effects.</p>



<p>This experience would be an absolute disaster for anyone who isn&rsquo;t the executive editor of a computer publication with a deep rolodex on hand (though <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://twitter.com/AzorFrank/with_replies&amp;xcust=2-1-1529986-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">AMD representatives are very responsive to driver feedback</a> on social media). But fortunately, I was able to work closely with AMD on on the issue. </p>



<p>AMD engineers not only managed to diagnose the potential root cause of this exotic bug, but also discovered a just-as-exotic troubleshooting workaround that helped revive my PC. A permanent fix is being investigated, but affected users can hopefully use this workaround to repair their systems without resorting to a full-blown fresh Windows install.</p>



<p>Here&rsquo;s what happened, <em>how</em> it happened, how you can avoid it, and how you can fix it if a similar disaster strikes your PC.</p>



<h2 id="how-amds-radeon-drivers-destroyed-my-windows-install">How AMD&rsquo;s Radeon drivers destroyed my Windows install</h2>



<p>I received a new custom Radeon RX 7900 XT for testing this week, so I went about my usual strict process for making sure the PC is up-to-date and ready to benchmark. Before swapping in a new graphics card or new drivers, while my existing stable setup is still intact, I perform several steps to make the system as &ldquo;like new&rdquo; as possible, to avoid potential issues caused by swapping in different GPUs from different brands. (The system hardware stays static, with minimal software installed beyond benchmarking tools, to ensure consistency.)</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="AMD Radeon RX 7900 XTX reveal" class="wp-image-1371299" height="800" src="https://b2c-contenthub.com/wp-content/uploads/2022/11/DSCF2136.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /><figcaption><p>This is a rig from AMD&rsquo;s Radeon RX 7900-series reveal, not my test system.</p></figcaption></figure><p class="imageCredit">Adam Patrick Murray / IDG</p></div>



<p>I already had a GeForce RTX 4070 Ti set up to give <a href="https://www.pcworld.com/article/1525299/nvidia-rtx-video-super-resolution-tested.html">Nvidia&rsquo;s awesome RTX Video Super Resolution</a> a whirl. With it installed, I manually updated Windows 10. Then, I powered down the system and replaced the 4070 Ti with the Radeon RX 7900 XT. It booted up normally. I then used Windows 10&rsquo;s Add and Remove Programs tool to uninstall all Nvidia software from my PC and rebooted. Standard stuff. I then used the fantastic <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.guru3d.com/files-details/display-driver-uninstaller-download.html&amp;xcust=2-1-1529986-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">DDU Uninstaller tool</a> to ensure that Nvidia&rsquo;s bits were truly and completely eradicated, and rebooted. Everything went fine.</p>



<p>Then the problems started.</p>



<p>I opened up Chrome, navigated to AMD&rsquo;s website, and downloaded the WQHL-certified Adrenalin 23.2.2 drivers that the site recommended for a 7900 XT. Then I installed the driver, checking the box to perform a &ldquo;factory reset&rdquo; clean installation rather than an upgrade-in-place. It turns out that checking that box, done in conjunction with a silent Windows update occurring in the background without my knowledge, <em>probably </em>led to my rig&rsquo;s downfall. </p>



<p>Everything went well&mdash;until the software said I needed to reboot my PC to finish the driver installation. After restarting, my system hit the MSI BIOS splash page like normal, but the second it tried loading Windows it immediately suffered a Blue Screen of Death, flashing the &ldquo;Inaccessible Boot Device&rdquo; error code shown in the image in the tweet below (which is unrelated to this AMD issue). Ugh. The system then started an endless cycle of BSOD &gt; reboot &gt; BSOD &gt; reboot without kicking off automatic repair attempts or presenting me the usual Windows troubleshooting options.</p>



<figure class="wp-block-embed is-type-rich is-provider-twitter wp-block-embed-twitter"><div class="wp-block-embed__wrapper">
<blockquote class="twitter-tweet"><p dir="ltr" lang="en">How can I enter safe mode before booting in Windows 10? AFAIK You can do that in Windows 7.<br /><br />INACCESSIBLE_BOOT_DEVICE <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://t.co/3u9oQ5f0Kc&amp;xcust=2-1-1529986-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">pic.twitter.com/3u9oQ5f0Kc</a></p>&mdash; Tridashie (@Tridashie) <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://twitter.com/Tridashie/status/1198906836562272256?ref_src=twsrc%5Etfw&amp;xcust=2-1-1529986-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">November 25, 2019</a></blockquote>
</div></figure>



<p>I didn&rsquo;t have time to troubleshoot it so I powered down the system and tried again the next day. Same deal. I yanked out the custom Radeon RX 7900 XT I need to test and replaced it with <a href="https://www.pcworld.com/article/1431755/amd-radeon-rx-7900-xtx-radeon-rx-7900-xt-review-rdna-3.html">AMD&rsquo;s reference Radeon RX 7900 XT</a>. This time, after two BSOD &gt; reboot cycles, Windows attempted to automatically repair the system after the BIOS splash screen. Success! &hellip;or so I thought. But I was terribly, terribly wrong.</p>



<p>Instead of correcting the issue, selecting <em>Startup Repair</em> made it even worse. When it was done, the screen went dark and completely unresponsive (while still powered on). Now, whenever I tried to boot the computer, I saw the little &ldquo;Windows thinking about it&rdquo; circle spinning after the BIOS screen for a brief moment, then a return to the infinite blackness. My Windows install was hosed so hard that the BSOD crashes didn&rsquo;t even occur anymore, and I had no chance to try standard Windows troubleshooting efforts.</p>



<p>In desperation I tried replacing the Radeon RX 7900 XT with the <a href="https://www.pcworld.com/article/1444726/nvidia-geforce-rtx-4070-ti-review.html">RTX 4070 Ti</a> and an <a href="https://www.pcworld.com/article/1499123/intel-slashes-arc-a750-price-to-249-touts-substantial-gaming-improvements.html">Intel Arc A750</a>&mdash;GPUs I&rsquo;ve tested in the past two weeks, that worked reliably&mdash;but to no avail. </p>



<figure class="wp-block-embed is-type-rich is-provider-twitter wp-block-embed-twitter"><div class="wp-block-embed__wrapper">
<blockquote class="twitter-tweet"><p dir="ltr" lang="en">Be careful when you install the latest Adrenalin 23.2.1. Backup your data!<a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://twitter.com/hashtag/AMD?src=hash&amp;ref_src=twsrc%5Etfw&amp;xcust=2-1-1529986-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">#AMD</a> <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://twitter.com/hashtag/Driver?src=hash&amp;ref_src=twsrc%5Etfw&amp;xcust=2-1-1529986-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">#Driver</a> <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://t.co/dOVZSth7OQ&amp;xcust=2-1-1529986-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">https://t.co/dOVZSth7OQ</a></p>&mdash; CapFrameX (@CapFrameX) <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://twitter.com/CapFrameX/status/1625771928592998401?ref_src=twsrc%5Etfw&amp;xcust=2-1-1529986-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">February 15, 2023</a></blockquote>
</div></figure>



<p>Googling the issue surfaced <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://wccftech.com/latest-amd-radeon-graphics-drivers-reportedly-causing-pc-boot-issues-corrupting-windows/amp/&amp;xcust=2-1-1529986-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">this WCCFTech article</a> from mid-February along with plenty of other coverage, citing numerous user reports of Adrenalin 23.2.1 destroying their Windows installs. It is a deeply frustrating experience, and one that would be disastrous for a standard PC gamer. I tweeted about my woes and an AMD representative emailed me within minutes. Obviously, being the executive editor of PCWorld may fast-track me for a quick response (though again, <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://twitter.com/AzorFrank/with_replies&amp;xcust=2-1-1529986-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">AMD representatives are very responsive to driver feedback</a> on social media). In this case, my high-profile headaches managed to help AMD probe the core issue, so I can provide troubleshooting steps that worked for me <em>and </em>happily report that a permanent fix is being investigated.</p>



<h2 id="how-to-fix-radeon-drivers-corrupting-your-windows-install">How to fix Radeon drivers corrupting your Windows install</h2>



<p>We spent two days going through various troubleshooting fixes while AMD engineers tried reproducing and diagnosing the problem. Swapping GPUs, trying new monitors, yanking the display cable out at different times, clearing the CMOS, and ensuring UEFI was selected instead of CSM in the BIOS (it was!) all proved fruitless. </p>



<p>But this morning, AMD&rsquo;s team got back to me with another suggestion: When the BIOS splash screen is up right after turning on the PC, slam the power button to try to coax Windows into forcing an automatic recovery attempt. I tried it four times to no avail. I was told to keep it up, that it <em>would</em> work eventually. And after fifteen total tries, it did! </p>



<p>I&rsquo;m not sure what caused it to finally catch, but timing seemed to play a part in it. Hitting the power button while the BIOS keypress options were up simply turned off my PC immediately. Hitting it once the spinning &ldquo;Windows thinking&rdquo; icon appeared kept the PC on, but did nothing&mdash;my system simply black-screened again. But eventually, I managed to hit the power button in the split second between the BIOS options disappearing and the Windows circle appearing, and <em>that</em> managed to kickstart an automatic recovery attempt. </p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="Windows advanced repair options" class="wp-image-1531569" height="606" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/windows-automatic-repair.jpg?quality=50&amp;strip=all" width="1024" /><figcaption><p>You want to select the System Restore option and select a restore point from prior to the Windows corruption. Windows should automatically have created one just before installing the new GPU drivers.</p></figcaption></figure><p class="imageCredit">IDG</p></div>



<p><em>Success!</em></p>



<p>After Windows did its thing for a bit, I eventually wound up in the Windows recovery tools menu, able to restart my PC or select advanced options. I went into the advanced options&rsquo; troubleshooting menu and selected <em>System Restore</em>, since <em>Startup Repair </em>hosed my PC even worse before. I selected a restore point from mid-February, loaded it up, and after two agonizingly frustrating days, my test rig was back in action. If you&rsquo;ve suffered from the recent Adrenalin drivers corrupting your Windows install, try this process to hopefully get back on your feet.</p>



<p>But how did this happen, and how can you prevent it from happening to you? </p>



<h2 id="how-to-avoid-radeon-drivers-breaking-your-windows-install">How to avoid Radeon drivers breaking your Windows install</h2>



<p>AMD tells me it took dozens of attempts to recreate the issue in their labs due to its extreme rarity. On a call, one representative actually called me &ldquo;patient zero.&rdquo; The company provided me with the following statement while its investigation is ongoing:</p>



<blockquote class="wp-block-quote"><p>&ldquo;We have reproduced an issue that can occur in an extremely small number of instances if a PC update occurs during the installation of AMD Software: Adrenalin Edition, and we are actively investigating. We recommend users ensure all system updates are applied or paused before installing the driver, and that the &ldquo;Factory Reset&rdquo; option is unchecked during the AMD driver installation process. We are committed to resolve issues as quickly as possible and strongly encourage users to submit issues with AMD Software: Adrenalin Edition via the Bug Report Tool.&rdquo;</p></blockquote>



<p>It&rsquo;s worth noting that my version of Windows 10 was updated prior to attempting the Adrenalin Software install, but the Game Bar or some other part of Windows may have been silently updating in the background to kickstart this disaster.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="AMD Adrenalin Software install" class="wp-image-1531567" height="717" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/amd-adrenalin-factory-install.jpg?quality=50&amp;strip=all" width="1024" /><figcaption><p>DO NOT click &ldquo;additional options&rdquo; and check the &ldquo;factory reset&rdquo; box until the core issue is fixed!</p></figcaption></figure><p class="imageCredit">AMD</p></div>



<p>As a workaround, simply don&rsquo;t check that factory reset box if you&rsquo;re installing new Radeon drivers. There&rsquo;s no reason to do so if you&rsquo;ve already got a working Radeon GPU set up and are simply updating to the latest drivers anyway. Simple as that. It worked for me after my test system was revived and I now have Adrenalin 23.2.2 installed and working like a charm.</p>



<h2 id="a-damned-shame">A damned shame</h2>



<p>It&rsquo;s a damned shame this happened. Most excruciatingly for myself and other gamers who had their Windows install deeply corrupted, of course, but also for AMD.</p>



<p>I&rsquo;ve been a <a href="https://www.pcworld.com/article/403045/amd-radeon-software-adrenalin-2019-update.html">vocal advocate</a> for the serious driver and software improvements AMD has been making over the last half-decade or so. People slammed the iffy state of Radeon drivers for years. AMD listened and poured tremendous investment and effort into polishing them up. Now, Team Red&rsquo;s drivers are even better than Nvidia&rsquo;s popular Game Ready drivers in many ways, and in June 2022 AMD felt confident enough about its software to <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://community.amd.com/t5/gaming/stability-performance-and-great-experiences-with-amd-software/ba-p/530424&amp;xcust=2-1-1529986-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">declare</a> that it offers &ldquo;industry-leading stability&rdquo; with &ldquo;99.95% of users experiencing no crashes when AMD Software is installed.&rdquo; </p>



<p>There&rsquo;s no doubt that AMD&rsquo;s driver stability and overall stability are now right up there with the best of them after years of intense refinement. This is an extremely unusual edge case. It sure sucks being in that 0.05%! But issues <em>this</em> catastrophic hurt the cause to rebuild Radeon software&rsquo;s image, no matter how rare they are. Regardless of whether Windows or AMD is to blame in the end, this experience is the sort of thing that would immediately make many PC gamers swear off Radeon GPUs forever, and tell all their friends why. And that&rsquo;s a shame.</p>



		<div class="wp-block-product-widget-block product-widget">
			<div class="product-widget__block-title-wrapper">
				<h4 class="product-widget__block-title" id="this-remains-the-best-1080p-graphics-card-for-most-people">
					This remains the best 1080p graphics card for most people				</h4>
			</div>

			<div class="product-widget__content-wrapper">
									<div class="product-widget__title-wrapper">
						<h3 class="product-widget__title" id="radeon-rx-6600-swft-210">Radeon RX 6600 Swft 210</h3>
					</div>
				
									<div class="product-widget__image-outer-wrapper">
						<div class="product-widget__image-wrapper">
							<img alt="Radeon RX 6600 Swft 210" class="product-widget__image" height="1667" src="https://b2c-contenthub.com/wp-content/uploads/2021/10/XFX-Radeon-RX-6600-Swft-210-8.jpg?quality=50&amp;strip=all" width="2500" />
						</div>
					</div>
				
									<div class="review product-widget__review-details">
													<div class="product-widget__rating-and-review-link">
								<div class="product-widget__review-details--rating">
											<div class="starRating"></div>
										</div>									<a class="product-widget__review-link" href="https://www.pcworld.com/article/543823/amd-radeon-rx-6600-review-finally-a-true-1080p-graphics-card.html" target="_blank">Read our review</a>
									
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

		


<p>Several Radeon GPUs hold spots in our roundup of <a href="https://www.pcworld.com/article/416006/the-best-graphics-cards-for-pc-gaming.html">the best graphics cards</a>. I&rsquo;m not going to remove them despite my personal disaster. This severe issue isn&rsquo;t widespread, only occurring in ultra-rare circumstances, while AMD offers truly compelling value up and down the stack with Nvidia hiking GeForce prices through the roof. And yes, AMD&rsquo;s drivers are indeed rock-solid the <em>vast</em> majority of the time. This particular scenario could have been catastrophic without AMD&rsquo;s direct help, but no software is perfect&mdash;especially in the complex PC ecosystem&mdash;and while I got stuck in a deeply frustrating situation, there&rsquo;s only a microscopic chance of it affecting <em>you</em>. (And hopefully this article can help you if it does.)</p>



<p>Most people don&rsquo;t check the factory install box anyway. Just be sure you don&rsquo;t either until a permanent fix is released. </p>

Graphics Cards</div>

## The Full Nerd ep 248: Ryzen 9 7950X3D and the state of PC gaming
 - [https://www.pcworld.com/article/1528516/the-full-nerd-ep-248-ryzen-9-7950x3d-and-state-of-pc-gaming.html](https://www.pcworld.com/article/1528516/the-full-nerd-ep-248-ryzen-9-7950x3d-and-state-of-pc-gaming.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-03-03 20:00:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>In this episode of The Full Nerd, <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://twitter.com/Gordonung&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Gordon Ung</a>, special guest <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://twitter.com/bradshoemaker&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Brad Shoemaker</a> of the <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://podcasts.apple.com/us/podcast/the-nextlander-podcast/id1570737028&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Nextlander </a>podcast, and <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://twitter.com/morphingball&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow"></a><a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://twitter.com/AdamPMurray&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Adam Patrick Murray</a> get nerdy about <a href="https://www.pcworld.com/article/1524570/amd-ryzen-9-7950x3d-review-v-cache.html">Ryzen 9 7950X3D reviews</a> and the state of PC gaming.</p>



<p>Longtime games journalist and Ryzen X3D-curious podcaster Brad Shoemaker joins us to go over the launch of AMD&rsquo;s long-awaited Ryzen 9 7950X3D CPU. The crew discusses why the Internet is so aggro about it, and <a href="https://www.pcworld.com/article/1528458/three-ryzen-9-7950x-misconceptions-debunked.html">debunks some misconceptions</a> about it. Gordon graphically shows you the vaunted Ryzen 7 5800X3D&rsquo;s biggest weaknesses against the new Ryzen 9 7950X3D, too. Gordon also discloses why he tested the Intel CPU at DDR5/6000 rather than with higher clocked RAM, which has some Intel fans screaming foul.</p>



<p>As a long-time games journalist, Brad gives us insight into the state of the industry, the console wars, and the PC vs. console. Brad also shares his thoughts on industry consolidation and whether it&rsquo;s good or bad.</p>



<figure class="wp-block-embed is-type-video is-provider-youtube wp-block-embed-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">

</div></figure>



<p>You can witness it all in the video embedded above. You can also watch&nbsp;<a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.youtube.com/watch?v=PIJ8QiHsOAc&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">The Full Nerd episode 248</a><a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://youtu.be/z7GxJ8Uku_Y&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">0 on YouTube</a>&nbsp;(subscribe to the channel while you&rsquo;re there!) or listen to it on Megaphone.fm if you prefer the audio alone.&nbsp;</p>








<p>Speaking of audio, you can subscribe to The Full Nerd&nbsp;in&nbsp;<a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://itunes.apple.com/us/podcast/the-full-nerd/id1113193062?mt=2&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">iTunes</a>&nbsp;(please leave a review if you enjoy the show). We&rsquo;re also on&nbsp;<a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://pca.st/ggAZ&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Pocket Casts</a>,&nbsp;<a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://podcasts.google.com/feed/aHR0cHM6Ly9mZWVkcy5tZWdhcGhvbmUuZm0vSURHODkzNTMwMDk1OQ&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Google Podcasts</a>,&nbsp;<a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://open.spotify.com/show/71KPlf1jOh1Z0KHZrHjir2?si=k1bakTv7T3aDRg9YcQrZbw&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Spotify</a>, or you can point your&nbsp;favorite&nbsp;podcast-savvy RSS reader to:&nbsp;<a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://feeds.megaphone.fm/IDG8935300959&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">https://feeds.megaphone.fm/IDG8935300959</a></p>



<p>If you want to wear your geekiness on your sleeve, check out <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://crowdmade.com/collections/pcworld&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">our Full Nerd merch</a>! We just rolled out some new designs so you can proudly proclaim that you&rsquo;re a friend of the show, or your love of 19&times;10 gaming. (If you know, you know.)</p>



<p>Have a PC- or gaming-related question? Email&nbsp;<a href="mailto:thefullnerd@pcworld.com">thefullnerd@pcworld.com</a>&nbsp;and we&rsquo;ll try to answer it in the next episode. You can also join the PC-related discussions and ask us questions on&nbsp;<a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://discordapp.com/invite/SGPRSy7&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">The Full Nerd&rsquo;s Discord server</a>.&nbsp;Finally, be sure to follow&nbsp;PCWorld&nbsp;on&nbsp;<a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.facebook.com/PCWorld/&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Facebook</a>,&nbsp;<a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.youtube.com/user/PCWorldVideos&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">YouTube</a>, and&nbsp;<a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.twitch.tv/PCWorldUS&amp;xcust=2-1-1528516-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Twitch</a>&nbsp;to watch future&nbsp;episodes&nbsp;live and pick our brains in real time!&nbsp;</p>

CPUs and Processors</div>

## Windows 11’s lackluster volume mixer is getting a serious upgrade
 - [https://www.pcworld.com/article/1531212/windows-11s-new-volume-panel-is-super-helpful.html](https://www.pcworld.com/article/1531212/windows-11s-new-volume-panel-is-super-helpful.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-03-03 16:39:09+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>Sound controls in Windows have always left something to be desired, often forcing you to dive into sub-menus to change audio output devices or adjust volume for specific programs. According to the Windows Insider Blog, that&rsquo;s going to change soon. The latest Windows 11 Insider Build includes a completely redesigned volume panel, with a variety of complex tools available in a single click. </p>



<p>The <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://blogs.windows.com/windows-insider/2023/03/02/announcing-windows-11-insider-preview-build-25309/&amp;xcust=2-1-1531212-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">new version of the tool</a> allows you to click the volume icon in the notification area, then instantly bring up a mini-menu. This includes sections for the output device (great for quickly swapping between speakers and a headset), different options for Spatial Audio, and individual volume sliders to both the master volume control and individual Windows apps. The specific volume panel is also available via a new keyboard shortcut, <em>Win + Ctrl + V</em>. </p>



<p>At the moment Windows 11 requires three clicks to change an output device, and you have to dive into the full Sound Settings portion of the main menu and click the Volume Mixer to adjust individual apps. The updated interface is a huge improvement &mdash; something I&rsquo;ve been wanting for years, and doing myself with third-party apps like <a href="https://www.pcworld.com/article/547570/my-5-favorite-free-power-user-tools-for-windows.html" rel="noreferrer noopener" target="_blank">SoundSwitch</a> (one of the <a href="https://www.pcworld.com/article/547570/my-5-favorite-free-power-user-tools-for-windows.html">5 free Windows power user tools we can&rsquo;t live without</a>). The changes are visible in Windows Preview Build 25309, and should hopefully hit the Windows 11 general release sometime later this year. </p>

Windows</div>

## Amazon Basics house brand enters the PC parts market
 - [https://www.pcworld.com/article/1531055/amazon-basics-house-brand-enters-the-pc-parts-market.html](https://www.pcworld.com/article/1531055/amazon-basics-house-brand-enters-the-pc-parts-market.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-03-03 15:32:38+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>Great Value, Kirkland, Signature Select, Husky &mdash; house brands, copied or repackaged products sold under a store&rsquo;s own label as cheap alternatives to name brands, have a long and storied history at retail. But perhaps no company has embraced the idea as completely and ruthlessly as Amazon has in the digital age. The corporation&rsquo;s Amazon Basics brand will sell you everything from diapers to dining sets, and now it&rsquo;s expanding into desktop PC components. </p>



<p>The first individual computer part to get the Amazon Basics label is a CPU cooler, a rather unassuming little number <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/B09R4MDLMM?&amp;xcust=2-1-1531055-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">selling for $26.99 in the US</a>. It boasts a relatively compact design for full-sized desktops, with four heat pipes and a single RGB 2000RPM 100mm cooling fan. It&rsquo;s compatible with the latest Intel and AMD CPU sockets: LGA 1700, 1200, 1156, 1155, 1151, 1150, plus AM4 and AM5. There&rsquo;s even a handy installation video for both motherboard types, with and without RGB headers. </p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Amazon Basics CPU cooler screenshot" class="wp-image-1531158" height="775" src="https://b2c-contenthub.com/wp-content/uploads/2023/03/amazon-cooler-screenshot.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">Amazon</p></div>



<p>Eagle-eyed readers might think the design looks a little familiar. As noted by <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.tomshardware.com/news/amazon-basics-cpu-cooler-is-its-first-foray-into-pc-components&amp;xcust=2-1-1531055-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Tom&rsquo;s Hardware</a>, the cooler appears to be either a rebadged version of the <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.coolermaster.com/catalog/coolers/cpu-air-coolers/hyper-h410r-rgb/&amp;xcust=2-1-1531055-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Cooler Master H410R</a>, or a basically perfect copy of the design, minus some cosmetic badges and about 10mm in height. Neither move would be unprecedented for Amazon. The company has previously gone directly to Chinese white box manufacturers for rebadged products, similar to retail store brands all over the world. And it&rsquo;s also commissioned flagrant copies of name-brand products, as in the case of <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://petapixel.com/2021/03/03/peak-design-calls-out-amazon-for-copycatting-the-everyday-sling-bag/&amp;xcust=2-1-1531055-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Peak Design&rsquo;s EveryDay Sling bag</a>. </p>



<p>While the Amazon Basics Computer Cooling Fan is <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/B0821GBNHM/?th=1&amp;xcust=2-1-1531055-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">less than half the price of the H410R on Amazon</a>, it&rsquo;s hardly the only option in its price range. Single-fan coolers from <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/B084P82HRY/&amp;xcust=2-1-1531055-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Arctic</a>, <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/B08YRN1621/?th=1&amp;xcust=2-1-1531055-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Be Quiet</a>, <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/B09XFKW431/&amp;xcust=2-1-1531055-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Thermaltake</a>, and <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/B017EVR67W/&amp;xcust=2-1-1531055-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Zalman</a> meet or beat its price, as do several entries from the usual weirdo brands that exist only on Amazon and other drop shipping sites. We may or may not see Amazon offer a further variety of PC components under the Amazon Basics brand &mdash; that will probably be decided by some maddeningly complex internal sales algorithm that man was not meant to wot of. </p>

Computer Components</div>

## OWC Thunderbolt Go Dock review: Big, pricey, ambitious
 - [https://www.pcworld.com/article/1519567/owc-thunderbolt-go-dock-review.html](https://www.pcworld.com/article/1519567/owc-thunderbolt-go-dock-review.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-03-03 15:30:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>


<div class="review" id="review-body"><span class="review-title">At a glance</span><h3 class="review-subTitle" id="experts-rating">Expert's Rating</h3><div class="starRating"></div>
<div><div class="review-columns"><div class="review-column"><h3 class="review-subTitle" id="pros">Pros</h3><ul class="pros review-list"><li>Power brick is hidden within, removing clutter</li><li>90W to charge your laptop</li><li>Supplies a terrific 9.5W for smartphone charging</li><li>HDMI 2.1 support</li></ul></div><div class="review-column"><h3 class="review-subTitle" id="cons">Cons</h3><ul class="cons review-list"><li>Ethernet is glitchy, and requires a driver</li><li>Bulky</li><li>Expensive</li><li>Limited built-in display options</li></ul></div></div></div><h3 class="review-subTitle review-subTitle--borderTop" id="our-verdict">Our Verdict</h3><p class="verdict">OWC&rsquo;s Thunderbolt Dock Go integrates the power brick, and that&rsquo;s worth something. But this Thunderbolt 4 dock ends up big, bulky, and expensive as a result.</p>
</div>
				<h3 class="review-best-price" id="best-prices-today-owc-thunderbolt-go-dock">
			Best Prices Today: OWC Thunderbolt Go Dock		</h3>
				<div class="wp-block-price-comparison price-comparison ">
			<div class="price-comparison__record price-comparison__record--header">
				<div>
					<span>Retailer</span>
				</div>
				<div class="price-comparison__price">
					<span>Price</span>
				</div>
			</div>

														<div class="price-comparison__record">
							<div class="price-comparison__image">
																	<span>OWC</span>
															</div>
							<div class="price-comparison__price">
								<span>$349.99</span>
							</div>
							<div>
								<a class="price-comparison__view-button" href="https://www.kqzyfj.com/click-8200811-11911660?sid=2-1-1519567-2-1519550-12028&amp;url=https://eshop.macsales.com/shop/owc-thunderbolt-go-dock" rel="nofollow" target="_blank">View Deal</a>							</div>
						</div>
												<div class="price-comparison__record price-comparison__record--footer">
					<span class="price-comparison__footer-text">
													Price comparison from over 24,000 stores worldwide												</span>
									</div>
						</div>
		


<p>OWC&rsquo;s Thunderbolt Go Dock has a unique selling point in its favor: the lack of an external power brick. This helps reduce cable clutter and, in theory, makes it easier to take this Thunderbolt 4 dock on the go. Unfortunately, it doesn&rsquo;t quite achieve its promise.</p>



<p>Like laptops, Thunderbolt docks can include fairly sizeable power bricks&mdash;often weighing about as much as the dock itself. Yet desktop PCs and some game consoles manage to integrate the power transformer inside the chassis itself, providing a cleaner, more streamlined look.</p>



<blockquote class="wp-block-quote"><p><em>Note: See our roundup of the <a href="https://www.pcworld.com/article/393714/best-thunderbolt-docks-for-a-laptop-pc.html">best Thunderbolt docks</a> to learn about competing products, what to look for in a Thunderbolt dock, and buying recommendations.</em></p></blockquote>



<h2 id="owc-thunderbolt-go-dock-features">OWC Thunderbolt Go Dock: Features</h2>



<p>You can make the case that the OWC Thunderbolt Go Dock combines the best of both worlds: All there is in the box is the 28-inch Thunderbolt 4 cable, the power cable, and the dock itself. If OWC included a small pouch that the items could be kept in, you could make the case that this is a travel dock. Regardless, the lack of additional cabling is a selling point in its favor. </p>



<p>OWC has traditionally served the Mac market, which has used Thunderbolt as a direct display interface as much as an I/O expansion cable. In addition to a single HDMI 2.1 port, the Dock Go provides two downstream Thunderbolt 4 ports, as well as the Thunderbolt 4 connection to the host PC. Those additional downstream ports can be used as display connections, though you&rsquo;ll need to pay an additional $20 or so for a <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/uni-Thunderbolt-Compatible-MacBook-Surface/dp/B075V5JK36/?th=1&amp;xcust=2-1-1519567-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Thunderbolt 4-to-USB-C cable</a> or a similar DisplayPort cable. In fact, we used such a cable to drive a second 4K display at 60Hz, verifying that the Dock Go&rsquo;s bandwidth works as advertised. </p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="OWC Thunderbolt Dock Go" class="wp-image-1520953" height="587" src="https://b2c-contenthub.com/wp-content/uploads/2023/02/OWC-Thunderbolt-Go-Dock-front.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /><figcaption>The front of the OWC Thunderbolt Go Dock includes well-labeled ports, including a USB-C port to charge a smartphone.</figcaption></figure><p class="imageCredit">Mark Hachman / IDG</p></div>



<p>It&rsquo;s worth noting that the single HDMI 2.1 port is really unusual&mdash;the massive bandwidth it provides technically allows for a single 10K display at 120Hz, which is certainly beyond today&rsquo;s available hardware. </p>



<p>Additional ports include a legacy 5Gb/s USB-A port, a 10Gb/s USB-C port, an audio jack, and an SD 4.0 UHS-II card slot on the front; on the back, the dock includes the two Thunderbolt 4 ports, the HDMI port, a 2.5Gb/s ethernet port, and a pair of 10Gb/s USB-A ports. The dock delivers 90W of charging power downstream via the Thunderbolt 4 cable, which snakes out from the side of the dock.</p>



<figure class="wp-block-pullquote"><blockquote><p>OWC&rsquo;s Thunderbolt Go Dock connected to two 4K displays perfectly; same for a single 4K display and a 1440p widescreen display at 100Hz. </p></blockquote></figure>



		<div class="wp-block-product-chart product-chart">
				</div>

		


<p>In my experience, the USB-A ports on the rear of the dock accommodated a few random USB keys and other devices, but they&rsquo;re closely spaced. If you have an oddly shaped promotional dongle, for example, it may not fit. You can use the front-facing port instead.</p>



<p>Despite its &ldquo;Thunderbolt Dock Go&rdquo; name, OWC&rsquo;s dock isn&rsquo;t small; at 9.5 inches long and 3.6 inches deep, it&rsquo;s larger than you might expect. It also weighs 2.09 pounds, which is about a pound less than a typical laptop weighs. The aluminum chassis does a great job of dissipating heat, so that the dock never heated up beyond a slightly warm temperature in my tests.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="OWC Thunderbolt Dock Go" class="wp-image-1520954" height="501" src="https://b2c-contenthub.com/wp-content/uploads/2023/02/OwC-Thunderbolt-Go-dock-rear.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /><figcaption>The rear of the OWC Thunderbolt Dock Go. We think that the USB-A ports are spaced a bit too tightly together in some cases, but USB cables should have no problems fitting. </figcaption></figure><p class="imageCredit">Mark Hachman / IDG</p></div>



<h2 id="owc-thunderbolt-go-dock-performance">OWC Thunderbolt Go Dock: Performance</h2>



<p>Although OWC doesn&rsquo;t list smartphone charging as a selling point, the dock certainly does generate enough power to fast-charge a smartphone: 9.5W from the front-facing USB-C port, and about 12W if you use one of the rear Thunderbolt ports for the same purpose. Otherwise, the USB-A ports produce about 2.5W, just enough to charge a smartphone over several hours. </p>



<p>OWC&rsquo;s Thunderbolt Go Dock connected to two 4K displays perfectly; same for a single 4K display and a 1440p widescreen display at 100Hz. OWC&rsquo;s Thunderbolt Go Dock initially passed our streaming performance tests with flying colors, streaming our 4K60 test video over its integrated ethernet without dropping any frames. </p>



<p>In part, that&rsquo;s because YouTube streamed the video at a lower bitrate than we expected. The reason for that became apparent: Though the dock&rsquo;s ethernet port lit up correctly, all of the data was being passed via Wi-Fi, even with the ethernet cable inserted. OWC support referred us to a Realtek Ethernet software driver, but even after installing it, rebooting, disconnecting the dock, and running a diagnostic program, ethernet still failed to work correctly. Inexplicably, it did work a reboot or two later. After doing so, the dock allowed reads and writes at expected speeds on our SSD while streaming video.</p>



<h2 id="should-you-buy-the-owc-thunderbolt-go-dock">Should you buy the OWC Thunderbolt Go Dock?</h2>



<p>The OWC Thunderbolt Dock Go is probably a little too big and heavy to tote along on a business trip, but it <em>is</em> possible. It appears that you&rsquo;ll need to install a software driver to enable ethernet, however, if and when that driver eventually works. And at a $349 MSRP, you&rsquo;ll pay for the privilege. We certainly appreciate what OWC set out to do here with the Thunderbolt Dock Go, but its size, price, and driver issue mean that it falls a bit short of an Editor&rsquo;s Choice award.</p>

Computer Accessories</div>

## Nab this colorful retro keyboard and mouse combo for just $35
 - [https://www.pcworld.com/article/1531040/1531040.html](https://www.pcworld.com/article/1531040/1531040.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-03-03 14:48:31+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>Okay, so, this retro wireless and keyboard mouse combo stopped me dead in my tracks this morning. It&rsquo;s so unique and gorgeous, if I wasn&rsquo;t so emotionally attached to my mechanical keyboard, I&rsquo;d swoop this one up in a heartbeat. Amazon&rsquo;s selling the <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/B09XB4NMNX&amp;xcust=2-1-1531040-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">KNOWSQT wireless keyboard and mouse combo for just $35.19</a>, which is 20 percent off of the original price. That&rsquo;s an amazing value right there. Heck, the mouse is even DPI adjustable.</p>



<p>The keyboard itself features a floating button design, which mimics the feel of an old typewriter. The keycaps are detachable, making them easy to clean. Plus, the colorful keycaps are just plain fun and will surely brighten up your desk space. As for the plug-and-play mouse, it has a working range of 35 feet. You don&rsquo;t have to install additional software in order to use it, either. Both peripherals are also compatible with PC and Mac. </p>



<p>This is an awesome deal. Whether you&rsquo;re looking to save some money or add a pop of color to your desk, this combo is well worth considering.</p>


<p class="cta wp-block wp-block-button"><a class="cta__btn" href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/B09XB4NMNX&amp;xcust=2-1-1531040-7-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Get the KNOWSQT wireless keyboard and mouse combo for $35.19 on Amazon</a></p>
Keyboards</div>

## Avast One review: Well-priced PC security with excellent protection
 - [https://www.pcworld.com/article/548703/avast-one-review-its-new-well-priced-and-looks-good.html](https://www.pcworld.com/article/548703/avast-one-review-its-new-well-priced-and-looks-good.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-03-03 11:45:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>


<div class="review" id="review-body"><img alt="Editors' Choice" class="review-logo" src="https://www.pcworld.com/wp-content/uploads/2021/09/PC-ED-CHOICE.png" /><span class="review-title">At a glance</span><h3 class="review-subTitle" id="experts-rating">Expert's Rating</h3><div class="starRating"></div>
<div><div class="review-columns"><div class="review-column"><h3 class="review-subTitle" id="pros">Pros</h3><ul class="pros review-list"><li>Good new design</li><li>Well priced</li><li>Excellent performance</li></ul></div><div class="review-column"><h3 class="review-subTitle" id="cons">Cons</h3><ul class="cons review-list"><li>Smart scan requires too much user intervention</li><li>Avast asks to install Google Chrome</li></ul></div></div></div><h3 class="review-subTitle review-subTitle--borderTop" id="our-verdict">Our Verdict</h3><p class="verdict">Avast One is a much needed improvement with excellent pricing, and all the features you&rsquo;ve come to expect from this premium suite. Both the Individual and Family plans are well worth a look for anyone looking for a solid third-party security suite.</p>
</div>


<p><em>Editor&rsquo;s note: This review was updated on 3/3/23 to update pricing and plan details, as well as third-party test results.</em></p>



<p>There are two things Avast&rsquo;s paid security suites have been known for besides solid protection: good design and high prices. That&rsquo;s changing a little bit, and for the better, with Avast One, the company&rsquo;s new top-tier product. Avast still offers a free version, Avast One Essential, as well as a Premium Security product that has fewer features but covers double the number of devices (10 instead of 5) but Avast One is the sweet (suite?) spot, with solid antivirus, some useful extra features, and multi-device coverage. Plus the pricing has improved over the years. </p>



<figure class="wp-block-pullquote"><blockquote><p>Avast One is a very good security suite. The price is right, and its protection is excellent.</p></blockquote></figure>



<blockquote class="wp-block-quote"><p><em>Note: This review is part of our&nbsp;<a href="https://www.pcworld.com/article/3219792/computers/best-antivirus-for-windows-pc.html">best antivirus </a><a href="https://www.pcworld.com/article/3219792/computers/best-antivirus-for-windows-pc.html">roundup</a>. Go there for details about competing products and how we tested them.</em></p></blockquote>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large is-resized"><img alt="avast one dashboard with a thumbs up indicating the PC is healthy" class="wp-image-548825" height="440" src="https://b2c-contenthub.com/wp-content/uploads/2021/11/AvastOneLooks-Good.png?w=1200" width="684" /></figure><p class="imageCredit">IDG</p></div>



<p>Avast One includes an entirely new desktop app. Gone are the blue and purple tones, and the orange splotch logo. In place of all that, you get a more subdued aesthetic, with a lot of whites and lightly shaded colors, accented by a bolder, and easily spotted blue for the interface buttons. </p>



<p>The left rail has four simple menu items: <em>Home</em>, <em>Explore</em>, <em>Messages</em>, and <em>Account</em>. This makes Avast One look deceivingly simple, but there are a ton of features once you start digging in. </p>



<p>The first time you fire up Avast One it asks to run a smart scan, a common feature in a number of antivirus suites. Smart Scans combine a security scan with scans for other problems such as browser trackers and an excess of temporary files. The basic idea is to clean up your PC and keep it running smoothly, as opposed to just scanning for malware. </p>



<p>This is a good idea since many top suites come with PC cleaning and maintenance utilities, but often require you to activate them. A smart scan gets you to use at least some of these capabilities, which is important considering some of them used to cost extra and now are just included in the suite. The one issue with Avast&rsquo;s approach is that it does the scan in three stages: browser threats, viruses &amp; malware, and PC cleaning. That&rsquo;s fine, but it requires user intervention to initiate each phase instead of just plowing through the entire scan and delivering a report at the end. The constant requirement to continue at the end of each phase gets a little annoying. Not a deal breaker, but this could be handled better.</p>



<p>While the smart scan is the primary scan Avast asks you to do, scroll down Avast One&rsquo;s Home page and you get shortcuts to run a deep scan, a targeted scan on a specific folder or set of folders, initiate a VPN scan, or use the PC optimization tools.</p>



<p>Moving on to <em>Explore</em> you get into the meat of Avast One&rsquo;s features. <em>Explore</em> is really more of a launchpad for all the deeper controls of the security suite. For example, under <em>Explore</em> you have <em>Scan Center</em>, which has its own screen and includes the controls for all the types of scans you want. This includes the types of scans we&rsquo;ve already talked about, as well as a boot-time scan. You can also save scans in the <em>Custom Scans</em> section if there&rsquo;s a type of scan you want to run repeatedly. This is also the section where you can schedule scans, such as running a deep scan once a month, and perform a quick scan every day. </p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large is-resized"><img alt="avast one's Explore section which houses all of the security suite's features" class="wp-image-548826" height="466" src="https://b2c-contenthub.com/wp-content/uploads/2021/11/AvastOneExplore.png?w=1200" width="699" /><figcaption>Avast One&rsquo;s <em>Explore</em> section.</figcaption></figure><p class="imageCredit">IDG</p></div>



<p>Other key security features inside <em>Explore</em> include file shield for monitoring changes to files for malicious behavior, ransomware protection, web shield for staying safe online, a firewall allowing you to block internet access on a per-app basis, webcam protection, and a number of other features. </p>



<p>The firewall is particularly nice since it offers customizable security in a very simple interface. It&rsquo;s not the most advanced firewall you can find, but it&rsquo;s a firewall that even non-techies can use if they feel the need. For paid users, the firewall hides key identifiers of your PC from other devices on the same network such as the PC&rsquo;s name and the type of device. If another device starts doing a port scan on your PC, the firewall will notify you, and it&rsquo;s built to deter man-in-the-middle attacks.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large is-resized"><img alt="avast one's scan center showing the various scans users can carry out." class="wp-image-548827" height="463" src="https://b2c-contenthub.com/wp-content/uploads/2021/11/AvastOneScanCenter.png?w=1200" width="712" /></figure><p class="imageCredit">IDG</p></div>



<p>Avast&rsquo;s built-in VPN allows unlimited bandwidth as part of the paid packages, with a wide range of country locations to choose from. Free users also aren&rsquo;t left out, with a solid 5GB per week. This is quite a switch from Avast&rsquo;s prior suites that wanted more money to use the VPN. The paid version supports peer-to-peer transfers, as well as streaming servers for viewing geo-restricted content. Avast can also automatically turn on the VPN when you do things like go to banking or shopping websites. Those are nice additions, though be aware that you really shouldn&rsquo;t be going onto a banking website over Wi-Fi on a network you don&rsquo;t trust. </p>



<p>The paid version also has what is commonly called dark web monitoring but what Avast calls <em>Password Protection</em>. This feature alerts you if any of your passwords for online services ever get revealed in a data breach.</p>



<p>The other two parts of Avast One are for managing your account and receiving notifications from the company. That&rsquo;s it. The interface is far more simplified than it once was, and it already wasn&rsquo;t very complicated. This is an excellent design and is easily navigable by anyone from a grizzled PC veteran to a novice user.</p>



<h2 id="performance">Performance</h2>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large is-resized"><img alt="A notification in avast one with a pencil drawing of a smiling technician fixing a PC" class="wp-image-548828" height="457" src="https://b2c-contenthub.com/wp-content/uploads/2021/11/AvastOneDriverupdates.png?w=1200" width="712" /><figcaption>Avast One&rsquo;s messaging alerts you to actions that should be carried out.</figcaption></figure><p class="imageCredit">IDG</p></div>



<p>Testing house <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.av-test.org/en/antivirus/home-windows/&amp;xcust=2-1-548703-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">AV-Test</a> gave the free Avast One Essential, which uses the same detection engines as Avast One, a 100 percent score for protection against 0-day malware and widespread and prevalent malware, in its most recent December 2022 evaluation.</p>



<p><a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.av-comparatives.org/tests/malware-protection-test-september-2022/&amp;xcust=2-1-548703-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">AV-Comparatives&rsquo; September 2022 Malware Protection Test</a> found that Avast blocked 100 percent of threats from more than 10,000 samples. You can&rsquo;t get better than that.</p>



<p><a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.av-comparatives.org/tests/real-world-protection-test-july-october-2022/&amp;xcust=2-1-548703-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">AV-Comparatives&rsquo; real-world protection test</a> for July and August found that Avast blocked 100 percent of threats from 626 samples. Again, top of the pack.</p>



<p>For our in-house hardware performance tests, we found that Avast had no real performance impact on our large file transfer test, archiving test, and the Handbrake encoding test. The only noticeable change is that unzip times were actually a little bit faster at just under 7 minutes with Avast installed compared with around 8 minutes without. </p>



<p>For the PC Mark Extended test, the PC performed slightly better, with an average score of 1630.67 after three consecutive runs compared with an average of 1643 without Avast installed. The main performance impact was found in the productivity tests that deal with spreadsheets and text documents. That&rsquo;s perhaps not surprising given that Avast One is monitoring files for malicious changes. The difference isn&rsquo;t too huge overall, however; and unless you&rsquo;re opening a ton of large datasets in Excel you shouldn&rsquo;t see much of a performance impact. Gaming performance was unaffected by Avast One.</p>



<h2 id="pricing">Pricing</h2>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large is-resized"><img alt="avast one's offer page for installing google chrome during setup" class="wp-image-548829" height="478" src="https://b2c-contenthub.com/wp-content/uploads/2021/11/AvastOneChrome.png?w=1200" width="727" /><figcaption>Old habits die hard. Despite all the changes, Avast still offers to install Google Chrome during setup.</figcaption></figure><p class="imageCredit">IDG</p></div>



<p><a href="https://www.anrdoezrs.net/links/8200811/type/dlg/sid/2-1-548703-1-0-0/https://www.avast.com/en-us/lp-aff-pcworld-a1?couponfield=yes&amp;cjevent=5d88757000d8ec3dc24a66fca90388f4774b3e91c779c6b24#pc" rel="nofollow">Avast One costs $29.99</a> for the first year for new customers, with a regular price of $99.99 per year. For that price you get one Avast account that covers five devices. That&rsquo;s quite a switch from Avast&rsquo;s old Premier pricing that would cover a single PC for $70.</p>



<p>Avast One Family provides six accounts and coverage for up to 30 devices and is priced at $48.99 for the first year for new customers, and a regular price of $139.99 per year. </p>



<p>If a paid suite isn&rsquo;t your bag then there&rsquo;s also Avast One Essential, which includes a lot of features for free, including that 5GB of VPN usage every week. But you miss out on items like the sensitive data shield, webcam protection, and optimization features such as the disk cleaner and driver updater.</p>



<p>Avast One is available for Windows, macOS, Android, and iOS.</p>



<h2 id="conclusion">Conclusion</h2>



<p>Avast One is a very good security suite. The price is right, and its protection is excellent. The performance impacts are negligible for most users, and it&rsquo;s also a good value within the Avast lineup, which is not something I would&rsquo;ve said about Avast Premier a few years ago. If you&rsquo;re looking for a new security suite, or want to upgrade your current Avast lifestyle, I&rsquo;d highly recommend looking at Avast One. </p>



<p><em><strong>Editor&rsquo;s note:</strong> Because online services are often iterative, gaining new features and performance improvements over time, this review is subject to change in order to accurately reflect the current state of the service. Any changes to text or our final review verdict will be noted at the top of this article.</em></p>

Security</div>

## Lenovo Thinkpad T16 Gen 1 review: A big-screened workstation for pros
 - [https://www.pcworld.com/article/1526483/lenovo-thinkpad-t16-gen-1-review.html](https://www.pcworld.com/article/1526483/lenovo-thinkpad-t16-gen-1-review.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-03-03 11:45:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>


<div class="review" id="review-body"><span class="review-title">At a glance</span><h3 class="review-subTitle" id="experts-rating">Expert's Rating</h3><div class="starRating"></div>
<div><div class="review-columns"><div class="review-column"><h3 class="review-subTitle" id="pros">Pros</h3><ul class="pros review-list"><li>16-inch 16:10 screen perfect for productivity</li><li>Great keyboard with full numpad</li><li>Decent battery life</li><li>Fast performance</li></ul></div><div class="review-column"><h3 class="review-subTitle" id="cons">Cons</h3><ul class="cons review-list"><li>Middling webcam</li><li>Weak stereo speakers</li><li>Jumpy trackpad</li></ul></div></div></div><h3 class="review-subTitle review-subTitle--borderTop" id="our-verdict">Our Verdict</h3><p class="verdict">The Lenovo ThinkPad T16 Gen 1 is a great option for business professionals thanks to its spacious keyboard, enormous screen, and zippy performance.</p>
</div>


<p>Sometimes all you need is a gigantic screen. Whether it&rsquo;s to get a better look at a PowerPoint slide or blow up a dense Excel spreadsheet, it&rsquo;s easier to get a lot of work done when you&rsquo;ve got a larger canvas. In years past, that might have meant springing for a bulky 17-inch class laptop. Thanks to narrow bezels, Lenovo&rsquo;s ThinkPad T16 Gen 1 has managed to cram a 16-inch display into a frame that would&rsquo;ve housed a 15-inch just a few short years ago. With ultrabook thinness, plenty of ports, and a meaty Intel i7 chip, this business laptop is plenty productive even without external screens or desktop docks.</p>



<h2 id="lenovo-thinkpad-t16-specifications-and-features">Lenovo ThinkPad T16: Specifications and features</h2>



<p>Our review unit features an Intel Core i7-1270P CPU, Intel Iris Xe graphics, 16GB of DDR4 RAM, and 512GB of NVMe PCIe SSD storage. For more details, check out the specifications list below: </p>



<ul><li><strong>CPU</strong>: Intel Core i7-1270P (12 cores, 16 threads: 4 performance, 8 efficiency) with vPro</li><li><strong>Memory</strong>: 16 GB DDR4 3200 MHz RAM soldered (up to 48 GB with additional SODIMM)</li><li><strong>Graphics/GPU</strong>: Intel Iris Xe Graphics (Nvidia GeForce MX550 also available with i7-1260P)</li><li><strong>Display</strong>: 16-inch 16&times;10 WUXGA (1920&times;1200) matte IPS LCD</li><li><strong>Storage</strong>: 512 GB M.2 2280 NVMe PCIe solid state drive</li><li><strong>Webcam</strong>: 1080p with physical shutter</li><li><strong>Connectivity</strong>:&nbsp; 2x Thunderbolt 4, 1x 3.5mm combo audio, 2x USB-A 3.2 Gen 1, 1x HDMI</li><li><strong>Networking</strong>: Wi-Fi 6E, Bluetooth, 5G WWAN (optional)</li><li><strong>Biometrics</strong>: Windows Hello facial recognition and fingerprint reader</li><li><strong>Battery capacity</strong>: 86Wh</li><li><strong>Dimensions</strong>: 14.25 W x 10.06 L x 0.81 H inches</li><li><strong>Weight</strong>: 3.9 pounds, 4.95 pounds with AC adapter</li><li><strong>Price: </strong>$1,458.72</li></ul>



<h2><strong>Lenovo ThinkPad T16</strong>: <strong>Design and build quality</strong></h2>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="ThinkPad hero" class="wp-image-1526485" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/02/thinkpad-t16-hero.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">IDG / Brendan Nystedt</p></div>



<p>If we can give Lenovo points for anything, it&rsquo;s consistency. If you get a ThinkPad, it acts like a ThinkPad. Rarely does a slinky, fashionable computer get the ThinkPad badge but instead these are computers with few frills intended for years of use. The ThinkPad T16 Gen 1 embodies this no-nonsense, function-over-form design. Its most distinctive features are its big screen and wide keyboard, both of which make this big machine perfect for an all-in-one workstation.</p>



<p>Just about everything else about this big, slim wedge is made for getting down to your spreadsheets, emails, and Word docs. Its lightly textured plastic gives it a durable feeling, like it&rsquo;d be able to sustain some bumps and jostles during its service lifetime. Since it is such an expansive laptop, it has a little bit of flex, but very little of that matters once you place the T16 where you&rsquo;d likely use it&ndash;on a desk. With its rubber feet sitting stably on a work surface, the T16 stays planted very nicely. In an office setting, I can see this working well on its own, or in a hotdesking scenario hooked up to external screens with a Thunderbolt hub.</p>



<p>While I found it to be a bit big for a caf&eacute; table (and you probably won&rsquo;t be using it on an airplane&rsquo;s tray table), the slim profile makes it easy to fit into a bag meant for a 15-inch laptop. If you&rsquo;ve ever thought about getting a portable USB-C powered display for your small ultrabook, you actually might be better off toting one of these big-screened workstations instead.</p>



<h2><strong>Lenovo ThinkPad T16</strong>: <strong>Connectivity</strong></h2>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="ThinkPad ports" class="wp-image-1526527" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/02/thinkpad-t16-ports.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">IDG / Brendan Nystedt</p></div>



<p>Although it&rsquo;s as thin as a smaller ultrabook, the Lenovo ThinkPad T16 manages to fit the ports you&rsquo;d want in 2023. It has not one but two Thunderbolt 4 ports, a full-size USB 3 port, a full-size HDMI port, a 3.5mm headset jack, and even a full-size RJ45 ethernet jack all along the left side of the device. On the right side, there&rsquo;s a well-placed USB 3 port, perfect for a corded mouse if you&rsquo;re righthanded. Overall, for a device in 2023, it represents a wide variety of options, meaning if you have few enough peripherals the T16 might even be suited for desk duty without a dock or dongle.</p>



<p>Wireless connectivity is exactly what we&rsquo;d expect from a modern, Intel-based laptop featuring WiFi 6E and Bluetooth 5.1. As some organizations might want mobile wireless as well, Lenovo offers up cellular, although our model didn&rsquo;t come with 4G or 5G. Finally, if your org uses smart cards, there&rsquo;s a spot for an optional smart card reader as well.</p>



<h2><strong>Lenovo ThinkPad T16</strong>: <strong>Keyboard and trackpad</strong></h2>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="ThinkPad keyboard" class="wp-image-1526507" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/02/thinkpad-t16-keyboard.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">IDG / Brendan Nystedt</p></div>



<p>Keyboard quality is a hallmark of the ThinkPad brand and the T16 is no exception. It has a light-but-precise-feeling keyboard with comfortable keycaps and I was happy to write the majority of this review on it. Given the big, 16-inch display inside the T16, there&rsquo;s extra space on the right side of the keyboard that&rsquo;s given over to a numpad. While I&rsquo;ve seen some laptop keypads crammed into smaller laptops with uncomfortable narrow buttons, the numpad on the T16 looks and works like a natural extension of the keyboard.</p>



<p>The big touchpad is perhaps less up to par here, and I found it to be overly sensitive and often hijacked my cursor while I was trying to work. The palm detection in particular wasn&rsquo;t well-tuned by default and since the trackpad takes up a good portion of the wrist rest, it&rsquo;s an issue I ran into frequently. Its surface is supposedly made from a slippery mylar, which feels fine but it&rsquo;s a definite downgrade from a glass material.</p>



<p>Real ones know that ThinkPads also come with an alternative to the trackpad, which is called a TrackPoint. This red nub in the middle of the keyboard lets you use the mouse without moving your hands down to the trackpad. It&rsquo;s an acquired taste, but the TrackPoint is pretty awesome once you&rsquo;ve mastered it. With three buttons (the middle lets you scroll when held down), it&rsquo;s a far better option for high-precision mouse use.</p>



<h2><strong>Lenovo ThinkPad T16</strong>: <strong>Display, speakers, and webcam</strong></h2>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="ThinkPad display" class="wp-image-1526508" height="675" src="https://b2c-contenthub.com/wp-content/uploads/2023/02/thinkpad-t16-display.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">IDG / Brendan Nystedt</p></div>



<p>The star of the show here is the ThinkPad T16&rsquo;s honkin&rsquo; huge 16-inch widescreen IPS LCD. Although it&rsquo;s not 4K or any other bananas high-resolution, at 1920&times;1200 and with a usefully-tall 16:10 aspect ratio, it&rsquo;s still an excellent default option. The 300-nit peak brightness of this matte-finished panel was also just right, making glare a non-issue in every location. Assuming you&rsquo;re tackling ordinary business tasks and not video editing or graphic design jobs, the T16&rsquo;s big screen feels so much more expansive than a usual ultrabook than the extra 2 or 3 inches on paper may suggest.</p>



<p>While I was hoping for impressive audio performance from the ThinkPad T16 Gen 1, I came away disappointed. While the twin 2W speakers are fine, they&rsquo;re blown away by other, smaller laptops packing twice the speakers with a offering far &ldquo;bigger&rdquo; sound. It&rsquo;s workable if you&rsquo;re mostly listening to meetings on Microsoft Teams, but if you like to crank up some jams while you get down to business you might want to grab a nice pair of headphones instead.</p>



<p>The webcam is another mixed bag. Although I loved that it has a physical shutter and supports Windows Hello face login, it&rsquo;s not particularly great at making faces look their best or sharpest (it has a maximum resolution of 1920&times;1080, and looks rather noisy). I found that in a caf&eacute; involving mixed warm indoor and cool outdoor lighting, it was unable to make me look like anything but a ghost. Compared to other cameras I&rsquo;ve tried lately, this is passable but not ideal.</p>



<h2><strong>Lenovo ThinkPad T16</strong>: <strong>Performance</strong></h2>



<p>In terms of performance, the ThinkPad T16 Gen 1 is a bit of a sleeper. Although it&rsquo;s a plain-looking business workstation, it&rsquo;s quiet and powerful. The 12 core, 16 thread Intel Core i7-1270P has a 28W TDP, and the bigger laptop body means it&rsquo;s kept cool and quiet even at full tilt. We put the T16 through its paces with our suite of benchmarks and found it to be competent and capable of ripping through typical business tasks, but probably not graphically intense chores like 3D games or creative work.&nbsp;</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="ThinkPad PCMark chart" class="wp-image-1526512" height="618" src="https://b2c-contenthub.com/wp-content/uploads/2023/02/thinkpad-t16-pcmark-chart.jpg?quality=50&amp;strip=all" width="901" /></figure><p class="imageCredit">IDG / Brendan Nystedt</p></div>



<p>We use the PCMark 10 benchmark to get a repeatable, comparable look at a laptop&rsquo;s abilities in a range of normal tasks. With all its cores, the ThinkPad T16 Gen 1 handily beat other thin business notebooks, and bested many of its smaller business rivals. There&rsquo;s little doubt that for complex analysis work, you shouldn&rsquo;t end up waiting long at all.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="ThinkPad Cinebench chart" class="wp-image-1526513" height="618" src="https://b2c-contenthub.com/wp-content/uploads/2023/02/thinkpad-t16-cinebenchr15-chart.jpg?quality=50&amp;strip=all" width="901" /></figure><p class="imageCredit">IDG / Brendan Nystedt</p></div>



<p>In this performance test, we use Cinebench R15 to get a sense for how well all a laptop&rsquo;s processors work together to render 3D graphics. With its dozen cores, the ThinkPad T16 held up quite well. It&rsquo;s clear that the extra threads as well as the bonus performance cores in the Intel P chips make a difference in these types of scenarios.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="ThinkPad 3DMark chart" class="wp-image-1526516" height="618" src="https://b2c-contenthub.com/wp-content/uploads/2023/02/thinkpad-t16-3dmark-chart.jpg?quality=50&amp;strip=all" width="901" /></figure><p class="imageCredit">IDG / Brendan Nystedt</p></div>



<p>Your boss would love knowing that you have a ThinkPad T16 simply because it&rsquo;s rather mediocre at graphically-challenging tasks like gaming. The i7 chip inside has Intel&rsquo;s latest Xe Graphics onboard, but tested behind some other models with more graphics cores when we threw an the 3DMark Time Spy test at it. Rest assured that if you aren&rsquo;t planning to secretly play <em>Halo Infinite</em> at work, the T16 should handle business-oriented tasks without struggle.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="ThinkPad Handbrake chart" class="wp-image-1526517" height="618" src="https://b2c-contenthub.com/wp-content/uploads/2023/02/thinkpad-t16-handbrake-chart.jpg?quality=50&amp;strip=all" width="901" /></figure><p class="imageCredit">IDG / Brendan Nystedt</p></div>



<p>Our last performance comparison takes a look at video encoding, using a high-definition file ripped from a Blu-ray disk. Using Handbrake, we time how long it takes to turn the movie into a tablet-friendly file that&rsquo;s heavily compressed. In this test, the T16 was crushed by the high-powered Asus Zenbook Pro 14 Duo with its powerful i7-12700H chip, but bested the U-class processor seen in machines like the HP Dragonfly Folio G3.</p>



<h2><strong>Lenovo ThinkPad T16</strong>: <strong>Battery Life</strong></h2>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="ThinkPad battery life chart" class="wp-image-1526519" height="618" src="https://b2c-contenthub.com/wp-content/uploads/2023/02/thinkpad-t16-batterylife-chart.jpg?quality=50&amp;strip=all" width="901" /></figure><p class="imageCredit">IDG / Brendan Nystedt</p></div>



<p>Even though it&rsquo;s a slim notebook, the ThinkPad T16 Gen 1 has a fairly large battery inside, clocking in at 86Wh. In our looping video test, we measured just under seven hours of runtime.</p>



<p>This means it can last a decent amount of time while away from a charger, although its big screen and higher performance P-class chip seem to suck down more battery. ARM-based like the Surface Pro 9, with the SQ3 chip, continue to offer the best battery life around, but we do wonder if there will ever be a big-screened laptop with that kind of processor inside.</p>



<h2><strong>Lenovo ThinkPad T16</strong>: <strong>Conclusion</strong></h2>



<p>It isn&rsquo;t surprising that the Lenovo ThinkPad T16 Gen 1 is a capable workhorse. After all, the ThinkPad name still stands for something and that something is getting work done. While I wouldn&rsquo;t recommend it for heavy graphics tasks or intensive editing in Adobe Premiere, this is a single machine that bridges the worlds of office desktop and laptop roles with aplomb and as little nonsense as possible.</p>



<p>If you&rsquo;re considering the T16 for yourself or people in your organization, you&rsquo;ll appreciate the quality keyboard, full-sized numpad, capable processor, and big display. For people who manage databases, tackle a ton of email, or hardcore spreadsheet jockeying, this is the portable, powerful work laptop that can help you stay in the zone at a desk or on the jobsite.</p>

Laptops</div>

## 10 tricks to use Google Search more efficiently
 - [https://www.pcworld.com/article/1526732/10-tricks-to-use-google-search-more-efficiently.html](https://www.pcworld.com/article/1526732/10-tricks-to-use-google-search-more-efficiently.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-03-03 11:30:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>Whether you&rsquo;re shopping, doing research, or just looking to settle a debate with friends, Google is often the first place we turn to for answers. But with billions of results at our fingertips, finding the information we need can sometimes feel like searching for a needle in a haystack.</p>



<p>Fortunately, there are a few tricks and tips you can use to make <a href="https://www.pcworld.com/article/402804/how-to-delete-google-search-history.html">your Google search</a> more efficient and effective. Here are a few of the best tricks to help you find exactly what you&rsquo;re looking for.</p>



<h2 id="search-a-website-for-exact-keywords">Search a website for exact keywords</h2>



<p>Some websites don&rsquo;t have great built-in search functions, which can make it hard to find something you&rsquo;re searching for on that particular site. Google, being the sophisticated search engine that it is, can do just this.</p>



<p>The search query you use is <strong>site:website.com keywords</strong>. So, for example, if you want to search PCWorld for &ldquo;security,&rdquo; you&rsquo;d enter:</p>



<p><strong>Example search query:</strong> <em>site:pcworld.com security</em></p>



<p>The search results will return pages that have &ldquo;security&rdquo; in them, as well as keyword variations such as &ldquo;secure.&rdquo;</p>



<h2 id="search-for-an-exact-phrase">Search for an exact phrase</h2>



<p>You can narrow your search down by prompting Google to return results that contain exact keyword matches. This is useful if you don&rsquo;t know which site you want to find the content on, but know which phrase you&rsquo;re looking for. To do this, you just need to put the words you want the exact match for in quotation marks.</p>



<p>For example, if you want to return results that contain the exact phrase &ldquo;punched paper tape reader&rdquo;, then you&rsquo;d enter:</p>



<p><strong>Example search query:</strong> <em>&ldquo;punched paper tape reader&rdquo;</em></p>



<p>This will only return results that contain the exact same words in the exact same order as what you put in quotes. So it won&rsquo;t return results that contain just &ldquo;punched tape&rdquo; or &ldquo;paper tape.&rdquo;</p>



<h2 id="find-items-between-a-certain-price-range">Find items between a certain price range</h2>



<p>This search query is perfect for those who are looking for a product within a certain budget. This search allows you to tell Google that you want it to return results of an item that falls within a specific price range by placing two periods between the numbers. This saves you time from looking through items that are way over budget by excluding them from the search&mdash;or at least the top results.</p>



<p>For example, if you want to search for flash drives that cost between $10 and $45, you&rsquo;d search:</p>



<p><strong>Example search query:</strong> <em>flash drives $10..$45</em></p>



<p>This may also return pages that have expensive flash drives on them, but also have flash drives in the price range you are looking for.</p>



<h2 id="exclude-certain-words-from-a-search">Exclude certain words from a search</h2>



<p>If you want to search for something, but that search term is dominated by a brand, you can exclude that brand from the search results by adding a hyphen next to it.</p>



<p>For example, if you&rsquo;re wanting to look at laptops, but you don&rsquo;t want <a href="https://www.pcworld.com/article/1068741/dell-inspiron-16-2-in-1-review.html">Dell laptops</a> in the search results, you&rsquo;d enter:</p>



<p><strong>Example search query:</strong> <em>laptops -dell</em></p>



<p>Dell laptops will be excluded from the search, but this doesn&rsquo;t apply to ads in the search results. So if Dell is running an ad campaign for &ldquo;laptops&rdquo;, their ads will still appear at the top of the search results.</p>



<h2 id="search-for-a-certain-file-type">Search for a certain file type</h2>



<p>The web is full of content. This can make it difficult to find certain documents, as the results will often be different web pages, images, and so on. But, you can narrow your search down by telling Google to only return results of a specific file type by using the filetype: prompt.</p>



<p>For example, if you want to find Ford&rsquo;s annual reports in <a href="https://www.pcworld.com/article/407214/best-pdf-editors.html">PDF format</a>, you&rsquo;d search:</p>



<p><strong>Example search query:</strong> <em>Ford annual reports filetype:pdf</em></p>



<p>Now, all of the search results are PDF files.</p>



<h2 id="perform-multiple-search-queries-at-the-same-time">Perform multiple search queries at the same time</h2>



<p>You can be an efficient Google searcher by performing multiple search queries at once. To do this, you just need to add OR between the two searches. This will provide results of both search queries, but both search queries won&rsquo;t necessarily appear in the same result&mdash;they&rsquo;ll be mixed in.</p>



<p>For example, if you want to search for both &ldquo;Best 1 TB HDD&rdquo; or &ldquo;Best 1 TB SSD&rdquo; at the same time, you&rsquo;d enter:</p>



<p><strong>Example search query:</strong> <em>&ldquo;Best 1TB HDD&rdquo; OR &ldquo;Best 1TB SSD&rdquo;</em></p>



<p>The order you put the keywords in doesn&rsquo;t have an effect on the results. So, putting &ldquo;Best 1 TB HDD&rdquo; before or after OR will make no difference.</p>



<h2 id="get-results-for-multiple-keywords">Get results for multiple keywords</h2>



<p>This search trick is similar to the OR search, but instead, you&rsquo;ll use AND to return results that contain both keywords in the search&mdash;not just one or the other.</p>



<p>So, if you wanted to find pages that had results for both &ldquo;<a href="https://www.pcworld.com/article/406861/best-external-drives.html">Best 1 TB HDD</a>&rdquo; and &ldquo;Best 1 TB SSD&rdquo; on the same page, you&rsquo;d enter:</p>



<p><strong>Example search query:</strong> <em>&ldquo;Best 1TB HDD&rdquo; AND &ldquo;Best 1TB SSD&rdquo;</em></p>



<p>Pages that contain one of the keywords but not the other are omitted from the results.</p>



<h2 id="find-results-published-before-or-after-a-certain-date">Find results published before or after a certain date</h2>



<p>If you&rsquo;ve ever searched for something and felt flustered because the results were outdated or too new, you&rsquo;re not alone. Fortunately, you can use before:&lt;date&gt; and after:&lt;date&gt; to filter out the results.</p>



<p>So, if you wanted results for tips for <a href="https://www.pcworld.com/article/1384165/best-work-from-home-tech-2022-2023.html">efficiently working from home</a>, but you only wanted to see articles on the topic that were posted after 2021, then you&rsquo;d enter:</p>



<p><strong>Example search query:</strong> <em>tips for efficiently working from home after:2021</em></p>



<p>Only articles posted after 2021 will appear. Alternatively, if you wanted to search for tips for efficiently working from home before 2020, when working remotely still seemed like a fantasy of a distant future, then you&rsquo;d search:</p>



<p><strong>Example search query:</strong> <em>tips for efficiently working from home before:2020</em></p>



<p>Only articles posted prior to 2020 will appear in the results.</p>



<h2 id="find-content-that-links-to-another-site">Find content that links to another site</h2>



<p>This trick is less known, and can only really be used in certain situations, like if you&rsquo;re curious about who cited an article on a different website. For example, if you&rsquo;re wanting to see which websites have linked back to pcworld.com, you&rsquo;d enter:</p>



<p><strong>Example search query:</strong> <em>link:pcworld.com</em></p>



<p>This is obviously a broad example, but you can put any url you want in the query, even specific articles.</p>

Desktop PCs</div>

## Windows Calendar app is crashing after the latest update
 - [https://www.pcworld.com/article/1530091/windows-calendar-app-is-crashing-after-the-latest-update.html](https://www.pcworld.com/article/1530091/windows-calendar-app-is-crashing-after-the-latest-update.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-03-03 10:45:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>Microsoft&rsquo;s Windows Calendar app within Windows 11 appears to be consistently crashing after the latest update.</p>



<p>Microsoft is beginning to receive reports of the Calendar app crashing repeatedly when it&rsquo;s opened from either the Start menu or in the Windows Mail app, where it&rsquo;s linked. PiunikaWeb began <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://piunikaweb.com/2023/03/02/windows-calendar-app-crashing-or-not-opening-fix-in-works/&amp;xcust=2-1-1530091-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">aggregating reports</a> late Tuesday afternoon. </p>



<p>This reporter has also witnessed the same behavior: If you open the Calendar app from within Mail, the app loads a window header, then crashes. The app demonstrates the same behavior if you load it from the Start menu, too. Others <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://answers.microsoft.com/en-us/outlook_com/forum/all/my-calendar-does-not-launch/a3e89d34-7adb-436e-8527-911522c5b516&amp;xcust=2-1-1530091-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">reporting the issue</a> to Microsoft are having the same problem. Microsoft advisors posting on the company&rsquo;s support forums say that Microsoft is aware of the issue, but has no current fix in place.</p>



<p>Fortunately, there does seem to be a workaround. Users can either use the Outlook app to access their integrated calendar, or else access their email and the calendar using Outlook for the Web. Microsoft also recommends logging out and resetting the Calendar app, but using Outlook for the Web client instead seems to be a lot less complicated and intrusive. </p>



<p>Microsoft debuted the latest update to Windows 11 this week, which added features such as links to Bing Chat within the Start menu, plus some handy <a href="https://www.pcworld.com/article/1527037/windows-11s-new-features-are-ho-hum-but-the-best-one-saves-you-money.html">power recommendations to lower your energy bill</a> and integrated screen recording within the Snipping Tool. Some of the updates included scheduled app updates as well as in Windows; on our test machine, we saw the Mail &amp; Calendar app update. While you can use Outlook, we do consider <a href="https://www.pcworld.com/article/606623/the-best-email-client-for-you-may-be-mail-not-outlook.html">Mail (and Calendar) to be a hidden gem</a> within Windows.</p>

Windows</div>

## This CES-featured AI art tool is just $50 for a limited time
 - [https://www.pcworld.com/article/1528544/this-ces-featured-ai-art-tool-is-just-50-for-a-limited-time.html](https://www.pcworld.com/article/1528544/this-ces-featured-ai-art-tool-is-just-50-for-a-limited-time.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-03-03 08:00:00+00:00

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>While the world has been preoccupied with&nbsp;<a href="https://www.pcworld.com/article/1424575/chatgpt-is-the-future-of-ai-chatbots.html" rel="noreferrer noopener" target="_blank">ChatGPT</a>&nbsp;and its implications, AI has made even more interesting strides in the art world. A highlight at&nbsp;<a href="https://www.pcworld.com/article/1447954/best-of-ces-2023-the-most-intriguing-and-innovative-pc-hardware.html" rel="noreferrer noopener" target="_blank">CES 2023</a>, AI art tools are making the art world more accessible to everybody, regardless of talent. All you need is an idea.</p>



<p>With a tool like&nbsp;<a href="https://shop.pcworld.com/sales/dream-ai-art-tool-premium-lifetime-subscription?utm_source=pcworld.com&amp;utm_medium=referral&amp;utm_campaign=dream-ai-art-tool-premium-lifetime-subscription&amp;utm_term=scsf-565860&amp;utm_content=a0x1P0000058SNvQAM&amp;scsonar=1" rel="noreferrer noopener" target="_blank">Dream by WOMBO</a>, you can make virtually any idea an artistic reality. Winner of Google&rsquo;s Best Overall App in 2022 and rated 4.8 stars on the App Store, this AI art tool is part of the tech innovations at CES that we&rsquo;re offering at big discounts between 2/28 and 3/5 at 11:59 p.m. Pacific.</p>



<p>Creating beautiful art with Dream by WOMBO is extremely easy. Just&nbsp;<a href="https://shop.pcworld.com/sales/dream-ai-art-tool-premium-lifetime-subscription?utm_source=pcworld.com&amp;utm_medium=referral&amp;utm_campaign=dream-ai-art-tool-premium-lifetime-subscription&amp;utm_term=scsf-565860&amp;utm_content=a0x1P0000058SNvQAM&amp;scsonar=1" rel="noreferrer noopener" target="_blank">enter a prompt</a>, pick an art style, and the AI generates your painting in a matter of seconds. With a Premium Plan, you&rsquo;ll get access to exclusive channels in the WOMBO Dream Discord, get exclusive art styles, and speed up creation by making four versions at a time. You can even fine-tune your best output with three alternatives.</p>



<p>Turn your wildest dreams into art. February 28th through 3/5, you can get a lifetime Premium Plan for&nbsp;<a href="https://shop.pcworld.com/sales/dream-ai-art-tool-premium-lifetime-subscription?utm_source=pcworld.com&amp;utm_medium=referral&amp;utm_campaign=dream-ai-art-tool-premium-lifetime-subscription&amp;utm_term=scsf-565860&amp;utm_content=a0x1P0000058SNvQAM&amp;scsonar=1" rel="noreferrer noopener" target="_blank">Dream by WOMBO AI Art Tool</a>&nbsp;for 76% off $169 at just $49.99.</p>



<p><a href="https://shop.pcworld.com/sales/dream-ai-art-tool-premium-lifetime-subscription?utm_source=pcworld.com&amp;utm_medium=referral-cta&amp;utm_campaign=dream-ai-art-tool-premium-lifetime-subscription&amp;utm_term=scsf-565860&amp;utm_content=a0x1P0000058SNvQAM&amp;scsonar=1" rel="noreferrer noopener" target="_blank">&nbsp;</a></p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image"><img alt="" src="https://cdnp2.stackassets.com/868d7c8f882a8f7a0413cf7fdcd442b5861b3657/store/59d8bee7a2e03a8e662d0d75ea1c8fe9ae839cb50348ba2f52131fcb76c9/sale_320032_primary_image.jpg" /></figure></div>



<p><strong>Dream by WOMBO AI Art Tool: Lifetime Subscription (Premium Plan) &ndash; $49.99</strong></p>



<p><a href="https://shop.pcworld.com/sales/dream-ai-art-tool-premium-lifetime-subscription?utm_source=pcworld.com&amp;utm_medium=referral-cta&amp;utm_campaign=dream-ai-art-tool-premium-lifetime-subscription&amp;utm_term=scsf-565860&amp;utm_content=a0x1P0000058SNvQAM&amp;scsonar=1" rel="noreferrer noopener" target="_blank">See Deal</a></p>



<p>Prices subject to change.</p>

Entertainment</div>

