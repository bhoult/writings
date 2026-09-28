---
title: "What are the best programming practices that are easy to follow, but make a significance in RAM usage?"
date: "2015-05-27"
display_date: "May 27, 2015"
source: "quora"
tags: [programming, advice]
---
# What are the best programming practices that are easy to follow, but make a significance in RAM usage?

That is a pretty generic question... depends a lot on the language and application. In general I would just say release the memory you use as soon as you are done with it. If you have to keep a large chunk around that is infrequently used then write it to disk and fetch it when you need it. Try to use the database for as much as you can, and return just what you need in the state closest to what you are going to want (pre-sorted, filtered, grouped, etc). 

A lot of times there is a trade off between readability, maintainability and memory usage, for example storing an array of objects may require more memory than an array of just the variables you need. 

Use the smallest variable type necessary for whatever you are keeping track of. Group booleans in to a byte, use enumerations, variable length strings instead of fixed width which are faster. Your chosen language may do some of this automatically, or you may have to manually specify everything.

Keep things DRY (Don't repeat yourself). Review your code periodically to see if you can get it smaller. If you can get some peer-review that can be helpful. You can learn a lot from the way other people do stuff that may not be apparent from a single perspective.
