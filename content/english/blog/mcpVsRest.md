---
title: "MCP and REST face-off"
meta_title: ""
description: "The differences between REST and MCP"
date: 2026-02-16T10:12:00
categories:
  - AI
author: Mark Rainey
tags: []
draft: false
---
At the recent MCPConference in London, one of the members of a panel made the statement "MCP is not just an API wrapper". This got me thinking what are the main differences.

For over a decade, REST has been the undisputed API backbone of the internet. It was designed for a world where humans interacted with machines through rigid interfaces: you click a button, a specific request is sent, and a structured response returns. However, as we move into the era of AI agents, the "fixed-route" nature of REST is beginning to show its age. Enter the Model Context Protocol (MCP), a new standard designed to give AI models a more intuitive way to interact with the digital world.

REST APIs are built for developers who write static code to fetch specific data. In contrast, MCP is built for Large Language Models (LLMs) that need to explore and use tools dynamically. While a REST endpoint is like a single vending machine button that gives you one specific snack, an MCP server is more like a helpful clerk who hands the AI a catalog of everything they can do and asks, "How can I help you accomplish your goal today?".

One of the most significant technical shifts in MCP is self-discovery. 

In the REST world, if you want an AI to use an API, you usually have to feed it pages of documentation or a massive schema. With MCP, the server is "self-describing". When an AI connects, the server automatically provides a list of available tools and resources. This allows an AI agent to instantly understand how to query a database or read a local file without a human having to write "glue code" for every new integration.

This approach potentially makes integration easier however it also means that there is less control over when or if the endpoint is called.

One of the most interesting aspects of the shift from REST to MCP is how the data lifecycle changes from a rigid transaction to a dynamic conversation. 

In the REST world, every interaction is synchronous and follows a very strict script; the client asks for specific data, the server provides it, and the connection is closed. If the client realizes it needs more information, it has to start a brand new cycle from scratch. MCP flips this on its head by allowing for an asynchronous flow where the server isn't just a passive responder. Because the server is "self-describing," it can actively participate in the task by suggesting additional tools or requesting more context from the AI model to fulfil a complex goal. This means that instead of a series of isolated "gets" and "posts," you have a continuous loop where the protocol can pause and ask for more data to ensure the final output is actually useful.

Furthermore, the transport layer of these protocols reflects their different environments. REST is almost exclusively tied to HTTP, making it perfect for the open web. MCP, however, is designed to work just as well over standard input/output. This makes it incredibly powerful for local development; it allows an AI coding assistant running on your laptop to securely talk to your local file system or a private development database without the overhead or security risks of exposing those services to the public internet.

Ultimately, the move toward MCP represents a shift from integration to interaction. Instead of developers spending hours mapping API endpoints to specific functions, they can now build "toolsets" that any MCP-compatible AI can pick up and use. This standardization is what will transform AI from a chatbot that just talks into an agent that can actually "do," whether that is debugging your code, managing your calendar, or analysing local datasets.
