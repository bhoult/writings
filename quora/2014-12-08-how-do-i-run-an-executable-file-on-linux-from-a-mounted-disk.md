---
title: "How do I run an executable file on Linux from a mounted disk?"
date: "2014-12-08"
display_date: "Dec 08, 2014"
source: "quora"
tags: [technology, advice]
---
# How do I run an executable file on Linux from a mounted disk?

This is just kind of a shot in the dark... but it sounds like you are trying to run a windows program on a linux OS. /dev/sdb is how linux or other unix based OS references drives. .exe is a file extension windows uses to denote an executable file. Linux cannot directly run a windows binary, linux also uses the filesystem permissions instead of the file extension to determine if a file is executable (ie. "chmod +x filename" will make filename executable if you then type ./filename from the directory it is in).

If you need to run a windows .exe in linux then check out the wine project.
