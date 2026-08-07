---
title: "Is AI going local?"
meta_title: ""
description: "The move from large AI providers to local and self hosted"
date: 2026-08-07T08:38:00
categories:
  - AI
author: Mark Rainey
tags: []
draft: false
---
AI about to be disrupted with a move to local compute - your phone, your computer - driven by a swarm of agents.

## Overview

AI is hitting physical and operational bottlenecks, from data centre power grids to RAM availability to software code review queues. As open-source models improve, the ideas behind Eliyahu Goldratt’s Theory of Constraints and Clayton Christensen’s Disruptive Innovation, tied to computing's historical pendulum between central and distributed architectures, means processing will inevitably shift from massive central clouds down to "local" hardware.

## Goldratt's Bottlenecks

In *The Goal*, Eliyahu Goldratt highlights that any system is limited by its single tightest constraint. At the moment there are a number of constraints that are restricting the application of AI. 
* **Hardware supply bottlenecks:** Huge demand for data centres, high-bandwidth RAM, and raw electrical grid output creates severe physical limits on centralised AI.
* **Software workflow bottlenecks:** In software development, AI can generate code instantly, but human code reviews create a massive context-switching bottleneck.
* **Pricing:** A lot of companies went all in on AI, not realising that the costs at the time were effectively subsidised by the AI providers. When this was removed companies introduced constraints on usage of AI, either in terms of the models being used or the amount it is used overall.

Pushing harder on a system without clearing the bottleneck just creates inventory (or queue) pileups and moves the bottleneck. Solving the code review queue may just move it to a testing or maintenance bottleneck. Throwing money and hardware at the infrastructure issues may solve that problem but another bottleneck will spring up somewhere. 

## Christensen’s Disruption: The Rise of "Good Enough" Local Models

Clayton Christensen showed how lower-end, cheaper technologies start off inferior, hit a "good enough" threshold for everyday tasks, and eventually disrupt incumbent high-end solutions. AI appears to be on that journey. At the moment the top models are leading the way but the open source models, particularly from China, are catching up quickly and soon we may get to a point where you start to question why you are paying for the top models when cheaper ones are good enough.

* **Open-source & efficiency:** Model quantization, pruning, and targeted architecture improvements are shrinking parameters, and hence the resources needed to run them, while maintaining output quality.
* **Local intelligence:** Most everyday tasks do not require a trillion-parameter model running in a distant server farm. A smaller model running on a laptop or phone is faster, cheaper, and private.

People are using the best models as it is the easiest option or the cheaper models are not quite good enough. This will change. Some tasks will still need the top models and people will be willing to pay for them but it could be massively disruptive to the current commercial leaders such as Anthropic and OpenAI.

## The Pendulum: Centralised vs. Distributed Computing Cycles

Tech history moves in predictable cycles, swinging between distributed and centralised computing.

* Mainframes (Centralised) to Personal Computers (Distributed)
* Server Architecture (Centralised) to Mobile Apps & Local Storage (Distributed)
* Cloud Computing (Centralised) to Edge Computing & Local AI (Distributed)

Each shift occurs when local hardware becomes powerful enough and centralised costs or latency become too high. We have seen this over and over again and it seems to be starting to happen in the AI world. 

Enterprises had mainframes with terminals. They introduced PCs with networks. They moved to self hosted data centres and then to the cloud. They have started using AI from providers but this is likely to head towards AI on the device and self hosted AI.

## Jevons Paradox: Increased Demand

Jevons Paradox proposes that as a technology makes the use of a resource more efficient, the total consumption of that resource often increases rather than decreases, because lower costs unleash massive elastic demand. 

As AI models become dramatically cheaper, faster, and more efficient to run per task, the intuitive assumption is that companies will simply use fewer resources or cut workforce hours to produce the same output. However, Jevons Paradox suggests the exact opposite: dramatically lowering the marginal cost of intelligence causes total demand for AI inference, raw compute power, and enterprise data processing to skyrocket.  

Cheaper AI unlocks entirely new use cases and when a task becomes 90% cheaper, organizations rarely choose to keep output static; instead, they build tenfold more custom software, run far more complex simulations, and demand tighter strategic oversight. 

## Privacy and Sovereignty: Who Has Your Data?

Data sovereignty and privacy are primary drivers pushing enterprises toward local, self-hosted AI. Cloud architectures require sending proprietary data across third-party networks and trusting others with your data. Running open-weight models on-premise keeps all data strictly within internal security perimeters - eliminating third-party exposure, vendor data-training risks, and drawn-out legal reviews.

Self-hosting also guarantees operational independence. It protects workflows from cloud API outages, surprise policy updates, or sudden price hikes. As local models close the capability gap with cloud APIs, security-conscious organizations no longer have to trade intelligence for total data custody.

## AI Agents: Your Own Next Generation Assistant  
  
AI agents may be the next step on the journey. Most interactions with AI at the moment are user driven and require real-time input. The next wave maybe agents.

Agents serve as the local assistants - the middle ground between private user data and the broader internet. Operating directly on a user’s device or private server, the agent manages personal context, local files, and system access with absolute privacy. It evaluates every task, executing routine actions natively on local models with zero latency, and reserving external network calls strictly for complex, specialized requests.

This setup transforms AI companies into modular service providers rather than all-in-one platforms. Instead of housing the entire user experience in the cloud, vendors sell specialized capabilities, like frontier-level reasoning, web search, or live APIs, that local agents call on demand. The local agent functions as a smart proxy, purchasing external micro-services only when necessary while keeping core orchestration, data custody, and user state entirely self-hosted.

## The Latency Curve: You Cannot Beat The Laws Of Physics 

High-latency network round-trips to cloud servers can shatter the experience of real-time software. Standard cloud workflows require routing data through distant servers and waiting for a response, introducing jarring delays of hundreds of milliseconds to several seconds. For applications like instant voice translation, ambient assistants, and dynamic UI rendering, this lag breaks the interaction.

Moving execution directly onto local device hardware eliminates network transmission entirely. Local inference enables zero-latency voice conversations that match natural human speech cadence and instant interface adjustments, transforming AI from an asynchronous search tool into a seamless, real-time user layer.

## Conclusion

AI is changing rapidly but it looks like we are at the start of the next centralised to distributed cycle. At the moment a small number of AI companies are driving the market however there are signs of change. 

The concerns about the price of using the newest and greatest tied to the rise of "good enough" models is about to disrupt the big commercial AI companies. They are burning through cash at an incredible rate due to their compute requirements. Will they be able to find a business model where people will pay enough to use their latest AIs? 

There will still be some demand for big central models for research and industries that may rely on cutting edge technology, but a large amount of daily work, coding assistance, and personal apps will shift to local - either on device or self hosted.

## Something To Ponder

If it does move to self hosted and on device, in particular, what use cases does this open up? How will you interact with AI? 

---
Annotations: 0,8663 SHA-256 9ec9196783e9ddf55624  
@: 0,8663  
...
