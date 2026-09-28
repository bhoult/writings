---
title: "Have you ever seen a virus on Ubuntu?"
date: "2016-09-16"
display_date: "Sep 16, 2016"
source: "quora"
tags: [technology, story]
---
# Have you ever seen a virus on Ubuntu?

I have seen a bunch of them in the last year or so. Although I am not sure if they would fit your definition of virus. Basically it is malware that gets installed in wordpress or other php based content management systems that cross contaminates to other sites under the same user account.

For example, I have a client that had eight wordpress sites installed in his account on a shared host. At some point one of them was compromised probably as a result of an insecure plugin. They installed a php file that let them execute arbitrary commands. Because all the other sites were running with the same user permissions, this script was copied to all the rest a few hundred times with different filenames.

Eventually there were a few dozen piece of malware happily replicating all over the place. They were performing ddos attacks and sending spam non stop. The host blocked the site until it was fixed.

So I got onto the main site and manually cleaned everything and updated WordPress and plugins. This took about 6 hours. It was reenabled and was reinfected within a day.

We eventually moved everything to an amazon vm, ran a version of apache that allows each site to run under a different user. Once they were isolated from each other we were able to disinfect each one. I versioned each using git so we could easily tell when files changed and could roll back to a clean state if they had.

Basically malware can roam freely on Linux so long as it stays in the confines of a single user. Anything that user has write access to is fair game. Hopefully that user is not root. And hopefully they cannot read your systems password file.
