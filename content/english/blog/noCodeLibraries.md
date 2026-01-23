---
title: "The code-free future ... maybe"
meta_title: ""
description: "A thought exercise on a library built from rules and tests and not code"
date: 2026-01-23T13:39:00
categories:
  - Technology
  - AI
author: Mark Rainey
tags: []
draft: false
---
What if code libraries in future contained no code?

In this [article](https://www.dbreunig.com/2026/01/08/a-software-library-with-no-code.html) it discusses a potential future where software libraries no longer contain code but consist of rules/specifications and tests. 

> What does software engineering look like when coding is free?

The example given is a simple set of functionality around timestamps. The claim is that by clearly defining a specification and a set of tests that should pass, the user of the library can use AI to generate their own implementation in their own language and coding style. As long as the tests pass they can, potentially, be confident that the code will work as expected.

At first glance this seems very powerful and, as a developer, I find the idea of a specification only library both liberating and terrifying. 

As the article rightly points out, there are some serious issues with this as it stands. 

With the current AI approach there are sufficient problems to make this an interesting thought exercise rather than something that is currently practical.

It will take significant effort for anything more than a simple function to define the functionality required and all the tests that need to pass. This will need to include both the "happy" and the "sad" path tests. It may also need to define more complex test scenarios around parallel execution for example.

Due to the way LLMs currently work they are non-deterministic. Two runs against the same rules and tests could, and are likely to, produce different code. Could regenerating the code introduce new issues?

How do you fix a bug and support it? 

> Replicating bugs is nearly impossible. If the customer gets stuck on an issue with their own generated codebase, how do we have a hope of finding the problem?

You could update the spec to cope with the error and then get the consumers to rerun it to generate new code with the fix in it. However, how do you know this will work across all the consumers - and across all the different languages?

Similarly, how do you handle updates to the library? How do you ensure all consumers generate new code to fix a security issue for example?

Does the specification work for languages with different programming paradigms? Does it generate code that is performant enough? How do you update an API/interface?

Despite being a potentially powerful and clever approach there are a LOT of hurdles to overcome before anything close to this is possible.

Then again, the speed AI is progressing I may be proven wrong very soon.
