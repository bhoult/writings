---
title: "So part one of the home-made auto focus stacking macro camera is done.  It is ab"
date: "2020-11-24"
display_date: "2020-11-24, 10:48 PM CST"
source: "facebook"
context: "timeline"
tags: [diy, technology, photography]
---
# So part one of the home-made auto focus stacking macro camera is done.  It is ab

So part one of the home-made auto focus stacking macro camera is done.  It is able to automatically take an arbitrary number of pictures while very precisely moving the camera forward fractions of a millimeter at a time.

Focus stacking allows you to get more of the picture in focus by taking multiple pictures and then combining the most in focus sections of each.  Normally with macro the depth of focus is very small.  If you look at the last pictures of the fly on a dime, there is a before (single frame) and after (50 stacked pictures).

The thing on top of the tripod is a focus rail.  You turn a knob on the end to make it move back and forth slightly.  The problem is that at this detail, touching it at all screws up the alignment.  So I attached a stepper motor to the knob with a 3d printed connector and a housing to hold the motor in place.  The stepper motor is the blue thing on the far left.

This allows for very precise and consistent movement without vibration.  

The whole thing is controlled by a tiny computer (raspberry pi).  I wrote some software to take multiple pictures while moving the camera forward a bit each time.  It can take 100 pictures at different focal points in a couple minutes.

The whole project cost about $200 in parts pi / camera / lens / motor etc.  Everything is open source.  The software used for alignment and stacking is hugin align_image_stack and hugin enfuse.

There is a bit of chromatic aberration that I need to fix and I need to refine the process some more.  But it is a good first step I think.

![](../images/facebook/e30cebe17ffb2806.jpg)

![](../images/facebook/d9953a12d26da68a.jpg)

![](../images/facebook/acc8d6be68257c54.jpg)

![](../images/facebook/ba1deac0ec15c648.jpg)

![](../images/facebook/c7e774381d6b80fc.jpg)

![](../images/facebook/e8a5ed537fc6dcd3.jpg)

![](../images/facebook/c974565e383926ee.jpg)

![](../images/facebook/3a8383e5b9ad1a36.jpg)

![](../images/facebook/53307660a9b5f466.jpg)
