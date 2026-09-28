---
title: "I'm looking at making a basic browser game, I've started learning Ruby on Rails. Will ROR be able to create what I need?"
date: "2018-04-17"
display_date: "Apr 17, 2018"
source: "quora"
tags: [programming, games, advice]
---
# I'm looking at making a basic browser game, I've started learning Ruby on Rails. Will ROR be able to create what I need?

You can use Ruby to make a game application that you download and run like an application, although it is not as popular for this as other options. Additionally Ruby is kind of slow so if your game requires complex graphics this could become an issue.

If you want to make a “basic browser game” then JavaScript is currently the only thing that runs natively in the browser unless you go with something like a Java applet. You could use flash I suppose but that is a dying system so I would not recommend it.

If your focus is just games then you should probably look into something like unity which is specifically for making games. I believe it can actually compile to run in a browser as well.

Ruby is a great language, eventually web assembly will probably allow you to run a Ruby interpreter on the browser and then you could access the DOM with that to make a game. This is probably a few years away though and will still probably be inefficient.

If you really want to use Ruby then look into opal. It basically converts Ruby to JavaScript so it can run on the browser. Unless you are already a Ruby expert though there is not really a good reason to do it this way since the project is young and the community is small. If you have to learn the language anyway then it is best to start with the tool best suited to the job. Currently my impression is that unity or JavaScript is probably what you want.
