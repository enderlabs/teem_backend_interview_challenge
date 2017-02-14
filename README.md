# Teem Backend Interview Challenge
## Instructions
Clone and submit your answers to the following questions with your Teem backend programmer application

The following problems are reviewed for

 * runability,
 ** we should be able to run your code with minimal effort,
 ** you should probably provide a readme,
 * completeness (does it answer the given question),
 * readability,
 ** this includes comments,
 ** and PEP8 considerations,
 * edge cases covered.

Solutions must be written in Python, use any version of Python higher than 2.7. These solutions should be written in a way that we could import and use them in other modules as well as being able to run them from the command line.

## Problem 1:
Write an efficient function `has_palindrome` that checks whether any permutation of an input string is a palindrome.

Examples:
`has_palindrome('civic')` should return `True`
`has_palindrome('ivicc')` should return `True`
`has_palindrome('civil')` should return `False`
Note, there is an O(n) solution to this problem.

## Problem 2:
At Teem we handle a lot of calendar data and we often want to find the available times for a group of people.

For this exercise a meeting is stored as a tuple of integers (start_time, end_time) where the integers represent the number of 30 minute blocks past 12am.

For example
```
(20, 22)  # a meeting from 10 am -- 11 am
(21, 22)  # a meeting from 10:30 am -- 11 am
```

Write a function called condense_meeting_times() that takes a list of meeting time ranges and returns a list of condensed ranges. For example,given [(20, 22), (21, 22), (25, 30)] it will output [(20,22), (25,30)]

Do not assume the meetings are in order. The meeting times are coming from multiple teams.

### Bonuses:
 - write the same function but assume the (start_time, end_time) are Unix timestamps.
 - write the same function but assume the (start_time, end_time) are ISO-8601 datetime strings.
