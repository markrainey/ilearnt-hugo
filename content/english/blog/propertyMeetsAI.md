---
title: "Property meets AI"
meta_title: ""
description: "The use of AI makes property searching easier and more powerful"
date: 2026-01-14T08:03:00
categories:
  - AI
author: Mark Rainey
tags: []
draft: false
---
Imagine being able to describe the property you want to buy rather than being limited to what the site allows you to filter on.

Recently the share price of Rightmove, the main property listing site in the UK has taken a hit. This was prompted by the announcement that they are making significant investments in AI. The drop in share price seems like a very short term view of where this could be heading.

We have dreams of one day moving to near the coast. We have narrowed it down to a set of potential areas but we are a bit away from making that move.

To look at the properties in an area you can set up a whole lot of filters but it is governed by what the site has decided you might want to select. If I want to filter by something different I am not able to.

It would be nice if you could use free text to describe the property you are looking for and potentially a number of areas and then be alerted when something matches. Maybe the areas could be as vague as "2 miles from the coast" or the property "must have an open plan kitchen".  
  
I have been playing with a couple of prompts on Google Gemini that are not quite to that level yet but make the analysis of how well a property matches very quick.

This prompt provides analysis of a single property and how well it meets the requirements - obviously insert your own property link and requirements.
> Give a summary of the property details at this house and identify the pros and cons of it - https://www.rightmove.co.uk/properties/XXXXXXXXX#/?channel=RES_BUY
> 
> We are a family of four with two university age children. We are looking for a 4 bedroom detached property near the south coast. It should have at least 2 bathrooms and a decent size garden. All the bedrooms should be on the same floor. It should not be on a main road. The kitchen should be open plan and it should not require a lot of work or maintenance. It should be in a good neighbourhood.
>
> Act as an expert on property in the UK market.
>
> Create an initial summary of the property and then a list of pros and cons followed by a verdict on whether it is a good match.
>
> It should be in a friendly readable tone.

The next prompt allows for a comparison of a number of potential properties and ranks them in order of how well they meet the requirements.

> For each of the properties at the end of this prompt, place them in order of meeting the requirements below and their suitability.
>
> We are a family of four with two university age children. We are looking for a 4 bedroom detached property near the south coast. It should have at least 2 bathrooms and a decent size garden. All the bedrooms should be on the same floor. It should not be on a main road. The kitchen should be open plan and it should not require a lot of work or maintenance. It should be in a good neighbourhood.
> 
> Act as an expert on property in the UK market.
> 
> For each property in the list also add a reason for why it is a good match and it's biggest weakness.
> 
> It should be in a friendly readable tone.
>  
> https://www.rightmove.co.uk/properties/XXXXXXXXX#/?channel=RES_BUY
> 
> https://www.rightmove.co.uk/properties/YYYYYYYYY#/?channel=RES_BUY
> 
> https://www.rightmove.co.uk/properties/ZZZZZZZZZ#/?channel=RES_BUY

I've not used it properly yet as we are not looking to move but it is a really nice starting point and I am sure there is a lot of tweaking that could be done.

If Rightmove is heading in this direction with their AI work then this could be a real game changer for users.