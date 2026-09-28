---
title: "Do web developers prefer to work from templates or code from scratch?"
date: "2016-03-03"
display_date: "Mar 03, 2016"
source: "quora"
tags: [programming, advice]
---
# Do web developers prefer to work from templates or code from scratch?

I used to get a template that was most similar to what I wanted and would then override what was needed until it was close to what I wanted. These templates were usually very large so overriding all the css could be a lot of work. In looking through them I found that they were usually far more complex than they needed to be. I expect they were the result of many iterations of what I was doing, just layering on more CSS on top of other layers of CSS.

There is kind of a reason for this, in theory templates are versioned and you should be able to replace the underlying template with a new version so long as you have added a CSS file on top rather than editing them directly. If you edited the actual template then you would have to track down all your changes and reproduce them. In practice I doubt many people ever bother to upgrade the underlying template though. Also, many of them are built to be flexible, variable number of columns, custom javascript, admin interfaces, stuff like that. These are not really intended for editing directly and include a lot of code that may never be used.

Eventually I started making templates from scratch... Well I normally use a CSS library like bootstrap but I build from scratch on top of that. The result is literally 100 times smaller in most cases, much easier to work with and debug. I have used very few pre-made templates in the past several years. Generally just when a client already has a template that they want to use.
