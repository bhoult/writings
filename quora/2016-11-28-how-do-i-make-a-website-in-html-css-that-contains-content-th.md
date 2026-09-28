---
title: "How do I make a website in HTML/CSS that contains content that uses Markdown?"
date: "2016-11-28"
display_date: "Nov 28, 2016"
source: "quora"
tags: [programming]
---
# How do I make a website in HTML/CSS that contains content that uses Markdown?

Markdown “compiles” to HTML. So you write your markdown and it converts it to HTML that you then upload to your webserver.

There are other options such as having a Javascript library compile it on demand, or using a plugin for the CMS or your choice that will convert it before it serves it up to the browser.

I wrote a lightweight static-ish CMS that converts from markdown on the browser (client side). It is open source so you are welcome to use it if you want http://ajaxcms.org
