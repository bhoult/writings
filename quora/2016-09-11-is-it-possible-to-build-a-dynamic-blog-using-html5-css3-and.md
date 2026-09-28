---
title: "Is it possible to build a dynamic blog using HTML5, CSS3, and JavaScript alone, or do you need some sort of CMS?"
date: "2016-09-11"
display_date: "Sep 11, 2016"
source: "quora"
tags: [programming, advice]
---
# Is it possible to build a dynamic blog using HTML5, CSS3, and JavaScript alone, or do you need some sort of CMS?

I just built one. It does all the processing / layout client side. Apache is used on the server to just serve static “content” files. The client (browser) parses the apache directory listing that is served by default if there is not an index.html in a folder.

There are a lot of advantages to this, the main ones being speed and security. But it also allows for some interesting animation effects that can continue seamlessly because there is no full page refresh as is common in most CMS systems.

You can see it in action here: AjaxCMS it is open source, so feel free to do with it as you will.
