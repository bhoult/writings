---
title: "What is the recommended way of installing Rails on a fresh copy of Ubuntu 16.04 in 2016?"
date: "2016-11-17"
display_date: "Nov 17, 2016"
source: "quora"
tags: [programming, technology]
---
# What is the recommended way of installing Rails on a fresh copy of Ubuntu 16.04 in 2016?

Not sure what is recommended, but Ubuntu generally packages very old versions of ruby. The newest rails usually needs a fairly recent ruby. So I always use RVM to install the latest ruby then just “gem install rails”. Takes a lot longer to compile everything, but it all works well after that.
