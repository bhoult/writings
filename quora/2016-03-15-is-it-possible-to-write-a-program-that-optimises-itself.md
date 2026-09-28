---
title: "Is it possible to write a program that Optimises itself?"
date: "2016-03-15"
display_date: "Mar 15, 2016"
source: "quora"
tags: [programming, technology]
---
# Is it possible to write a program that Optimises itself?

To some extent yes, I believe this is part of the reason that javascript has become so fast in recent years. It optimizes things like regular expressions as they are run, to the extent that it in many cases becomes faster than writing it in a language like C.

I was reminiscing a couple days ago about an old project where I had to maintain, debug, expand an old (really old) and very large perl program that was terribly written. It was a monstrosity cobbled together by a huge number of people with varying degrees of experience. In once case there was an array with a few thousand elements that needed to be sorted. The programmer apparently did not know that there was a native sort in perl, but he knew that he could dump the data in sorted form from the database. His solution was to create a table in the database, insert all the data into it, query it back in sorted form then drop the database. This is just one of many seemingly insane things that were part of this system.

Anyway, there is some speculation these days that AI might make programmers obsolete in much the same way that it is about to do with truck drivers. I personally doubt this in the near term because programming is really nothing more than describing a problem and its solution in exact and specific terms. As programming languages and frameworks progress, they are in a practical sense just refining reasonable assumptions about various recurring problems and then optimizing for that case in the form of a language construct or a library. These are rapidly evolving and eventually become what we consider "best practice". Because of this you will still have to describe the same problem and its solution to an AI. Syntax may become more flexible and the process may become more of a conversation but the mentality of programming will be largely the same.

So... back to my horrendous pile of perl. It seem (to me) that what may happen next it basically program re-writers or optimizers. My perl mess, while bordering on indecipherable, had been poked at long enough that it was actually pretty stable. In its present state it describes perfectly but non-optimally the problems to be solved and their solutions. It should be possible (not that I am capable of doing so), to analyze the source code and it's execution to determine given all possible inputs what is required to produce it's output. Then write the code necessary to optimally accomplish it by matching it to a known "best practice". This makes it a task approaching something similar to what googles deep-mind recently accomplished in beating the go champion.

So in my perl code it would see that a given chunk of code merely produces a sorted list of it's input. It would strip out that code and replace it with the best sort for that dataset. There was also a huge mass of code that was likely never actually run. It would recognize that and remove it resulting in an increase in readability. ... and so on.

I, for one, welcome our future code-optimizing overlords.
