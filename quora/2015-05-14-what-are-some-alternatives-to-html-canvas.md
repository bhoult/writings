---
title: "What are some alternatives to HTML Canvas?"
date: "2015-05-14"
display_date: "May 14, 2015"
source: "quora"
tags: [programming, technology]
---
# What are some alternatives to HTML Canvas?

Your options at this point are the following:
1. Canvas (bitmaps)
2. SVG (vectors)
3. WebGL (3d)

Each has advantages and disadvantages and a number of libraries to help you use them. In general the properties of each are as follows:
Canvas - Fast, Flexible, Well Supported, slightly harder to animate but libraries make this a non-issue.
SVG - Easy to animate but slow. Reasonable browser support.
WebGL - Fast if hardware accelerated with a good video card. Browser support is not that great, but works with the latest version of major browsers. Check out three.js. Also lines wider than 1 pixel are problematic in WebGL for some crazy reason. I had to make my own out of polygons.
