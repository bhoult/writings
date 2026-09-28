---
title: "If sequel performs better in Sinatra, is it wise to use sequel (instead of ActiveRecord) in Rails5?"
date: "2016-03-11"
display_date: "Mar 11, 2016"
source: "quora"
tags: [programming, advice]
---
# If sequel performs better in Sinatra, is it wise to use sequel (instead of ActiveRecord) in Rails5?

In most cases database queries are not going to be your performance problem. If you use active record correctly (using includes, pluck etc.) it is pretty easy to optimize most queries, especially with lazy evaluation and caching that is included.

In rare cases it may be worth the effort to hand craft the sql, but this would only be for the pieces that get heavy use.

I did find once that doing a lot of inserts was slow with active record. Probably because of all the callbacks and validations, but even with these disabled it was taking several minutes to process a spreadsheet and then do several thousand inserts into the database. We managed to reduce that to a couple seconds by dumping sql statements to a text file and then piping that directly into mysql.
