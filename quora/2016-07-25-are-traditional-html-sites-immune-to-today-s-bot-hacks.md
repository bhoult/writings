---
title: "Are traditional HTML sites immune to today's bot hacks?"
date: "2016-07-25"
display_date: "Jul 25, 2016"
source: "quora"
tags: [technology, programming]
---
# Are traditional HTML sites immune to today's bot hacks?

By traditional html I assume you mean static sites without a database or any server side code.

If that is the case then they are less vulnerable but not entirely immune. There are multiple ways a site can be hacked. If the hacker is targeting a vulnerability in the code of something like a CMS or is attacking the database with something like SQL injection then static html would not have these vulnerabilities.

They can still compromise the site though if they get access to the password of the host account or server, or through SSH or ftp access. Basically if they can write to the server filesystem then you are "hacked".

Also static sites will be less vulnerable to a denial of service attack since they have lower overhead, but they could still be overwhelmed if the attacker has sufficient bandwidth.
