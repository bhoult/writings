---
title: "Is it a good idea to convert large excel file to JSON object for mass upload in database?"
date: "2016-09-05"
display_date: "Sep 05, 2016"
source: "quora"
tags: [programming]
---
# Is it a good idea to convert large excel file to JSON object for mass upload in database?

As others have mentioned it will depend entirely on the database implementation you want to use. A story though:

I once had to upload a bunch of excel sheets into a mysql database from a rails application. One excel sheet produced about 10,000 database records and doing that with Active Record took about 8 minutes.

By disabling all the callbacks and validation in rails we got it down to about 2 minutes.

Mysql has a dump utility that basically exports the database as a series of inserts in a big text file. We noticed that restoring a backup by piping this dump into the command line mysql client was pretty quick.

So we converted the spreadsheet to a bunch of insert statements in a text file and then piped that into the command line mysql client. Turns out this took 2–3 seconds total.

So from 8 minutes to two seconds.
