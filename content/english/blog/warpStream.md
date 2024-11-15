---
title: "Thinking differently can be worth a lot"
meta_title: ""
description: "A company took an existing product, flipped some assumptions and got bought for $220m"
date: "2024-11-15T07:12:00"
categories:
  - Technology
author: Mark Rainey
tags: []
draft: false
---

We use the technology Apache Kafka as a key element in the implementation of the distributed ledger we have developed.

It provides us with a way to send messages between components, partition them up in a deterministic way and consume them in multiple places in the same order in each partition.

This is nothing new, lots of companies use it this way.

However, a company called [WarpStream](https://www.warpstream.com/) looked at Kafka and decided that there was a gap in the market that they could exploit. They realised that not all scenarios rely on it being fast with low latency. A large number are about high volumes where latency is much less of a driving factor.

With this in mind, they have developed an API compatible implementation that runs in the cloud. Their approach allows them to massively simplify the deployment and operations. It uses Amazon S3 storage as the underlying store for the data which is much slower however the upside is that it is significantly cheaper than the current approach.

These decisions mean that it is about 5-10x cheaper to run and the operations overhead is smaller. As long as you don't mind the latency it is a significant win.

Confluent, the maintainers of Apache Kafka, realised the impact this could have, especially to their business, and bought WarpStream for $220m - about a year after the company started.

By identifying a specific use case for an existing product and producing a compatible solution with different operational requirements, WarpStream were not only able to open up new market opportunities, they were able to cash in.

*Are there other opportunities where rethinking the requirements or the constraints could open up a market for a product?*

For a brilliant and more detailed explanation see this X [thread](https://x.com/BdKozlovski/status/1852725315203653841).

__Links__

[WarpStream - An Apache Kafka Compatible Data Streaming Platform](https://www.warpstream.com/)


[X thread](https://x.com/BdKozlovski/status/1852725315203653841)
