---
title: "What are better alternatives for PHP and MySQL?"
date: "2015-04-10"
display_date: "Apr 10, 2015"
source: "quora"
tags: [programming, advice]
---
# What are better alternatives for PHP and MySQL?

PHP and MySql are probably enough. If you have pretty basic needs and are a single developer and are not overly worried about maintaining and expanding the app for several years then PHP is fine for just getting something small accomplished.

The problem with PHP is that it does not encourage well designed software. You can pretty much do it however you want and that can be fun until you have to maintain or contribute to someone else's undocumented and poorly designed code. If you are just starting then you will probably rely on function calls and global variables instead of objects which will make your programs tend toward "spaghetti code". The more complex it becomes the harder it is to maintain or improve on. Eventually if it gets too complex you will start avoiding working on it out of fear that something will inadvertently break.

Frameworks were created to combat this tendency. They usually figure out the best way to do something and then try to encourage you to do it that way. So you have Rails (ruby) and Django (python) among many others. If you work according to the standards of the framework then someone else familiar with the framework can generally have a good idea of how your code works without spending a lot of time studying whatever way you decided to do it. If you have proper testing and isolation then you can be confident that adding or changing something will not unexpectedly break something else.

It is pretty much as easy to develop and maintain a small program inside a framework as it is to just make it from scratch. However it is much harder to grow or maintain a program without a framework. For this reason if you are looking for something to learn you might as well go with a framework and learn good habits from the beginning. 

People generally learn from making mistakes, through this they try to come up with ways to avoid those mistakes in the future. The things they learn are consolidated in these frameworks to prevent future problems. If at all possible try to learn from other peoples mistakes so you don't have to make them again on your own.
