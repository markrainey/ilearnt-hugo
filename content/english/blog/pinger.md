---
title: "Pinger - a simple network diagnostic tool"
meta_title: ""
description: "Tracking down network issues with Pinter"
date: 2026-01-28T11:51:00
categories:
  - Technology
  - Coding
author: Mark Rainey
tags: []
draft: false
---
I am in the UK and my Internet connection is provided by Virgin Media - there I have admitted it.

Those who have experienced the "joys" of Virgin Media know that this means my connection sometimes decides to go on a journey to another place and either breaks completely or becomes unstable.

At home I run a Linksys mesh network which works brilliantly most of the time but occasionally also gets a bit confused.

My go to tools tended to be [Google Speed Test](https://www.google.com/search?q=google+speed+test&udm_14) and [Packet Loss Test](https://packetlosstest.com/). This would help confirm whether there was an issue but it didn't help me track down which part was the problem.

This is why I wrote [Pinger](https://github.com/markrainey/Pinger).

To test when things had gone wrong I would ping my router and then ping a site on the Internet. If it can get to the former but not the latter then the chances are the problem is with Virgin Media.  
  
To automate this I wrote Pinger so I could ping multiple addresses at the same time and display the times if any of them are outside certain constraints. At the moment I ping the router, the external IP address of the router and the BBC news site.

It is just a console application written in C# (you will need to build it yourself). You can edit the configuration file to define the addresses you want to ping. It can also log the results to a file if you need "evidence" for your ISP.

If things become unstable or I lose connection I just launch Pinger and it gives me a very quick indication of where the problem might be. The resolution usually involves going around the house and rebooting various network boxes or running the Virgin Media website status check and then waiting for status updates as they fix it (hopefully).
