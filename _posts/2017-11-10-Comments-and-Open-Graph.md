---
layout: post
title:  "Comments and Open Graph"
date:   2017-11-10 15:21 +01
categories: Comments and open graph
author: Sebastian Källstedt
comments: true
---

### Q: How did you implement comments to blog posts?

I implemented disqus as my comment provider. Disqus was easy to implement and gave clear instructions of how to set up.
Currently my disqus code is in post.html because this page is currently on local and not hosted on Github pages. 
This project from jekyll came with a pre defined disqus_comments.html in the _includes folder but that code seemed to need an actuall url to work proporlly. I will try to implement this when I have hosted my site on GH pages. 

The disqus comment system and how to implement it is done by setting up a function in the html file that uses my disqus account name to create a script that creates the the comment section by using some javascript code. It loads fast and looks good and will be my choice for future projects. 

### Q: What is Open Graph and how did you make use of it?

Open Graph is a protocoll that enables web pages to become rich objects in a social graph. This means that if I am to share my site on for example facebook it allows my site to have the same functionality as any other object on Facebook. The protocol pretty much tells Facebook in this case how my site should look and what information that should be presented when shared. To do this you have to add some metadata to your site. The most common ones and also the ones I have used on my site is title, type, image and url.

I added this metadata to my head.html file since this file is included in every other page that is created on my site. This is how it looks when added:

{% highlight html %}

<meta property="og:title" content="Seb's hangout!" />
<meta property="og:type" content="About.blog" />
<meta prpoerty="og:url" content="https://kellarn.github.io" />
<meta property="og:image" content="/Seb.png" />

{% endhighlight %}