---
title: "How can I make a bot? I just need to get some data from a webpage which gets opened in Javascript."
date: "2016-03-11"
display_date: "Mar 11, 2016"
source: "quora"
tags: [programming, advice]
---
# How can I make a bot? I just need to get some data from a webpage which gets opened in Javascript.

I would suggest using phantom.js (headless chrome browser) along with casper.js to make it easier.

CasperJS, a navigation scripting and testing utility for PhantomJS and SlimerJS 

PhantomJS | PhantomJS 

This is pretty much the only solution I have found that will work with any site. Many sites these days pull in content or generate content with ajax calls in javascript. Because of this most traditional webscraping tools will fail since they don't run the javascript code in the html. Because Phantom.js is actually running a headless version of chrome in the background you are able to do anything a real web-browser can do.

The downside is that it is a little more complicated than some of the other solutions suggested here. It will also be slower and more resource intensive since it has to load a full browser instance. If the content you need does not depend on ajax calls then ruby/mechanize or python/scrappy (mentioned by Daksh) would probably be simpler. But Phantom.js / Casper.js will work every time.

Also, you can make a simple phantom script to wait until all the javascript runs and then dump the html to be processed with something that is easier or you are more familiar with. I use sparklemotion/nokogiri in ruby.
