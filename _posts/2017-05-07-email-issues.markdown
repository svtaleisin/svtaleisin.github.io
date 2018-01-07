---
title: Email Issues
modified:
categories: 
tags: []
published: true
date: 2017-05-07T06:49:50+12:00
---

It would appear that I messed up  the email system with the last post. Hopefully
this issue will not re-occur in the  future since, I've added an automated check
before updating the blog.

If   you're  not   technical  then   you  can   stop  reading   now  and   click
through   at   the  bottom   of   the   email   to   previous  post   or   click
[here](http://www.taleisin.com/river-adventures/).

---

<!--more-->

If you're technical and care about what went wrong...

Mailchimp cannot deal with relative urls in the rss feed. This means that I have
to tell Jekyll  to use absolute urls.  If I'm using absolute urls  I cannot test
the blog  on my  local machine since  the links  all point to  the live  site. I
thought I had solved the issue by  changing the config file with a script before
serving  locally and  deploying remotely.  Clearly something  went wrong  in the
script (which  works when I test  it, you know the  old "it works on  my machine
excuse"). I've now added a condition to  the deploy script to only deploy if the
absolute urls are present in the rss feed.

In theory this should  prevent broken links in emails going  forward, but if 20+
years in  IT has  taught me  anything... This too  will be  proven wrong  in the
future.
