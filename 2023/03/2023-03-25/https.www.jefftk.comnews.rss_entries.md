# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Reproject on Cropping
 - [https://www.jefftk.com/p/reproject-on-cropping](https://www.jefftk.com/p/reproject-on-cropping)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2023-03-25 08:00:00+00:00

<p><span>

Sometimes you'll come across a picture that looks all skewed, usually
where someone cropped a small piece out of the corner of something
larger:

</span>

<p>

<a href="https://www.jefftk.com/standard-corner-crop-big.jpg"><img class="mobile-fullwidth" height="443" src="https://www.jefftk.com/standard-corner-crop.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Projecting a 3D scene to make a 2D picture unavoidably introduces
distortion, worse the farther you are from the center, so if you crop
to just the corner of a picture you're getting a lot of distortion.

</p>

<p>

It would be possible to make this better: your phone knows the
distortions its lens makes, and every time you crop something it could
automatically reproject the image.  I can approximate correction with a
vertical shear:

</p>

<p>

<a href="https://www.jefftk.com/shear-y-corner-crop-big.jpg"><img class="mobile-fullwidth" height="443" src="https://www.jefftk.com/shear-y-corner-crop.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Followed by a horizontal scale:

</p>

<p>

<a href="https://www.jefftk.com/shear-y-scale-x-corner-crop-big.jpg"><img class="mobile-fullwidth" height="443" src="https://www.jefftk.com/shear-y-scale-x-corner-crop.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

In writing this up, however, I realized that my phone's (Pixel 5a)
camera app takes a different approach.  Instead of waiting for you to
crop an image, it automatically fixes faces itself.  The pictures
above were taken with Open Camera, which doesn't have these smarts;
here's what I get with the default camera app:

</p>

<p>

<a href="https://www.jefftk.com/pixel-photos-corner-crop-big.jpg"><img class="mobile-fullwidth" height="465" src="https://www.jefftk.com/pixel-photos-corner-crop.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

It made the fix initially, not on cropping; the full-size image also
minimizes distortion around my face:

</p>

<p>

<a href="https://www.jefftk.com/uncropped-corner-distortion-fixed-big.jpg"><img class="mobile-fullwidth" height="412" src="https://www.jefftk.com/uncropped-corner-distortion-fixed.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Since this is only applied to my face, though, and not the rest of my
body, it does give a slightly uncanny effect.  Compare to the
full-size version of the Open Camera image:

</p>

<p>

<a href="https://www.jefftk.com/uncropped-no-correction-big.jpg"><img class="mobile-fullwidth" height="412" src="https://www.jefftk.com/uncropped-no-correction.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

You can see what the Pixel camera app did around my face by looking at
the line of the bookcase:

</p>

<p>

<a href="https://www.jefftk.com/pixel-photos-corner-crop-annotated-big.jpg"><img class="mobile-fullwidth" height="465" src="https://www.jefftk.com/pixel-photos-corner-crop-annotated.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

In real life and in a raw photo that line would be straight:

</p>

<p>

<a href="https://www.jefftk.com/standard-corner-crop-annotated-big.jpg"><img class="mobile-fullwidth" height="443" src="https://www.jefftk.com/standard-corner-crop-annotated.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

And in my manually corrected version from above the line is straight:

</p>

<p>

<a href="https://www.jefftk.com/shear-y-scale-x-corner-crop-annotated-big.jpg"><img class="mobile-fullwidth" height="443" src="https://www.jefftk.com/shear-y-scale-x-corner-crop-annotated.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

But because the Pixel camera is doing its correction on the whole
image, instead of waiting for you to crop, it isn't able to preserve
all the straight lines in the original image.

</p>

<p>

I think the Pixel edit is probably still worth doing, since we care a
lot about faces and they do look more natural projected as if you were
looking straight at them.  Reprojecting the whole image to minimize
distortion when you crop would also be a pretty nifty feature, and
doesn't introduce the kind of distortions that fixing one part of a
larger image does.

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0ZuTgZRhEVknkSr4yeNV6mqq119Fdo2o6rSAnqEa4mTwmwLBtSk1C94mQmaartYPul">facebook</a>, <a href="https://lesswrong.com/posts/Q47fsq4CeTtgEFLvm">lesswrong</a>, <a href="https://mastodon.mit.edu/@jefftk/110086126826900225">mastodon</a></i></p>

