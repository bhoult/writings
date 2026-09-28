---
title: "How can Linux be so much faster, stable, safer, and reliable than Windows even though it’s free? Why doesn't Microsoft do the same with Windows?"
date: "2017-02-23"
display_date: "Feb 23, 2017"
source: "quora"
tags: [technology]
---
# How can Linux be so much faster, stable, safer, and reliable than Windows even though it’s free? Why doesn't Microsoft do the same with Windows?

Two primary reasons.

First, backwards compatibility. Newer versions of Windows have to maintain reasonable compatibility with older Windows software. If this breaks then Microsoft programmers have to fix it which is expensive. This requires that Microsoft maintain, and support multiple versions of old APIs and drivers along with including them in newer versions of Windows even if they are rarely used.

Let's say you have an old version of Photoshop that you bought 10 years ago and you do not want to buy the new version because the old one works just fine. If you upgrade windows and it breaks then you would be upset with Microsoft. Fixing it means you have to buy a new version of Photoshop.

Compare this with open source. Because they have access to the source code of the applications as well as the OS they can update all the apps to use the latest versions of whatever device drivers or APIs are used. So if you are using an old version of GIMP and you update Ubuntu then Ubuntu will have tested and updated GIMP as well and it does not cost anything so people generally don't mind updating. Every 6 months Ubuntu does exactly this, they release a new version where everything in their repository is tested and fixed to be up to date. There is no reason to maintain compatibility with 10 year old APIs. So it is smaller, lighter and presumably more secure without old vulnerabilities still sitting around.

This lets open source essentially “evolve” faster. There is a barrier between windows application developers and OS developers at Microsoft that requires support contracts, time, money and politics to overcome. Maintaining backwards compatibility becomes more of a burden as an application gets older, grows in complexity, or gains a larger user base. Open source does not have to deal with this because anyone can get access to the full source code make changes as needed without having to ask permission.

The second reason is one of priorities. Microsoft sells new versions of Windows with new computers. It is in their best interest that people periodically buy new computers for this reason. Computer companies install windows by default for this same reason. It is in their best interest of Windows gets slow and unreliable every few years, so you will buy a new computer.

The people that program Linux and its associated software did it primarily to solve a problem they had. In most cases functionality was not a secondary objective after profitability. They don't benefit from your computer becoming disfunctional over time. Closed source operating systems are basically the same model as “pay to play”.
