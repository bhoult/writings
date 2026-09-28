---
title: "Computer Vision: How can I detect text in an image? I don't want to use any OCR libraries to detect the text."
date: "2016-02-19"
display_date: "Feb 19, 2016"
source: "quora"
tags: [programming, technology, advice]
---
# Computer Vision: How can I detect text in an image? I don't want to use any OCR libraries to detect the text.

Scan the image to count the number of pixels with the exact same color. Text will likely all be a single color whereas the rest of the photo will be small variation in color even if it looks similar.

If that is not sufficient then see if most of the highest and lowest pixels of this color form horizontal lines. If so then it is likely a text overlay. 

You may also have to rule out the color if it horizontally spans more than some number of pixels to prevent picking up graphical overlays that are not text.
