---
title: "Innovation tokens"
meta_title: ""
description: "Should you bring in new technologies or just stick with the boring ones?"
date: "2025-01-02T17:31:00"
categories:
  - Work
  - Technology
author: Mark Rainey
tags: []
draft: false
---
When you work in technology it is tempting to bring in the new exciting technologies that claim to make your life easier, run faster and bring you rainbow unicorns every day.

Sometimes it is better to stick with the boring technologies.

I really like an approach in this [article](https://mcfunley.com/choose-boring-technology) where Dan McKinley talks about "Innovation Tokens". As it is from 2015 the example technologies given below would now probably be considered boring but the idea holds if you consider they were new at the time: 

> Let’s say every company gets about three innovation tokens. You can spend these however you want, but the supply is fixed for a long while ... If you choose to write your website in NodeJS, you just spent one of your innovation tokens. If you choose to use MongoDB, you just spent one of your innovation tokens. If you choose to use service discovery tech that’s existed for a year or less, you just spent one of your innovation tokens. If you choose to write your own database, oh god, you’re in trouble.

He emphasises that boring does not mean bad. It just means that it has been around for a long time and we know how it operates - especially when failures occur.

When I worked at a hedge fund we developed a real time market data system. It would receive very large amounts of price data and then distribute them to the relevant users and their applications. We developed it using Streambase (one of the first streaming platforms) and Vertica (the first commercial column database). In fact the latter was not even in production when we started developing with it.

Our system worked and we even won an award for it but the use of these technologies meant that it was more difficult to maintain and also recruit people to work on it. We easily used up all our innovation tokens and then some. We hit the issues around not knowing how failures are best handled. However we would not have been able to deliver a system with the required performance at that time without these new technologies.

On the system I am involved in at the moment we make sure we justify the introduction of any new technologies - we don't just introduce them for the sake of it. 

And we did write our own complex database - our main initial product - in the form of a distributed ledger.

The key takeaway for me is to stop and consider whether adding a new technology is really required and the best approach - and are you willing to spend one of your innovation tokens to do so?

__Links__

[Choose Boring Technology](https://mcfunley.com/choose-boring-technology)