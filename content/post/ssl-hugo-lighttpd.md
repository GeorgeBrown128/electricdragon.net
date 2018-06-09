+++
date = "2016-04-28T23:47:16Z"
description = ""
draft = true
tags = ["development", "website", "ssl"]
title = "An SSL Website with Hugo and Lighttpd"
topics = ["hugo", "website"]
+++

As I mentioned in a [previous post]("website-in-hugo/"), the process of
getting the website up and running with hugo was very quick. I decided I also
wanted to set up SSL encryption. I acknowledge since my website is entirely
open source this may seem a little OTT, but it's a nice thing to add, and was
very easy to do!

## 1 Server Software

I'm using a small VPS to host my site. It runs Ubuntu server, which is a nice
platform to run on, though just about any flavour of Linux should work fine.

The first thing to install is Hugo. Hugo is currently distributed as an
executable you can just drop onto your machine.

You'll also want some software to serve up webpages. Hugo is able to act as a
webserver if you want, however it can't do anything terribly advanced. I've
opted for Lighttpd, since it is easy to configure, and as its name suggests,
is light on my limited VPS resource.

Finally you'll need to install letsencrypt. This is a free automated SSL
certificate tool. It seems the mechanism is to place some files on your
website, ask the authentication server to check their presence, and then if it
finds the right files, you're rewarded a letsencrypt certificate. As far as I
can tell, the letsencrypt certs are just as trusted as anybody else's. Let's
hope they stay that way!

## 2 Generate Some Content

The very first step to setting up the website is to get some content prepared
for it. Hugo is used to
