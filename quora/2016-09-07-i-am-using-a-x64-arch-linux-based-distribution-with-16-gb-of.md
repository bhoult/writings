---
title: "I am using a x64 Arch Linux based distribution, with 16 GB of RAM and a 4th generation i7. Why is my system slow and unresponsive?"
date: "2016-09-07"
display_date: "Sep 07, 2016"
source: "quora"
tags: [technology, advice]
---
# I am using a x64 Arch Linux based distribution, with 16 GB of RAM and a 4th generation i7. Why is my system slow and unresponsive?

If the window manager is expecting a working 3d card in order to accelerate visual effects then it likely is currently falling back to simulating a GPU using the CPU. This will cause CPU to spike whenever you move windows around.

Solutions are to fix your Nvidia drivers or use a window manager that does not require 3d like xfce or similar.
