---
title: "When your WPF menu alignment is wrong"
meta_title: ""
date: 2020-07-07T12:00:00
author: "Mark Rainey"
categories: ["coding"]
tags: []
draft: false
---
I had a very weird problem where my menus on a WPF application were dropping down to the left instead of the normal to the right.

It turns out it is due to having a tablet setting set to right handed ... even though I don't have a tablet. The answer was found on the link at the bottom of this post.

To fix it:

Press the **Windows key + R** and then copy/paste the following line of text.

shell:::{80F3F1D5-FECA-45F3-BC32-752C152E456E}

Press OK.

In the Tablet PC Settings configuration dialog select the "Other" Tab. In the Handedness section, place a check mark in the Left Handed option.

Click OK.

Fixed.



__Links__

[How can I get WPF menus to align like the old win forms menu?](https://stackoverflow.com/questions/11237378/how-can-i-get-wpf-menus-to-align-like-the-old-win-forms-menu)

