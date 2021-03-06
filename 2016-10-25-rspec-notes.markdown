---
title: Rspec Notes
categories: ruby rspec
---

Notes about **rspec** which I find interesting.

## How to run

Assuming you are using **bundler**, otherwise just ignore `bundle exec` and call `rspec` directly

```
$ bundle exec rspec <rspec_file>
$ bundle exec rspec <rspec_file>:<line_number>
```

## Describe and Context

Difference between `describe` and `context` ? There's no functional difference, they are interchangeable

But usually context is used to describe the condition, e.g. not full date selected

## Rspec as documentation

Test cases can be used as documentations for the application/project you are working for.
In **rspec**, you can run below command to list the tests as documentation.

```
$ bundle exec rspec -fd <filename>

Club::MatchHistory
  #match_history
    should return an empty array if there are no matches for the club
    should return all matches for the current season
    should not return a future match
```