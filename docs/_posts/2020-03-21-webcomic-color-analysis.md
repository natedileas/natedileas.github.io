---
layout: post
title: Webcomic Color Analysis
date: 2020-03-21 01:40
author: ndileas
comments: true
categories: [code, comics, imsci, Uncategorized]
---

<p>I read a lot of webcomics. Some of my favorites have had huge style changes over their run, like <a href="http://questionablecontent.net/">QC</a> and <a href="https://www.gogetaroomie.com/">GGAR</a>. Others, the artist was already pretty set on a format and style (<a href="https://betweenfailures.com/">Between Failures</a>, <a href="https://www.dumbingofage.com/">Dumbing of Age</a>). </p>



<p>I'm also a huge nerd, specifically about images. So I thought it might be interesting to merge the two, and answer a question at the same time: What does a comic strip look like in a single image?</p>



<figure class="wp-block-image alignwide size-full"><img src="https://natedileas.files.wordpress.com/2020/03/qc_slit_20-03-20-21-30-53.png" alt="" class="wp-image-58" /><figcaption>QC (2003 - Present): Over 4,000 strips combined.</figcaption></figure>



<p>^ This, in one visualization!</p>



<p>Savvy readers may be able to do some interesting analysis here. This image is about 4.2k pixels wide, over 17 years of comics. You can see the rise and fall of the blue apartment, coffee of doom, and all sorts of other interesting stuff. Even without any context, it's pretty neat.</p>



<p>This visualization is one view of larger dimensional space. There are many others, but this is the one I liked the best for the images I tried. To do this, I downloaded each image, converted to Lab space, and ran k-means over the results. I don't really want to write too much about process, so if you want to look at my code it's <a href="https://github.com/natedileas/comic-colors">here</a>. I was partially inspired by this site: http://mkweb.bcgsc.ca/color-summarizer/?faq</p>



<p>What I do want to look at is other webcomics! Here are the results for some of the others mentioned in the intro.</p>



<div class="wp-block-group"><div class="wp-block-group__inner-container">
<div class="wp-block-columns">
<div class="wp-block-column">
<figure class="wp-block-image size-full"><img src="https://natedileas.files.wordpress.com/2020/03/doa_slit_20-03-18-20-43-37.png" alt="" class="wp-image-52" /><figcaption>Dumbing of Age. This comic has had new strips nearly every day since 2010.</figcaption></figure>




<div class="wp-block-column">
<figure class="wp-block-image size-full"><img src="https://natedileas.files.wordpress.com/2020/03/btf_slit_20-03-20-20-08-00.png" alt="" class="wp-image-56" /><figcaption>Between Failures. The switch from black + white to color is very distinctive.</figcaption></figure>






<p>Are there other webcomics that would look cool this way? Let me know!</p>

