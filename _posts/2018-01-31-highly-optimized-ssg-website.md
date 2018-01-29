---
layout: post
title: "Highly Optimized SSG Website"
date: "2018-01-31 14:17:07 -0400"
---

Over the last two weeks I have been rebuiling a [website meant for walking users through the greenhouse planning process](https://greenhouse.planning.solar/){:target="_blank" }. Most of the content was redeveloped from [the old site](http://greenhouseplanning.com/){:target="_blank"}{:target="_blank"}. Take a second and look at both and note the overt user experience improvements.

The site was designed to be highly optimized, using a [Static Site Generator](https://www.staticgen.com/){:target="_blank"} as it's pseudo content management system. This is adventageous because non-technical users will never update the site, only a web developer. So we're able to take the compilation out from the runtime of the server and precompile all the assets statically. This means pages get served to the client much quick, because they don't have to wait for the server to generate them.

The site performs exceedingly well in speed tests. Using Google's [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/){:target="_blank"}, I was able to bring the pagespeeds to:

* Mobile Speed: 99/100
* Desktop Speed: 98/100

Through another performance grading tool, [Website Grader](https://website.grader.com){:target="_blank"}, the site performed equally as well:

* Performance: 27/30
* Mobile: 30/
* SEO: 30/30
* Security: 10/10

On my network I'm able to load the homepage in ~0.5 seconds with a page size of 334KB. The pages are being served up through an [NGINX](http://nginx.org/){:target="_blank"} webserver. The sites are hosted on a scaleable 

This website structure is highly advantageous with how well optimized it can be. Future plans would be to include a [JavaScript Framework](https://en.wikipedia.org/wiki/Comparison_of_JavaScript_frameworks){:target="_blank"} with [RESTful services](https://en.wikipedia.org/wiki/Representational_state_transfer){:target="_blank"} for more dynamic content that spans several websites. I'm leaning towards [AngularJS](https://angularjs.org/){:target="_blank"} however [EmberJS](https://www.emberjs.com/){:target="_blank"} might make more sense for this usecase.

There's a few other hidden surprises within this latest website build. I'm hoping to show these off in the coming months.

