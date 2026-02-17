---
title: "Weird blog traffic"
meta_title: ""
description: "An unexpected spike in blog traffic and the reason behind it"
date: 2026-02-17T10:09:00
categories:
  - Technology
author: Mark Rainey
tags: []
draft: false
---

This blog has seen a recent up-tick in views and that would normally be a good thing. However this up-tick has been a bit unusual.

I use Google Analytics to provide an overview of the traffic to this blog. I also pass traffic through the free tier of Cloudflare so I can also get a different view there.

A few months ago I was fortunate to have an article included in the [ChangeLog newsletter](https://changelog.com/news/120). This created a brief big spike in traffic. A few weeks ago I also had an article included in the [CTO Craft newsletter](https://www.techmanagerweekly.com/tmw-467/?ref=tech-manager-weekly-newsletter) and this also saw a spike. 

I started seeing more traffic on a daily basis. My initial view was "yay, people are reading my ramblings". However I noticed that it nearly all came from Singapore and China, and in particular Lanzhou. 

Last week Wired posted an [article](https://www.wired.com/story/made-in-china-niche-websites-are-seeing-a-surge-of-mysterious-traffic-from-china/) (behind a paywall unfortunately) about how lots of different sites are seeing a similar spike in traffic from these places. They seem to be related to bots being used to train AI.

As this was distorting my stats I decided to try and take action to prevent this. After a bit of research one approach suggested adding some rules in Cloudflare. 

I went to "Security / WAF". I added clicked on "Create Rule" and added a custom rule. For the Chinese traffic this involved selecting "Country" equals "China" then adding an additional "And" with "Known Bots" and the radio button turned off.

The expression preview looks like this

> (ip.src.country eq "CN" and not cf.client.bot)

I added a similar one for Singapore. 

It's only been a couple of days but it looks like my number of views has dropped (boo!) but it also appears that is due to the reduced traffic from these two sources (yay!).


