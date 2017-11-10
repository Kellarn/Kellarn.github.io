---
layout: post
title:  "Robots and Humans"
date:   2017-11-10 15:01 +01
categories: Robots and humans
author: Sebastian Källstedt
comments: true
---

### Q: What is robots.txt and how have you configure it for your site?

Robots.txt is a text file that is placed in the root of your site. This file tells all type of robots that are used by for example search engines and others that wants to index your site, what they are allowed to index. These robots are also known as for example Crawlers or spiders and they are basically programs that travele the web automatically. These robots are also used in bad ways by scammers that try to find email adresses from websites. Even though you have a robots.txt on your site these robots can ignore your setup so that they can index or search your sites anyway, so it is not a safe way to try to hide something on your website.

This is how I have set up my robots.txt on my site:

{% highlight html %}
User-agent: *
Disallow:
{% endhighlight %}

This means that I allow all robots to index all of my sites. I know this means that my email might get spammed, but for now I am willing to see how this works to see if there are actually any robots on my site.


### Q: What is humans.txt and how have you configure it for your site?

Humans.txt is basically just a text file that contains information about the site. This is meant for humans to read to it doesn't include any sort of code or anything else. This files ususally contains information about the people who built the site, the owner,special thanks or other meantions and development tools.

My humans.txt file have information about my site, where it was built, some special thanks and when and where it was last updated. 

{% highlight html %}

                            
/* TEAM */

                            
Developer: Sebastian Källstedt
Designer: Sebastian Källstedt

                            
Contact: Sebastian@kallstedt.com

Github: Kellarn
                            
Location: Kalmar, Sweden.

                         
                 
                        [...]
						

							
/* THANKS */

							
Name: Johan Leitet , Mats Loock

						
                 
                        [...]
                        

                            
/* SITE */

                            
Last update: 2017/11/10

                            
Standards: HTML5, CSS3

                            
Components: SASS, JEKYLL, DOCKER

                            
Software: Visual Studio Code, Adobe Illustrator
{% endhighlight %}


