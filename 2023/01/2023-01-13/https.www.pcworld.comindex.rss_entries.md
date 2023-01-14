# Source PC world, Source URL:https://www.pcworld.com/index.rss, Source language: en-US

## Tom Hanks didn’t offer me a job, but it sure sounds like he did
 - [https://www.pcworld.com/article/1473072/tom-hanks-did-not-offer-me-a-job-but-ai-sounds-like-it.html](https://www.pcworld.com/article/1473072/tom-hanks-did-not-offer-me-a-job-but-ai-sounds-like-it.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-01-13 19:09:39+00:00
 - user: None

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>Tom Hanks didn&rsquo;t just call me to pitch me a part, but it sure sounds like it.</p>



<p>Ever since PCWorld began covering the rise of <a href="https://www.pcworld.com/article/788422/how-to-get-started-with-ai-art-dall-e-mini-ai-dungeon-and-more.html">various AI applications like AI art</a>, I&rsquo;ve been poking around in the code repositories in GitHub and links within Reddit, where people will post tweaks to their own AI models for various approaches. </p>



<p>Some of these models actually end up on commercial sites, which either roll their own algorithms or adapt others that have published as open source. A great example of an existing AI audio site is <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://app.uberduck.ai/speak#mode=tts-basic&amp;voice=siri-female-british&amp;xcust=2-1-1473072-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Uberduck.ai</a>, which offers literally hundreds of preprogrammed models. Enter the text in the text field and you can have a virtual Elon Musk, Bill Gates, Peggy Hill, Daffy Duck, Alex Trebek, Beavis, The Joker, or even Siri read out your pre-programmed lines.</p>



<p>We uploaded a fake Bill Clinton praising PCWorld last year and the model already sounds pretty good.</p>



<figure class="wp-block-audio"><audio controls="controls" src="https://b2c-contenthub.com/wp-content/uploads/2022/06/audio-2.wav"></audio><figcaption>Here&rsquo;s a model of our former President sitting down with PCWorld and a snack. It&rsquo;s fake, of course.</figcaption></figure>



<p>Training an AI to reproduce speech involves uploading clear voice samples. The AI &ldquo;learns&rdquo; how the speaker combines sounds with the goal into learning those relationships, perfecting them, and imitating the results. If you&rsquo;re familiar with the excellent 1992 thriller <em>Sneakers</em> (with an all-star cast of Robert Redford, Sidney Poitier, and Ben Kingsley, among others), then you know about the scene in which the characters need to &ldquo;crack&rdquo; a biometric voice password by recording a voice sample of the target&rsquo;s voice. This is almost the exact same thing.</p>



<p>Normally, assembling a good voice model can take quite a bit of training, with lengthy samples to indicate how a particular person speaks. In the past few days, however, something new has emerged: <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://valle-demo.github.io/&amp;xcust=2-1-1473072-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Microsoft Vall-E, a research paper</a> (with live examples) of a synthesized voice that requires just a few seconds of source audio to generate a fully programmable voice.</p>



<p>Naturally, AI researchers and other AI groupies wanted to know if the Vall-E model had been released to the public yet. The answer is no, though you can play with another model if you wish, called Tortoise. (The author notes that it&rsquo;s called Tortoise because it&rsquo;s slow, which it is, but it works.)</p>



<h2 id="train-your-own-ai-voice-with-tortoise">Train your own AI voice with Tortoise</h2>



<p>What makes Tortoise interesting is that you can train the model on whatever voice you choose simply by uploading a few audio clips.  The <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://github.com/Fictiverse/tortoise-tts-Windows&amp;xcust=2-1-1473072-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Tortoise GitHub page</a> notes that you should have a few clips of about a dozen seconds or so. You&rsquo;ll need to save them as a .WAV file with a specific quality.</p>



<p>How does it all work? Through a public utility that you might not be aware of: <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://colab.research.google.com/&amp;xcust=2-1-1473072-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Google Colab</a>. Essentially, Collab is a cloud service that Google provides that allows access to a Python server. The code that you (or someone else) writes can be stored as a notebook, which can be shared with users who have a generic Google account. The <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://colab.research.google.com/drive/1wVVqUPqwiDBUVeWWOUNglpGhU3hg_cbR?usp=sharing&amp;xcust=2-1-1473072-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Tortoise shared resource is here</a>.</p>



<p>The interface looks intimidating, but it&rsquo;s not that bad. You&rsquo;ll need to be logged in as a Google user and then you&rsquo;ll need to click &ldquo;Connect&rdquo; in the upper-right-hand corner. A word of warning. While this Colab doesn&rsquo;t download anything to your Google Drive, other Colabs might. (The audio files this generates, though, are stored in the browser but can be downloaded to your PC.) Be aware that you&rsquo;re running code that someone else has written. You may receive error messages either because of bad inputs or because Google has a hiccup on the back end such as not having an available GPU. It&rsquo;s all a bit experimental. </p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Google Collab Tortoise" class="wp-image-1473081" height="766" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/Google-Collab.png?w=1200" width="1200" /><figcaption>The Tortoise Collab. Click the &ldquo;Connect&rdquo; button to get started, then click  the small &ldquo;play&rdquo; icon next to each block of code in turn.</figcaption></figure><a class="imageCredit" href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://colab.research.google.com/drive/1wVVqUPqwiDBUVeWWOUNglpGhU3hg_cbR?usp=sharing&amp;xcust=2-1-1473072-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Mark Hachman / IDG</a></div>



<p>Each block of code has a small &ldquo;play&rdquo; icon that appears if you hover your mouse over it. You&rsquo;ll need to click &ldquo;play&rdquo; on each block of code to run it, waiting for each block to execute before you run the next.</p>



<p>While we&rsquo;re not going to step through detailed instructions on all of the features, just be aware that the red text is user modifiable, such as the suggested text that you want the model to speak.  About seven blocks down, you&rsquo;ll have the option of training the model. You&rsquo;ll need to name the model, then upload the audio files. When that completes, select the new audio model in the fourth block, run the code, then configure the text in the third block. Run <em>that</em> code block.</p>



<p>If everything goes as planned, you&rsquo;ll have a small audio output of your sample voice. Does it work? Well, I did a quick-and-dirty voice model of my colleague Gordon Mah Ung, whose work appears on our <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.youtube.com/playlist?list=PLJw2-YrAPHYEb0UPqGLhUCmT6tWpzG3q4&amp;xcust=2-1-1473072-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">The Full Nerd podcast</a> as well as various videos. I uploaded a several-minute sample rather than the short snippets, just to see if it would work.</p>



<p>The result? Well, it <em>sounds</em> lifelike, but not like Gordon at all. He&rsquo;s certainly safe from digital impersonation for now. (This is not an endorsement of any fast-food chain, either.)</p>



<figure class="wp-block-audio"><audio controls="controls" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/Gordon-Taco-Bell-2.wav"></audio></figure>



<p>But an existing model that the Tortoise author trained on actor Tom Hanks sounds pretty good. This is not Tom Hanks speaking here! Tom also did <em>not</em> offer me a job, but it was enough to fool at least one of my friends.</p>



<figure class="wp-block-audio"><audio controls="controls" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/Tom-VM-1.wav"></audio></figure>



<p>The conclusion? It&rsquo;s a little scary: the age of believing what we hear (and soon see) is ending. Or it already has.</p>



<p></p>

Personal Software</div>

## Sabrent Rocket 2230 SSD review: The perfect Steam Deck companion
 - [https://www.pcworld.com/article/1441884/1tb-sabrent-rocket-2230-ssd-review.html](https://www.pcworld.com/article/1441884/1tb-sabrent-rocket-2230-ssd-review.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-01-13 15:30:00+00:00
 - user: None

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>


<div class="review" id="review-body"><span class="review-title">At a glance</span><h3 class="review-subTitle" id="experts-rating">Expert's Rating</h3><div class="starRating"></div>
<div><div class="review-columns"><div class="review-column"><h3 class="review-subTitle" id="pros">Pros</h3><ul class="pros review-list"><li>Short (30mm long), 2230 form factor</li><li>Very good everyday performance</li><li>Attractive label and packaging</li></ul></div><div class="review-column"><h3 class="review-subTitle" id="cons">Cons</h3><ul class="cons review-list"><li>A tad pricey for the capacity</li><li>Somewhat low TBW rating</li></ul></div></div></div><h3 class="review-subTitle review-subTitle--borderTop" id="our-verdict">Our Verdict</h3><p class="verdict">Sabrent&rsquo;s Rocket 2230 is perfect for upgrading devices and laptops where a longer 2280 won&rsquo;t fit, such as Valve&rsquo;s Steam Deck. Everyday performance is roughly on par for a DRAM-less design, and we even like the color.</p>
</div>


<p>The common 2280 (22mm wide, 80mm long) NVMe SSD is great for most things, but there are some devices such as the red-hot <a href="https://www.pcworld.com/article/1438078/valve-offers-juicy-details-on-the-steam-deck-2.html">Steam Deck</a> that don&rsquo;t have the room for this form factor. Hence you need an option such as Sabrent&rsquo;s Rocket 2230&mdash;a shorty SSD that&rsquo;s only 30mm long. The Rocket 2230 is a good performer for a HMB (Host Memory Buffer/DRAM-less) design and a good choice for such devices.</p>



<p>Note that for some reason, all the Rocket 2230 SKUs are confusingly numbered 2130, not 2230&mdash;e.g., the 1TB drive we tested is the SB-2130-1TB. (Perhaps the 2230 SKUs were already taken?)</p>



<blockquote class="wp-block-quote"><p><em>Note: This review is part of our ongoing roundup of the <a href="https://www.pcworld.com/article/407542/best-ssds.html">best SSDs</a>. Go there to learn more about competing products, what to look for in an SSD, and buying recommendations.</em></p></blockquote>



<h2 id="sabrent-rocket-2230-design-and-features">Sabrent Rocket 2230: Design and features</h2>



<p>The Sabrent Rocket 2230&rsquo;s size has already been discussed, so let&rsquo;s talk internals: a Phison e21 controller and 176-layer B47R Micron TLC NAND. As mentioned, the Rocket 2230 is an HMB design, meaning it uses some of your system DRAM for primary caching duties. </p>



<p>HMB can&rsquo;t match the peak performance of a design that includes onboard DRAM, but it&rsquo;s pretty darn fast and a lot cheaper. Ditching the DRAM also makes it far simpler to implement an SSD in a shorter form factor. You can of course use a 2230 SSD in any M.2 slot, which might allow for better cooling and more room for other stuff. Just saying.</p>



<p>Sabrent (or Phison&rsquo;s controller if you prefer) uses portions of the NAND as secondary cache by writing only a single bit (writing as SLC) to it, transferring it later written as TLC when time allows. This is standard to all modern SSDs and is one reason to overbuy on capacity. The less free NAND is available, the less can be used as cache.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="" class="wp-image-1442820" height="800" src="https://b2c-contenthub.com/wp-content/uploads/2022/12/Sabrent-Rocket-2230-seated.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /><figcaption>A perfect illustration of just how short the Rocket 2230 is&ndash;less than half the length of standard 2280 drives.</figcaption></figure></div>



<p>As for that capacity, the Sabrent Rocket 2230 is available in $50/256GB, $90/512GB, and $150/1TB capacities. That&rsquo;s a bit on the high side for the latter capacity, but you&rsquo;re paying to some degree for the smaller size. Same thing as with kitchen appliances&mdash;smaller costs more. Go figure.</p>



<p>I&rsquo;d feel remiss if I didn&rsquo;t give props to Sabrent for my favorite packaging touch: a copper-colored case. This is actually wrapped inside a retail box, but it makes me smile when I see it. It can be re-deployed as a pill or parts case once you&rsquo;ve removed the drive. It makes you glad you spent a bit more.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="" class="wp-image-1442857" height="938" src="https://b2c-contenthub.com/wp-content/uploads/2022/12/Sabrent-Copper-Box-2.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /><figcaption>This picture doesn&rsquo;t do justice to the box the Sabrent  Rocket 2230 arrives in.</figcaption></figure></div>



<p>The Rocket 2230 is warrantied for five years and 600TBW (terabytes that may be written) per 1TB of capacity. About average for the genre. </p>



<h2 id="sabrent-rocket-2230-performance">Sabrent Rocket 2230: Performance</h2>



<p>I actually tested both the 1TB and 512GB versions of the 2230. Performance was nearly identical with the exception of the 512GB version running out of cache during the 450GB write and slowing to around 100MBps writing. This was not an issue with the 1TB drive as you&rsquo;ll see in the third chart below.</p>



<p>First off, the CrystalDiskMark 8 results. They&rsquo;re pretty fair for a second-tier NVMe drive using Host Memory Buffer. It actually outpaced two HMB rivals in a couple of tests.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-full"><img alt="" class="wp-image-1442778" height="524" src="https://b2c-contenthub.com/wp-content/uploads/2022/12/Sabrent-2230-CDM8.jpg?quality=50&amp;strip=all" width="1024" /><figcaption>The Rocket 2230 actually managed first place (of these three drives) in several CrystalDiskMark 8 tests. It wasn&rsquo;t quite as impressive in the real world. </figcaption></figure></div>



<p>Keep in mind that the other two drives (<a href="https://www.pcworld.com/article/793850/crucial-p3-plus-nvme-ssd-review.html">Crucial P3 Plus</a> and <a href="https://www.pcworld.com/article/1341419/teamgroup-mp44l-nvme-ssd-review.html">Teamgroup MP44L</a>) in these charts had 2TB of capacity, which allowed them to dedicate more cache to larger transfers without undue computational overhead&mdash;i.e., determining if they would run out.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="" class="wp-image-1442779" height="600" src="https://b2c-contenthub.com/wp-content/uploads/2022/12/Sabrent-2230-48GB.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /><figcaption>Though in the lower tier for the 48GB transfer test, this is still good performance. All NVMe drives are fast.</figcaption></figure></div>



<p>The 1TB capacity of the Rocket 2230 had no issues during the 450GB write, but the 512GB version slowed to a piddling 100MBps at around the halfway mark thanks to its lack of secondary cache. That&rsquo;s normal and one reason to overbuy in terms of capacity with any SSD.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="" class="wp-image-1442780" height="599" src="https://b2c-contenthub.com/wp-content/uploads/2022/12/Sabrent-2230-450GB.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /><figcaption>The 1TB Rocket 2230 turned in a decent time in the 450GB write test. Lower capacities will be significantly slower as the drive falls to 100MBps when writing without cache. </figcaption></figure></div>



<p>Given that the Rocket 2230 I tested had 1TB less of NAND to play with than the comparison drives, the above numbers are very good. Lower tier, but hey, it&rsquo;s NVMe&mdash;it&rsquo;s still very fast.</p>



<blockquote class="wp-block-quote"><p><em>Internal drive tests currently utilize Windows 11 64-bit running on an MSI MEG X570/AMD Ryzen 3700X combo with four 16GB Kingston 2666MHz DDR4 modules, a Zotac (Nvidia) GT 710 1GB x2 PCIe graphics card, and an ASMedia ASM3242 USB 3.2&times;2 card. Copy tests utilize an ImDisk RAM disk using 58GB of the 64GB total memory.</em></p><p><em>Each test is performed on a newly formatted and TRIM&rsquo;d drive so the results are optimal. Over time, as a drive fills up, performance will decrease due to less NAND for caching and other factors.</em> </p><p><em>The performance numbers shown apply only to the drive we were shipped and of the capacity tested. SSD performance can vary by capacity due to more or fewer chips to shotgun reads/writes across and the amount of NAND available for secondary caching.</em> <em>Vendors also occasionally swap components, though Sabrent has never been among those that we&rsquo;re aware of.</em></p></blockquote>



<h2 id="should-you-buy-the-sabrent-rocket-2230-ssd">Should you buy the Sabrent Rocket 2230 SSD?</h2>



<p>The Rocket 2230 is a good, if not spectacular performer for an HMB drive. It&rsquo;s also attractive and sports a decently long warranty. I have zero reason not to recommend it as an upgrade in devices that don&rsquo;t support 80mm M.2 drives. This would be a stellar SSD to slap into your Steam Deck. But if your computer does support longer standard SSDs, you can get the same capacity and performance for less cash.</p>

Storage</div>

## This tiny mechanical gaming keyboard is only $30
 - [https://www.pcworld.com/article/1472848/1472848.html](https://www.pcworld.com/article/1472848/1472848.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-01-13 15:01:35+00:00
 - user: None

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>From the click-clack sound of the keys to the customizable lighting, mechanical keyboards are a lot of fun to use. If you&rsquo;re looking to pick one up for a great price, you&rsquo;re in luck, as we&rsquo;ve got a delicious deal for you today. Amazon&rsquo;s currently selling the <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/Portable-Mechanical-Keyboard-MageGee-Backlit/dp/B098LG3N6R&amp;xcust=2-1-1472848-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">MageGee mechanical gaming wired keyboard for just $29.99</a>, which is 19 percent off of the original price. All you have to do is plug in and play. You don&rsquo;t have to deal with any drivers or additional software.</p>



<p>The MageGee keyboard features red switches, a portable 60 percent compact layout, and customizable blue LED backlighting. Red switches are linear switches, which means they&rsquo;re generally quieter than blue ones and they don&rsquo;t offer any tactile feedback. They don&rsquo;t require much force to press, either. That means they respond super fast, which is ideal for gamers. The keyboard is also quite small and lightweight, which is perfect for traveling. </p>



<p>This is a killer deal. Don&rsquo;t miss out.</p>


<p class="cta wp-block wp-block-button"><a class="cta__btn" href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/Portable-Mechanical-Keyboard-MageGee-Backlit/dp/B098LG3N6R&amp;xcust=2-1-1472848-7-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">Get the MageGee mechanical gaming wired keyboard for $29.99 at Amazon</a></p>
Keyboards</div>

## Sapphire Nitro+ Radeon RX 7900 XTX Vapor-X review: Big, badass, beautiful
 - [https://www.pcworld.com/article/1471803/sapphire-nitro-radeon-rx-7900-xtx-vapor-x-review.html](https://www.pcworld.com/article/1471803/sapphire-nitro-radeon-rx-7900-xtx-vapor-x-review.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-01-13 11:45:00+00:00
 - user: None

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>


<div class="review" id="review-body"><img alt="Editors' Choice" class="review-logo" src="https://www.pcworld.com/wp-content/uploads/2021/09/PC-ED-CHOICE.png" /><span class="review-title">At a glance</span><h3 class="review-subTitle" id="experts-rating">Expert's Rating</h3><div class="starRating"></div>
<div><div class="review-columns"><div class="review-column"><h3 class="review-subTitle" id="pros">Pros</h3><ul class="pros review-list"><li>Exceptional 4K and 1440p performance</li><li>24GB memory</li><li>Nitro+ custom cooler is frigid, silent, and gorgeous</li><li>Dual-BIOS switch, fan, and ARGB headers</li></ul></div><div class="review-column"><h3 class="review-subTitle" id="cons">Cons</h3><ul class="cons review-list"><li>Massive four-slot design</li><li>Very high power draw</li><li>Lags GeForce RTX 40-series GPUs in ray tracing</li><li>Steep $200 premium puts Nitro+ near RTX 4080 pricing</li></ul></div></div></div><h3 class="review-subTitle review-subTitle--borderTop" id="our-verdict">Our Verdict</h3><p class="verdict">The Sapphire Nitro+ looks gorgeous, runs frigid, can&rsquo;t be heard, <em>and </em>it&rsquo;s the fastest XTX we&rsquo;ve tested (albeit by a hair), complete with handy extra features for overclockers. If you&rsquo;re in the market for a four-figure graphics card that chews through high refresh-rate 4K and 1440p gaming without compromise, and your PC can handle its massive size and power draw, the Nitro+ is very highly recommended. </p>
</div>
				<h3 class="review-best-price" id="best-prices-today-nitro-radeon-rx-7900-xtx-vapor-x">
			Best Prices Today: Nitro+ Radeon RX 7900 XTX Vapor-X		</h3>
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
																	<img alt="Amazon" src="https://www.pcworld.com/wp-content/themes/idg-base-theme/dist/static/img/amazon-logo.svg" />
															</div>
							<div class="price-comparison__price">
								<span>$1,475.00</span>
							</div>
							<div>
								<a class="price-comparison__view-button" href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/B0BR6JWP1Q?tag=pcworld02-20&amp;linkCode=ogi&amp;th=1&amp;psc=1&amp;xcust=2-3-1471803-2-1471831-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">View Deal</a>							</div>
						</div>
												<div class="price-comparison__record price-comparison__record--footer">
					<span class="price-comparison__footer-text">
													Price comparison from over 24,000 stores worldwide												</span>
									</div>
						</div>
		


<p>Big, badass graphics cards don&rsquo;t get much bigger or more badass than the Sapphire Nitro+ Radeon RX 7900 XTX Vapor-X&mdash;the first Sapphire GPU to sport the premium Vapor-X brand in nearly a decade.</p>



<p>While <a href="https://www.pcworld.com/article/1431755/amd-radeon-rx-7900-xtx-radeon-rx-7900-xt-review-rdna-3.html">AMD&rsquo;s reference version of the XTX</a> sticks to a reasonable 2.5-slot design, Sapphire threw restraint out the window with the highly customized Nitro+. This monster swells to a chunk <em>quad-slot </em>height, then adds an extra 8-pin power connector to fuel even loftier performance. It&rsquo;s the fastest 7900 XTX we&rsquo;ve tested <em>and </em>it runs cool and quiet while looking superb. This is one of the most impressive custom graphics cards I&rsquo;ve ever laid hands on.</p>



<p>If your PC can fit this beast, and your wallet can accept its $1,200 price tag&mdash;a $200 premium over the reference model&mdash;then you&rsquo;ll love everything about the Sapphire Nitro+ Radeon RX 7900 XTX Vapor-X. Let&rsquo;s dig in.</p>



<blockquote class="wp-block-quote"><p><strong>Further reading: </strong><em><a href="https://www.pcworld.com/article/416006/the-best-graphics-cards-for-pc-gaming.html">The best graphics cards for PC gaming</a></em></p></blockquote>



<h2 class="toc" id="sapphire-nitro-radeon-rx-7900-xtx-vapor-x-specs-price-and-features">Sapphire Nitro+ Radeon RX 7900 XTX Vapor-X: Specs, price, and features</h2>



<p>There isn&rsquo;t too much to say about the <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.sapphiretech.com/en/consumer/nitro-radeon-rx-7900-xtx-vaporx-24g-gddr6&amp;xcust=2-3-1471803-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Nitro+&rsquo;s technical aspects</a>, as it&rsquo;s running on the same spectacular Radeon RX 7900 XTX chip as the reference model, paired with an ample 24GB of fast GDDR6 memory. Sapphire tweaked and tuned it for even more power, however.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Sapphire Nitro+ 7900 XTX " class="wp-image-1471819" height="800" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/sapphire-nitro-radeon-rx-7900-xtx-vapor-x-7.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">Brad Chacos/IDG</p></div>



<p>The Nitro+ 7900 Vapor-X screams along with a blistering 2,510MHz Game Clock, a substantial uplift over the reference 2,300MHz speeds. That matches the similarly premium <a href="https://www.pcworld.com/article/1433026/xfx-speedster-merc-310-7900-xtx-review.html">XFX Speedster Merc 7900 XTX</a>, but the Sapphire card&rsquo;s more efficient cooler lets it squeak out clear victories across our gaming test suite, even if only to the tune of a few extra (and practically unnoticeable) frames per second. The baseline 7900 XTX is already the second-most powerful GPU on the planet, trailing only the <a href="https://www.pcworld.com/article/1348123/nvidia-geforce-rtx-4090-review-ada-lovelace.html">$1,600 GeForce RTX 4090</a> in raw might, and the Nitro+ cranks it to 11.</p>



<p>Doing so requires more literal power, however. The Sapphire Nitro+ Radeon RX 7900 XTX Vapor-X demands a trio of 8-pin power connectors, up from the reference version&rsquo;s pair, and it&rsquo;s rated to draw 420 watts of power. The reference XTX draws 355W. In the real world, that means the Nitro+ 7900 XTX consumes more power than even the RTX 4090 during gaming sessions.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Sapphire Nitro+ 7900 XTX" class="wp-image-1471818" height="800" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/sapphire-nitro-radeon-rx-7900-xtx-vapor-x-8.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">Brad Chacos/IDG</p></div>



<p>The card includes a three-way BIOS switch that changes the card&rsquo;s behavior, however. The default position lets you hop between the Nitro+&rsquo;s dual BIOS options using <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.sapphiretech.com/en/software&amp;xcust=2-3-1471803-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Sapphire&rsquo;s Trixx utility</a>, rather than having to manually flip the BIOS switch on the card. If you don&rsquo;t want to install that software, however, the second position sticks to the default high-performance BIOS, while the third position is a lower-power mode that drops to reference speeds in exchange for shaving 50W off the power draw. The default BIOS runs so cool and quiet that there&rsquo;s no reason to recommend the low-power option unless power draw is a major concern&mdash;and if it is, you shouldn&rsquo;t be buying a 7900 XTX to begin with.</p>



<p>The Sapphire Nitro+ Radeon RX 7900 XTX Vapor-X&rsquo;s real draw is its custom design. There&rsquo;s so much hardware in here, Sapphire tossed a GPU support bracket into the box to keep your graphics card from potentially sagging in its motherboard slot over time!</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Sapphire Nitro+ 7900 XTX" class="wp-image-1471816" height="750" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/sapphire-nitro-radeon-rx-7900-xtx-vapor-x-4.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">Sapphire</p></div>



<p>Let&rsquo;s start with aesthetics: The Nitro+ 7900 XTX looks absolutely beautiful, sporting a deliciously clean all-metal design, punctuated by raised, full-length RGB bars on both sides of the heatsink. The bars somehow shine with shocking vibrancy, with rounded edges that add to its visual cohesion. The default sweeping rainbow pattern fills your case with shimmering light since Sapphire slapped the bars on both sides. It&rsquo;s gorgeous, albeit in a <em>totally different way</em> than the also-gorgeous <a href="https://www.pcworld.com/article/1433026/xfx-speedster-merc-310-7900-xtx-review.html">XFX Speedster Merc 7900 XTX</a>, which went in an RGB-less direction instead.</p>



<p>The Nitro+ 7900 XTX&rsquo;s true secret sauce lies underneath the hood though. Sapphire absolutely stuffed this behemoth full of cooling technology. <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.sapphiretech.com/en/consumer/nitro-radeon-rx-7900-xtx-vaporx-24g-gddr6&amp;xcust=2-3-1471803-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Sapphire&rsquo;s webpage for the Nitro+</a> goes into far deeper detail, but at a high level, the die-cast aluminum frame holds a trio of axial fans with dual ball-bearing designs. They support Sapphire&rsquo;s rad Quick Connect feature, which lets you quickly and easily disconnect individual fans if they need repair. Better yet, they stop spinning completely when the GPU isn&rsquo;t under high load. That means the Nitro+ 7900 XTX is completely silent when you aren&rsquo;t gaming or performing other GPU-stressing work.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Sapphire Nitro+ 7900 XTX" class="wp-image-1471811" height="800" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/sapphire-nitro-radeon-rx-7900-xtx-vapor-x-6.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /><figcaption><p>Chonky and clean.</p></figcaption></figure><p class="imageCredit">Brad Chacos/IDG</p></div>



<p>Another key perk: Sapphire slapped a second HDMI 2.1 port on the Nitro+, doubling up on the reference design. VR users, take note! It&rsquo;s joined by a pair of DisplayPort 2.1 connections, though Sapphire eschewed the reference model&rsquo;s USB-C port to include the extra HDMI. It also includes helpful ARGB and fan headers if you want to hook it more deeply into the rest of your system.</p>



<p>Of course, the Sapphire Nitro+ Radeon RX 7900 XTX Vapor-X supports all of AMD&rsquo;s awesome Radeon software features, like FSR, Radeon Anti-Lag, Smart Access Memory, and more. But enough chit-chat. Let&rsquo;s get to the benchmarks!</p>



<h2 class="toc" id="our-test-system">Our test system</h2>



<p>We test graphics cards on an AMD Ryzen 5900X PC used exclusively for benchmarking GPUs. We now test with PCIe Resizable BAR (also known as Smart Access Memory on Ryzen systems) active, as most modern gaming PCs released in the last four years support the performance-boosting feature, either natively or via a motherboard firmware update. Nvidia also recommends turning on the optional &ldquo;Hardware-accelerated GPU scheduling&rdquo; option in Windows to let the RTX 40-series stretch its legs to the fullest, so we&rsquo;ve made that tweak as well. Most of the hardware was provided by the manufacturers, but we purchased the storage ourselves.</p>



<ul><li>AMD Ryzen 5900X, stock settings</li><li>AMD Wraith Max cooler</li><li>MSI Godlike X570 motherboard</li><li>32GB G.Skill Trident Z Neo DDR4 3800 memory, XMP active</li><li>Corsair <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/Corsair-HX1500i-Platinum-Ultra-Low-Connectors/dp/B0B3S8GMCK&amp;xcust=2-3-1471803-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">HX1500i power supply</a> (and optional <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.corsair.com/us/en/Categories/Products/Accessories-%7C-Parts/PC-Components/Power-Supplies/600W-PCIe-5-0-12VHPWR-Type-4-PSU-Power-Cable/p/CP-8920284&amp;xcust=2-3-1471803-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">$20 12VHPWR 600 cable</a> for Nvidia GPUs)</li><li><a href="https://www.pcworld.com/article/3440740/sk-hynix-gold-s31-review-a-great-sata-ssd-from-the-largest-vendor-youve-likely-never-heard-of.html">1TB SK Hynix Gold S31 SSD</a> x2</li></ul>



<p>We&rsquo;re comparing the $1,200 Sapphire Nitro+ against the $1,000 reference Radeon RX 7900 XTX as well as XFX&rsquo;s similarly premium $1,100 Speedster Merc custom card, as what we&rsquo;re really looking for here is the Nitro+&rsquo;s performance as a custom XTX model. We&rsquo;ve also included other GPUs that are worth considering when you&rsquo;re looking for excellent 4K and 1440p gaming.</p>



<p>We test a variety of games spanning various engines, genres, vendor sponsorships (Nvidia, AMD, and Intel), and graphics APIs (DirectX 9, 11, DX12, and Vulkan), to try to represent a full range of performance potential. Each game is tested using its in-game benchmark, then sanity checked by <a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.nvidia.com/en-us/geforce/technologies/frameview/&amp;xcust=2-3-1471803-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow">Nvidia&rsquo;s FrameView tool</a>, at the highest possible graphics presets unless otherwise noted, with VSync, frame rate caps, real-time ray tracing or DLSS effects, and FreeSync/G-Sync disabled, along with any other vendor-specific technologies like FidelityFX tools or Nvidia Reflex. We&rsquo;ve also enabled temporal anti-aliasing (TAA) to push these cards to their limits. We run each benchmark at least three times and list the average result for each test.</p>



<p>Rather than rolling out our full testing suite for this review, we stuck to a simpler lineup that&rsquo;s representative of a variety of APIs (DX9, DX11, DX12, Vulkan), to show the Nitro+&rsquo;s performance across various scenarios. Be sure to check out our initial Radeon RX 7900 XTX review for a broader, deeper look at the GPU&rsquo;s general performance. (In short, it beats the $1,200 RTX 4080 in traditional games for a much lower price, and matches the RTX 30-series&rsquo; ray-tracing performance, but lags far behind the RTX 40-series in ray tracing. It also lacks a DLSS 3 Frame gen competitor.)</p>



<h2 class="toc" id="sapphire-nitro-radeon-rx-7900-xtx-vapor-x-gaming-performance-benchmarks">Sapphire Nitro+ Radeon RX 7900 XTX Vapor-X: Gaming performance benchmarks</h2>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Sapphire Nitro+ 7900 XTX benchmarks" class="wp-image-1471807" height="1200" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/cyberpunk-1.jpg?quality=50&amp;strip=all&amp;w=1184" width="1184" /></figure><p class="imageCredit">Brad Chacos/IDG</p></div>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Sapphire Nitro+ 7900 XTX benchmarks" class="wp-image-1471809" height="1200" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/rdr2-1.jpg?quality=50&amp;strip=all&amp;w=1184" width="1184" /></figure><p class="imageCredit">Brad Chacos/IDG</p></div>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Sapphire Nitro+ 7900 XTX benchmarks" class="wp-image-1471805" height="1200" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/codmw2-1.jpg?quality=50&amp;strip=all&amp;w=1184" width="1184" /></figure><p class="imageCredit">Brad Chacos/IDG</p></div>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Sapphire Nitro+ 7900 XTX benchmarks" class="wp-image-1471813" height="1200" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/troy.jpg?quality=50&amp;strip=all&amp;w=1184" width="1184" /></figure><p class="imageCredit">Brad Chacos/IDG</p></div>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Sapphire Nitro+ 7900 XTX benchmarks" class="wp-image-1471810" height="1200" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/csgo-1.jpg?quality=50&amp;strip=all&amp;w=1185" width="1185" /></figure><p class="imageCredit">Brad Chacos/IDG</p></div>



<h2 class="toc" id="sapphire-nitro-radeon-rx-7900-xtx-vapor-x-power-and-thermals">Sapphire Nitro+ Radeon RX 7900 XTX Vapor-X: Power and thermals</h2>



<p>We test power draw by looping the&nbsp;<em>F1 22</em>&nbsp;benchmark at 4K for about 20 minutes after we&rsquo;ve benchmarked everything else (to warm up the GPU) and noting the highest reading on our Watts Up Pro meter, which measures the power consumption of our entire test system. The initial part of the race, where all competing cars are onscreen simultaneously, tends to be the most demanding portion.&nbsp;</p>



<p>This isn&rsquo;t a worst-case test; this is a GPU-bound game running at a GPU-bound resolution to gauge performance when the graphics card is sweating hard. If you&rsquo;re playing a game that also hammers the CPU, you could see higher overall system power draws. Consider yourself warned.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Sapphire Nitro+ 7900 XTX benchmarks" class="wp-image-1471806" height="1199" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/power-1.jpg?quality=50&amp;strip=all&amp;w=1183" width="1183" /></figure><p class="imageCredit">Brad Chacos/IDG</p></div>



<p>The Sapphire Nitro+ pushes AMD&rsquo;s already-power hungry Radeon 7900 XTX to new heights, but doing so requires even higher peak power draw than the monstrous RTX 4090. That&rsquo;s a bit of a bummer, but you probably aren&rsquo;t buying a fire-breathing 7900 XTX for its efficiency.</p>



<p>We test thermals by leaving GPU-Z open during the&nbsp;<em>F1 22</em>&nbsp;power draw test, noting the highest maximum temperature at the end.</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Sapphire Nitro+ 7900 XTX benchmarks" class="wp-image-1471804" height="1199" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/temps-1.jpg?quality=50&amp;strip=all&amp;w=1183" width="1183" /></figure><p class="imageCredit">Brad Chacos/IDG</p></div>



<p>The Sapphire Nitro+ Radeon RX 7900 XTX&rsquo;s awesome Vapor-X cooler does stellar work here. Technically, it runs slightly warmer than the XFX Speedster Merc, but both deliver absolutely <em>frigid </em>results that overclockers will appreciate, and the Nitro+&rsquo;s gentler fan curve actually sounds even quieter than the already borderline-silent Merc. These are both outstanding custom designs that far outshine the undersized 7900 XTX reference model, though you pay for it in price, power consumption, and sheer size.</p>



<h2 class="toc" id="should-you-buy-the-sapphire-nitro-radeon-rx-7900-xtx-vapor-x">Should you buy the Sapphire Nitro+ Radeon RX 7900 XTX Vapor-X?</h2>



<p>If you mostly stick to traditional games and want a barn-burner of a graphics card for hundreds of dollars less than the RTX 4080, <a href="https://www.pcworld.com/article/1431755/amd-radeon-rx-7900-xtx-radeon-rx-7900-xt-review-rdna-3.html">AMD&rsquo;s Radeon RX 7900 XTX</a> is an excellent choice, as our original review detailed in depth. And if you want to splurge for a high-end, impeccably designed custom version of the XTX, Sapphire&rsquo;s Nitro+ is well worth considering. It&rsquo;s blisteringly fast, cool, quiet, and utterly fantastic.</p>



<p>It won&rsquo;t be for everyone. The Nitro+ is absolutely <em>massive</em> and draws more power than even the RTX 4090&mdash;but big, badass, custom cards are what you expect from flagships like this. If that worries you, consider the reference XTX&rsquo;s smaller 2.5-slot, 2x 8-pin design instead. The price might also give you pause. Sapphire&rsquo;s $200 premium feels justifiable for a custom design <em>this </em>magnificent, but it also bumps it right up against the <a href="https://www.pcworld.com/article/1379747/nvidia-geforce-rtx-4080-tested-5-things.html">GeForce RTX 4080&rsquo;s (terribly high) starting price</a>. The Nitro+ is faster, and you won&rsquo;t get a RTX 4080 similar to the Nitro+&rsquo;s spectacular quality without spending closer to $1,400 or $1,500, but if you place a higher premium on ray-tracing performance and DLSS 3 Frame Gen over card design and overall quality of life, you might&mdash;<em>might</em>&mdash;opt for a &ldquo;cheap&rdquo; 4080 over the wonderfully baller Nitro+. (I wouldn&rsquo;t.)</p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image size-large"><img alt="Sapphire Nitro+ 7900 XTX " class="wp-image-1471814" height="800" src="https://b2c-contenthub.com/wp-content/uploads/2023/01/sapphire-nitro-radeon-rx-7900-xtx-vapor-x-2.jpg?quality=50&amp;strip=all&amp;w=1200" width="1200" /></figure><p class="imageCredit">Brad Chacos/IDG</p></div>



<p>Staying in AMD-land, if you&rsquo;re opting for a high-end 7900 XTX, the aesthetics and street pricing are the biggest differentiators between the $1,200 Nitro+ and the $1,100 <a href="https://www.pcworld.com/article/1433026/xfx-speedster-merc-310-7900-xtx-review.html">XFX Speedster Merc 7900 XTX</a>. They&rsquo;re both face-meltingly fast, attractive, and wonderfully quiet and cool. I personally prefer the Nitro+&rsquo;s futuristic industrial look and shimmering dual-side RGB bars, but the Merc is a looker of a totally different variety. Go where your eyes (and wallet) guide you.</p>



<p>Bottom line? The Sapphire Nitro+ looks gorgeous, runs frigid and damned-near dead silent, <em>and </em>it&rsquo;s the fastest XTX we&rsquo;ve tested (albeit by a hair). If you&rsquo;re in the market for a four-figure graphics card that&rsquo;s actually worth the money (<em>cough</em> unlike the RTX 4080 <em>cough</em>), we highly recommended this option. It&rsquo;s the best Radeon offers.</p>

Gaming, Graphics Cards</div>

## The best ultrawide monitors: Let’s get large
 - [https://www.pcworld.com/article/1470449/best-ultrawide-monitors.html](https://www.pcworld.com/article/1470449/best-ultrawide-monitors.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-01-13 11:30:00+00:00
 - user: None

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>Do you want a huge amount of usable display space, but also want to stick with a single monitor? If so, an ultrawide monitor is the ticket. These monitors have a wider display panel that&rsquo;s far more impressive, and immersive, than your average widescreen. We&rsquo;ve tested a bunch of ultrawide monitors in order to name the best picks in various categories. You can learn more about our evaluation process and what to look for in an ultrawide monitor below our recommendations. &nbsp;</p>



<p>You can find even more monitor recommendations in our roundup of the <a href="https://www.pcworld.com/article/811315/best-monitors-2.html">best monitors</a>.</p>



		<div class="wp-block-product-chart product-chart">
					<div class="product-chart-separator"></div>
			<div class="wp-block-product-chart-item product-chart-item">
									<div class="product-chart-item__title-wrapper">
						<h3 class="product-chart-item__title-wrapper--title product-chart-title " id="1-alienware-aw3423dwf-best-ultrawide-monitor">
							1.  Alienware AW3423DWF &ndash; Best ultrawide monitor						</h3>
					</div>
													<div class="large-pro-cons-product-chart-section">
											<div class="product-chart-item__image-outer-wrapper
							product-chart-item__image-outer-wrapper--large">
							<div class="product-chart-item__image-wrapper">
								<img alt="Alienware AW3423DWF - Best ultrawide monitor" class="product-chart-item__image" height="1000" src="https://b2c-contenthub.com/wp-content/uploads/2022/12/alienware-aw3423dwf-3.jpg?quality=50&amp;strip=all" width="1500" />
							</div>
						</div>
															<div class="product-chart-body">
						<div class="product-chart-columns">
							
								<div class="product-chart-column">
									<p class="product-chart-subTitle">Pros</p>
									<ul class="product-pros-cons-list">
															<li> 
					Excellent contrast ratio&nbsp;					</li> 
										<li> 
					Top-notch color gamut and accuracy					</li> 
										<li> 
					Great motion clarity&nbsp;					</li> 
										<li> 
					Respectable HDR performance					</li> 
										<li> 
					Extremely competitive price					</li> 
														</ul> 
								</div>
																					<div class="product-chart-column">
								<p class="product-chart-subTitle">Cons</p>
								<ul class="product-pros-cons-list">
														<li> 
					Stand is a bit too large					</li> 
										<li> 
					No USB-C					</li> 
										<li> 
					Maximum HDR brightness is lackluster					</li> 
													</ul> 
							</div>
													</div>
					</div>
														</div>
						
					<div class="product-chart-item__information ">
														<div class="product-widget__information--rrp-wrapper">
										<span class="product-widget__information--rrp-label">
																			</span>
										<span class="product-widget__information--rrp-value">
																				</span>
									</div>
									
											</div>
										<div class="product-content">
						
<p>The Alienware AW3423DWF is a legendary monitor. It packs the incredible contrast and realism of OLED in a 34-inch widescreen panel, yet it&rsquo;s priced at just $1,099. That&rsquo;s not inexpensive, but it&rsquo;s better value than other OLED monitors available right now.</p>

<p>Image quality is where it stands out. It delivers a vivid, immersive, rich experience with deep black levels and bright highlights, which are enhanced by the display&rsquo;s glossy finish. Movies and games seem nearly three-dimensional&mdash;as if you&rsquo;re looking through a window, not staring at a monitor.</p>

<p>What&rsquo;s the catch? The monitor is not bright, especially in SDR, so it&rsquo;s a bad choice for a brightly lit room. We also noticed the OLED panel has trouble rendering small fonts smoothly. These are minor issues, though, and shouldn&rsquo;t trouble most owners.</p>

<p>This monitor targets gamers, so it offers an enhanced refresh rate of up to 165Hz and supports AMD FreeSync Premium Pro for smooth frame pacing in games. However, its excellent image quality will be impressive in everyday use, as well.</p>

<p>It has good connectivity, with two DisplayPort inputs and one HDMI, as well as a USB-A hub with four ports. There&rsquo;s even a healthy range of calibration options that help demanding owners dial in the image to their personal specifications.</p>
						</div>
											Read our full 
					<a class="product-chart-item__review-link" href="https://www.pcworld.com/article/1440675/alienware-aw3423dwf-review.html" target="_blank"> Review Alienware AW3423DWF</a>
								</div>
			<div class="ad page-ad has-ad-prefix ad-article"></div>			<div class="product-chart-separator"></div>
			<div class="wp-block-product-chart-item product-chart-item">
									<div class="product-chart-item__title-wrapper">
						<h3 class="product-chart-item__title-wrapper--title product-chart-title " id="2-asus-proart-pa348cgv-best-ultrawide-monitor-for-professionals">
							2.  Asus ProArt PA348CGV &ndash; Best ultrawide monitor for professionals						</h3>
					</div>
													<div class="large-pro-cons-product-chart-section">
											<div class="product-chart-item__image-outer-wrapper
							product-chart-item__image-outer-wrapper--large">
							<div class="product-chart-item__image-wrapper">
								<img alt="Asus ProArt PA348CGV - Best ultrawide monitor for professionals" class="product-chart-item__image" height="1000" src="https://b2c-contenthub.com/wp-content/uploads/2022/10/asus-proart-PA348CGV-5.jpg?quality=50&amp;strip=all" width="1500" />
							</div>
						</div>
															<div class="product-chart-body">
						<div class="product-chart-columns">
							
								<div class="product-chart-column">
									<p class="product-chart-subTitle">Pros</p>
									<ul class="product-pros-cons-list">
															<li> 
					Excellent SDR image quality&nbsp;					</li> 
										<li> 
					Sturdy, hefty design&nbsp;					</li> 
										<li> 
					Wide range of customization					</li> 
										<li> 
					120Hz refresh rate					</li> 
														</ul> 
								</div>
																					<div class="product-chart-column">
								<p class="product-chart-subTitle">Cons</p>
								<ul class="product-pros-cons-list">
														<li> 
					USB-C hub lacks video-out or ethernet					</li> 
										<li> 
					HDR is merely passable					</li> 
													</ul> 
							</div>
													</div>
					</div>
														</div>
						
					<div class="product-chart-item__information ">
														<div class="product-widget__information--rrp-wrapper">
										<span class="product-widget__information--rrp-label">
																			</span>
										<span class="product-widget__information--rrp-value">
																				</span>
									</div>
									
													<div class="product-chart-item__pricing-details ">
																	<span class="product-chart-item__pricing-details--label">
										Best Prices Today:
									</span>
																<span class="product-chart-item__pricing-details--links-wrapper">
																			<span class="not-amp">
										<a class="product-chart-item__pricing-details--link" href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/B09XJMGMVS?tag=pcworld02-20&amp;linkCode=ogi&amp;th=1&amp;psc=1&amp;xcust=2-3-1470449-6-1346718-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">$729.99 at  Amazon</a>										</span>
																		</span>
							</div>
											</div>
										<div class="product-content">
						
<p>The Asus ProArt PA348CV surpassed our expectations. Priced at just $729.99, it&rsquo;s towards the low end of pricing for a professional ultrawide display&mdash;yet its performance is near the top of the pack.</p>

<p>This monitor has a wide color gamut, excellent color accuracy, and a virtual buffet of image-quality calibration features that let users precisely tune the image. It&rsquo;s also a bright and vivid monitor, making it easy to use in nearly any office. Admittedly, it doesn&rsquo;t set any records in image quality tests&mdash;but it ties or comes close to alternatives that are hundreds of dollars more expensive.</p>

<p>Asus throws in a useful USB-C port that supports DisplayPort Alternate Mode and delivers 90 watts of USB Power Delivery. It also drives a USB-A hub with four downstream ports. Additional video connectivity includes two HDMI and one DisplayPort for a total of four input options.</p>

<p>Surprisingly, Asus throws in an enhanced refresh rate up to 120Hz. It&rsquo;s not sold as a gaming monitor, but it can handle gaming well enough. That&rsquo;s good news if you need one home office monitor for both work and play.</p>
						</div>
											Read our full 
					<a class="product-chart-item__review-link" href="https://www.pcworld.com/article/1346674/asus-proart-pa348cgv-review.html" target="_blank"> Review Asus ProArt PA348CGV</a>
								</div>
			<div class="ad page-ad has-ad-prefix ad-article"></div>			<div class="product-chart-separator"></div>
			<div class="wp-block-product-chart-item product-chart-item">
									<div class="product-chart-item__title-wrapper">
						<h3 class="product-chart-item__title-wrapper--title product-chart-title " id="3-lg-ultragear-34gn850-best-budget-ultrawide-for-gamers">
							3.  LG Ultragear 34GN850 &ndash; Best budget ultrawide for gamers						</h3>
					</div>
													<div class="large-pro-cons-product-chart-section">
											<div class="product-chart-item__image-outer-wrapper
							product-chart-item__image-outer-wrapper--large">
							<div class="product-chart-item__image-wrapper">
								<img alt="LG Ultragear 34GN850 - Best budget ultrawide for gamers" class="product-chart-item__image" height="958" src="https://b2c-contenthub.com/wp-content/uploads/2022/07/LG-Ultragear-34GN850-03.jpg?quality=50&amp;strip=all" width="800" />
							</div>
						</div>
															<div class="product-chart-body">
						<div class="product-chart-columns">
							
								<div class="product-chart-column">
									<p class="product-chart-subTitle">Pros</p>
									<ul class="product-pros-cons-list">
															<li> 
					21:9 panel with a 34-inch screen					</li> 
										<li> 
					Curved monitor					</li> 
										<li> 
					Impressive gaming performance					</li> 
										<li> 
					Ergonomic adjustment options					</li> 
														</ul> 
								</div>
																					<div class="product-chart-column">
								<p class="product-chart-subTitle">Cons</p>
								<ul class="product-pros-cons-list">
														<li> 
					Only average power consumption					</li> 
										<li> 
					Expensive					</li> 
													</ul> 
							</div>
													</div>
					</div>
														</div>
						
					<div class="product-chart-item__information ">
														<div class="product-widget__information--rrp-wrapper">
										<span class="product-widget__information--rrp-label">
																			</span>
										<span class="product-widget__information--rrp-value">
																				</span>
									</div>
									
													<div class="product-chart-item__pricing-details ">
																	<span class="product-chart-item__pricing-details--label">
										Best Prices Today:
									</span>
																<span class="product-chart-item__pricing-details--links-wrapper">
																			<span class="not-amp">
										<a class="product-chart-item__pricing-details--link" href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.lg.com/us/monitors/lg-34gn850-b-gaming-monitor&amp;xcust=2-3-1470449-6-804143-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">699.99 at  LG</a><a class="product-chart-item__pricing-details--link" href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/B08HNJ26NL?tag=pcworld02-20&amp;linkCode=ogi&amp;th=1&amp;psc=1&amp;xcust=2-3-1470449-6-804143-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">$921.66 at  Amazon</a>										</span>
																		</span>
							</div>
											</div>
										<div class="product-content">
						
<p>The LG Ultragear 34GN850-B, released in 2020, was once the king of ultrawide gaming. It was dethroned by Alienware&rsquo;s AW3423DWF&mdash;and as a result LG has slashed the price. Originally $999.99, this monitor is now available for $699.99 (and sometimes less).</p>

<p>That&rsquo;s great news. Although surpassed by the Alienware, LG&rsquo;s Ultragear 34GN850-B is an attractive monitor with excellent color performance, good image clarity, and a bright, vivid picture. It has an enhanced refresh rate of up to 144Hz (with a 160Hz overclocked mode) and supports both AMD FreeSync and Nvidia G-Sync for smooth gameplay.</p>

<p>Its weakness? Contrast. The IPS panel scores lower in contrast than other monitors on this list, including the Asus ProArt PA348CV, which also has an IPS panel. The image can look hazy in darker scenes.</p>

<p>Connectivity is respectable with two HDMI ports, one DisplayPort, and two-port USB-A hub for connecting wired peripherals. The monitor also retains many of the features that would be expected of a high-end monitor including a sturdy ergonomic stand and attractive design.&nbsp;</p>
						</div>
											Read our full 
					<a class="product-chart-item__review-link" href="https://www.pcworld.com/article/804136/lg-ultragear-34gn850-review-2.html" target="_blank"> Review LG Ultragear 34GN850</a>
								</div>
			<div class="ad page-ad has-ad-prefix ad-article"></div>			<div class="product-chart-separator"></div>
			<div class="wp-block-product-chart-item product-chart-item">
									<div class="product-chart-item__title-wrapper">
						<h3 class="product-chart-item__title-wrapper--title product-chart-title " id="4-aoc-cu34g2x-best-budget-ultrawide">
							4.  AOC CU34G2X &ndash; Best budget ultrawide						</h3>
					</div>
													<div class="large-pro-cons-product-chart-section">
											<div class="product-chart-item__image-outer-wrapper
							product-chart-item__image-outer-wrapper--large">
							<div class="product-chart-item__image-wrapper">
								<img alt="AOC CU34G2X - Best budget ultrawide" class="product-chart-item__image" height="592" src="https://b2c-contenthub.com/wp-content/uploads/2022/11/61-ke7QpxL._AC_SL1000_.jpg?quality=50&amp;strip=all" width="901" />
							</div>
						</div>
															<div class="product-chart-body">
						<div class="product-chart-columns">
							
								<div class="product-chart-column">
									<p class="product-chart-subTitle">Pros</p>
									<ul class="product-pros-cons-list">
															<li> 
					Gaming monitor in ultrawide 21:9 format					</li> 
										<li> 
					Impressive gaming performance					</li> 
										<li> 
					Large 34-inch curved panel					</li> 
										<li> 
					Ergonomic adjustment options					</li> 
														</ul> 
								</div>
																					<div class="product-chart-column">
								<p class="product-chart-subTitle">Cons</p>
								<ul class="product-pros-cons-list">
														<li> 
					High power consumption					</li> 
													</ul> 
							</div>
													</div>
					</div>
														</div>
						
					<div class="product-chart-item__information ">
														<div class="product-widget__information--rrp-wrapper">
										<span class="product-widget__information--rrp-label">
																			</span>
										<span class="product-widget__information--rrp-value">
																				</span>
									</div>
									
													<div class="product-chart-item__pricing-details ">
																	<span class="product-chart-item__pricing-details--label">
										Best Prices Today:
									</span>
																<span class="product-chart-item__pricing-details--links-wrapper">
																			<span class="not-amp">
										<a class="product-chart-item__pricing-details--link" href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.amazon.com/dp/B07ZB2TNZZ?tag=pcworld02-20&amp;linkCode=ogi&amp;th=1&amp;psc=1&amp;xcust=2-3-1470449-6-804157-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">$399.99 at  Amazon</a>										</span>
																		</span>
							</div>
											</div>
										<div class="product-content">
						
<p>Ultrawide monitors have many perks, but low pricing is not among them. Fortunately, budget shoppers have one good option: the AOC CU34G2X, which retails at or below $349.99.</p>

<p>This monitor has a 34-inch ultrawide VA panel that, by most measures, performs surprisingly close to more expensive alternatives. It provides a good contrast ratio and delivers vivid color performance. It also has the same 3440&times;1440 resolution as the other monitors on this list, so it looks just as sharp. In truth, less demanding shoppers may find it difficult to notice any difference between this monitor and more expensive options like the Asus ProArt PA348CV.</p>

<p>The AOC CU34G2X is marketed as a gaming monitor and has an enhanced refresh rate of up to 144Hz. It doesn&rsquo;t officially support AMD FreeSync or Nvidia G-Sync, however, so gamers may have mixed results when trying to use these adaptive sync standards.</p>

<p>Though it punches above its price in image quality, the AOC CU34G2X&rsquo;s design looks cheap. It leans a bit too hard on an aggressive red-and-black gaming theme. That will annoy shoppers who prefer a calmer, less obtrusive look.</p>

<p>Connectivity is great, though, with two HDMI and two DisplayPort inputs plus a four-port USB-A hub. The monitor also has a height adjustable stand, a must-have perk that isn&rsquo;t guaranteed on budget ultrawide monitors.</p>
						</div>
											Read our full 
					<a class="product-chart-item__review-link" href="https://www.pcworld.com/article/804151/aoc-cu34g2x-gaming-monitor-review.html" target="_blank"> Review AOC CU34G2X</a>
								</div>
			<div class="ad page-ad has-ad-prefix ad-article"></div>		</div>

		


<h2 id="what-to-look-for-in-an-ultrawide-monitor">What to look for in an ultrawide monitor</h2>



<p>Ultrawide monitors are a favorite of PC enthusiasts, but remain a niche within the larger monitor market. This leaves shoppers with fewer options. Most ultrawide monitors have a 34-inch panel with a resolution of 3440&times;1440, and similar connectivity.</p>



<p>Still, these monitors can differ in several key areas. Here&rsquo;s what to look for.</p>



<h3 id="panel-type-is-a-big-deal">Panel type is a big deal</h3>



<p>Ultrawide monitors offer less choice in some regards but that script is flipped when it comes to panel type. Ultrawide monitors come in a variety of panel types: IPS, VA, and OLED.</p>



<p>IPS panels are common in mid-range and premium ultrawide monitors. This panel type delivers great color performance, high maximum brightness, superb sharpness, and good motion performance. It&rsquo;s weak in contrast, however, which can disappoint when viewing TV shows or movies.</p>



<p>VA panels are typically a budget option, though some are found in premium ultrawide monitors. They have better contrast than IPS panels and deliver similar color performance and brightness&mdash;however, budget VA panels tend to be merely okay in these areas. Most VA panels fall short in motion performance and may look blurry when playing fast-paced games.</p>



<p>OLED is king of the hill. It leads in color, contrast, and motion performance. Sharpness is often slightly reduced compared to IPS and VA, but most people will find it a minor downgrade. OLED also is the best choice for HDR.</p>



<p>In general, OLED is better than IPS, and IPS is better than VA. However, some people might prefer VA over IPS because it has a better contrast ratio and looks darker in dark content.</p>



<h3 id="a-height-adjustable-stand-is-a-must-have">A height-adjustable stand is a must-have</h3>



<p>All the monitors on this list provide an ergonomic stand that adjusts for height, tilt, and swivel. This is a must-have feature, but one that isn&rsquo;t found on the least expensive ultrawide monitors.</p>



<p>As tempting as it may be to save money on a budget model without a height-adjustable stand, you would regret it.</p>



<p>Ultrawide monitors are bulky and tend to require a larger, heavier stand, which in turn makes them more difficult to place on an elevated platform. The old college trick of sticking a monitor on a shoe box won&rsquo;t work.</p>



<h3 id="look-for-usb-c-but-dont-expect-it">Look for USB-C, but don&rsquo;t expect it</h3>



<p>USB-C compatibility is an excellent feature, and <a href="https://www.pcworld.com/article/612470/you-should-buy-a-usb-c-hub-monitor-heres-what-you-need-to-know.html">USB-C hub monitors</a> can clear away tons of clutter on your desk. Unfortunately, many ultrawide monitors don&rsquo;t support USB-C yet, or have limitations that detract from the USB-C port&rsquo;s usefulness.</p>



<p>Asus&rsquo;s ProArt PA348CV, our favorite ultrawide for professionals, is one exception. It has a USB-C port with up to 90 watts of Power Delivery, and the port drives a USB-A hub with four downstream ports.</p>



<p>Dell, HP, and BenQ also offer ultrawide monitors with USB-C. Most of these lack an enhanced refresh rate, however, and they&rsquo;re typically more expensive than the Asus.</p>



<h3 id="pricing-is-important-and-can-swing-wildly">Pricing is important&mdash;and can swing wildly</h3>



<p>Monitor pricing is always important, but it&rsquo;s key for ultrawide monitors. Although very expensive at MSRP, ultrawide monitors routinely see huge price cuts during seasonal sales. They also receive major semi-permanent price cuts later in their life.</p>



<p>The LG Ultragear 34GN850-B is an example of this. Originally sold for $999.99, it&rsquo;s now routinely available for $699.99, and went as low as $599.99 during Amazon&rsquo;s Black Friday sale. That&rsquo;s a 40 percent reduction in price! Waiting for a deal can save you hundreds.</p>



<h3 id="dont-buy-an-ultrawide-for-console-gaming">Don&rsquo;t buy an ultrawide for console gaming</h3>



<p>A quick word of warning: You should not buy an ultrawide monitor if you plan to connect a game console frequently. &nbsp;</p>



<p>Game consoles don&rsquo;t support ultrawide aspect ratios, so you&rsquo;ll see black bars on either side of the image. That&rsquo;s unattractive and wastes the monitor&rsquo;s potential. It&rsquo;s best to stick with a widescreen monitor if console gaming is a priority.</p>



<h2 id="how-we-test-monitors">How we test monitors</h2>



<p>PC World&rsquo;s team of staff and freelance reviewers conduct in-depth testing to compare monitors across a wide range of categories and price points. We test dozens of monitors each year to find the best pick for every category and price point.</p>



<p>Our testing uses a SpyderXElite color calibration tool. It delivers objective, unbiased measurements for a wide range of metrics including brightness, contrast, color gamut, color accuracy, color temperature, and gamma. Results are recorded and logged for future comparison. This allows our experts to easily compare many monitors at once and eliminates subjective bias from the results.</p>

Monitors</div>

## Learn Python while this bundle is specially discounted
 - [https://www.pcworld.com/article/1471959/learn-python-while-this-bundle-is-specially-discounted.html](https://www.pcworld.com/article/1471959/learn-python-while-this-bundle-is-specially-discounted.html)
 - RSS feed: https://www.pcworld.com/index.rss
 - date published: 2023-01-13 08:00:00+00:00
 - user: None

<div id="link_wrapped_content">
<section class="wp-block-bigbite-multi-title"><div class="container"></div></section>



<p>If you want to learn to code this year, there&rsquo;s no better place to start than with Python. Considered one of the best first languages to learn because of its relatively intuitive syntax and general-purpose nature, you can get up to speed with&nbsp;<a href="https://shop.pcworld.com/sales/the-2021-premium-python-certification-bootcamp-bundle?utm_source=pcworld.com&amp;utm_medium=referral&amp;utm_campaign=the-2021-premium-python-certification-bootcamp-bundle&amp;utm_term=scsf-561535&amp;utm_content=a0x1P0000057uN1QAI&amp;scsonar=1" rel="noreferrer noopener" target="_blank">The Premium Python Certification Bootcamp Bundle</a>.</p>



<p>This extensive bundle includes&nbsp;<a href="https://shop.pcworld.com/sales/the-2021-premium-python-certification-bootcamp-bundle?utm_source=pcworld.com&amp;utm_medium=referral&amp;utm_campaign=the-2021-premium-python-certification-bootcamp-bundle&amp;utm_term=scsf-561535&amp;utm_content=a0x1P0000057uN1QAI&amp;scsonar=1" rel="noreferrer noopener" target="_blank">13 courses designed for absolute beginners</a>&nbsp;to elevate their programming skills over time. You&rsquo;ll learn how to set up a Python project, how to utilize variables and operators, discover how to manage data, control program flow, use functions for program execution, and much more. As you work, you&rsquo;ll get more familiar with object-oriented programming and learn some of the more complex applications of Python. From ethical hacking to&nbsp;<a href="https://go.redirectingat.com/?id=111346X1569483&amp;url=https://www.pcmag.com/opinions/the-artificial-intelligence-we-fear-is-our-own&amp;xcust=2-1-1471959-1-0-0&amp;sref=https://www.pcworld.com/feed" rel="nofollow" target="_blank">artificial intelligence</a>, image processing, and more, you&rsquo;ll get a comprehensive understanding of this scalable language.</p>



<p>Learn Python while&nbsp;<a href="https://shop.pcworld.com/sales/the-2021-premium-python-certification-bootcamp-bundle?utm_source=pcworld.com&amp;utm_medium=referral&amp;utm_campaign=the-2021-premium-python-certification-bootcamp-bundle&amp;utm_term=scsf-561535&amp;utm_content=a0x1P0000057uN1QAI&amp;scsonar=1" rel="noreferrer noopener" target="_blank">The Premium Python Certification Bootcamp Bundle</a>&nbsp;is on sale for a specially reduced price. Grab it for just $29.99 now.</p>



<p><a href="https://shop.pcworld.com/sales/the-2021-premium-python-certification-bootcamp-bundle?utm_source=pcworld.com&amp;utm_medium=referral-cta&amp;utm_campaign=the-2021-premium-python-certification-bootcamp-bundle&amp;utm_term=scsf-561535&amp;utm_content=a0x1P0000057uN1QAI&amp;scsonar=1" rel="noreferrer noopener" target="_blank">&nbsp;</a></p>


<div class="extendedBlock-wrapper block-coreImage undefined"><figure class="wp-block-image"><img alt="" src="https://cdnp0.stackassets.com/cad160c46cc376951a70536b5f592363c8c835e7/store/2631205dd808135498fb87c7cd933e9b3199feddfca78a02e7da4ee28696/sale_183438_primary_image.jpg" /></figure></div>



<p><strong>The Premium Python Certification Bootcamp Bundle &ndash; $29.99</strong></p>



<p><a href="https://shop.pcworld.com/sales/the-2021-premium-python-certification-bootcamp-bundle?utm_source=pcworld.com&amp;utm_medium=referral-cta&amp;utm_campaign=the-2021-premium-python-certification-bootcamp-bundle&amp;utm_term=scsf-561535&amp;utm_content=a0x1P0000057uN1QAI&amp;scsonar=1" rel="noreferrer noopener" target="_blank">See Deal</a></p>



<p>Prices subject to change.</p>

Professional Software</div>
