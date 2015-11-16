---
layout: post
title:  "1dv022 - Examination 1"
date:   2015-11-07
categories: jekyll update
author: Fred
---
# Answers to examination questions

### What do you think of pre-compiling your CSS? 
* Compare to regular CSS

With SCSS you can use variables, mixins and other cool stuff since you compile the files
later on an produces usable CSS files for the sites.
DRY, with SCSS you re-use the code on multiple pages.
Easy to complicate if you start nesting away.
A steaper learning curve then regular CSS since you add another layer of complexity.

* Which techniques did you use?

[SASS][sass-home]

* Pros and Cons?

Modular is good.
Easy to use but take some time getting the hang off.
There are numerous frameworks to be used with SASS.
A large community and it's more or less industry approved.
It's been around.

### What do you think of static site generators?
* What type of projects are they suitable for?

This could be used for larger projects but the sweetspot are smaller sites that
are needed fast. SSG are also very secure and are easy to maintain. Blog posts
are also very fast to write and publish.

* Personal page with a blog.
* Projects not needing real-time updates of content or user input
* Sites that need to be established fast and maybe just for a short period

My personal view is that a SSG suits me since it's fast, pretty secure, version controlled if using GIT and
not generating a lot of traffic.
It allows me to good control of the contect, easy to update and I can run it with Git-pages.


### What is robots.txt and how have you configured it for your site?
Robots.text is a text at the root indicating parts of your website you don't want
to be accessed by searchengines. It uses an [exclusion standard][robot-standard] that 
indicates what kind of access these engines are allowed or disallowed to have.
This information is how ever NOT mandatory to follow, they are more of a  suggestion.

I did allow Google to index my site but any other engine are not allowed.

### What is humans.txt and how have you configured it for your site?
[Humans.txt][humans-home] is also a textfile containing information about the people being involved
in the website. Could also include people you like to thank for inspiration and/or help.
It is a kind of appreciation for the hard work that's being put into the project.

I added a textfile under the root and wrote about the people that done the work(me!) and
also the people that have inspired me and helped me.

### How did you implement comments to blog posts?
I used Disqus for the comments on the page.
In the YAML front of the post.html I added "comments=true". Included provided code in a new file
called disqus.html under /_include and included that in the file for posts(post.html).
For now I enable comment on all blogposts, will most likely change so I have to enable it
on individual posts later on.

### What is Open Graph and how do you make use of it?
This protocol enables a website to have multiple social objects.
It's done through adding metadata to the head of the webpage. There are four required properties.

Since there are so many options you could have using liquid I created a new file "opengraph.html" 
and included that in my "head.html".

#### Required properties:
* title
* type
* image
* url


[robot-standard]:   https://en.wikipedia.org/wiki/Robots_exclusion_standard
[humans-home]:      http://www.humanstxt.org
[sass-home]:        http://www.sass-lang.com