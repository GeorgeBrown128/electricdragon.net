+++
date = "2016-04-28T15:32:51+01:00"
description = "A Journey into the World of Static Website Generation"
draft = false
tags = ["development", "website"]
title = "Building a Website in Hugo"
topics = ["hugo", "website"]
+++

For a long time, I was running a webserver that served up a few handwritten 
HTML pages. I'd used the [Bootstrap](http://getbootstrap.com/) to try and make 
the content a bit prettier, but it was never that great. In addition I was 
rarely able to add content, since writing HTML is a relatively slow and boring 
process.

My friend [Harry Beadle](http://harrybeadle.co.uk/) showed me how he'd started 
writing his website in markdown, using [Jekyll](https://jekyllrb.com/) to 
convert the files into a complete website.

While this solution looked quite exciting, but I was reluctant to set up 
[Ruby](https://www.ruby-lang.org/en/). Ruby didn't seem terribly lightweight - 
and being a student I don't have a huge chunk of money to pour into server 
solutions! [StaticGen](https://www.staticgen.com/) links to a plethora of 
static site generators. I settled on [Hugo](http://gohugo.io/), which promises 
to be fast and light, and works in [Go's](https://golang.org/) comparatively 
simple ecosystem.

With the executable on my machine, I had a pretty website up and running in 5 
minutes, using the [Blackburn](http://themes.gohugo.io/blackburn/) theme.

From there it was a simple case of writing documents in markdown, a process 
which I was more than familiar with! So far it's looking very promising!
