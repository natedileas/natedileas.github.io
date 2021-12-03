---
layout: post
title: Advent of Code 2020 - Intro + Day 1
permalink: /aoc/2020/1/
date: 2020-12-02 02:11
author: ndileas
comments: true
categories: [code, Uncategorized]
---

I'm doing [advent of code](https://adventofcode.com/2020) again this year. For the uninitiated, AOC (not that AOC) is a set of coding puzzles, where a new puzzle is released each day of advent at midnight. They feature delightful prose, fun story, and cool puzzles. 



{% include image.html
            img="https://natedileas.files.wordpress.com/2020/12/advent_of_code_2019_day4_taken_12012020.png"
            title="Apparently elves are bad at computer security."
            caption="Apparently elves are bad at computer security." %}


Last year I did it for the first time, and I really enjoyed it, although I didn't finish all the days. I'm going to try and finish all the challenges this year, and do a little writeup on each day's solution. Here goes something (that I probably won't finish)!



Here's [day 1's](https://adventofcode.com/2020/day/1) puzzle! Backstory: I'm on vacation on a tropical island, and christmas will have to save itself this year. I need to do various things so that I can pay for my hotel room, in stars!, a local unconvertable currency. However, apparently Santa has a large bureaucracy, and somehow I always end up doing expense reports:

{% include image.html
            img="https://natedileas.files.wordpress.com/2020/12/advent_of_code_2020_day1_taken_12012020.png"
            title="Accounting is being run by elves. I always suspected."
            caption="Accounting is being run by elves. I always suspected." %}



It was a very easy puzzle. It boiled down to, find a set of size N of numbers that sum to 2020 from the input set, then find the product of that set. Part 1 was N=2, part 2 of the challenge was N=3. Since the input list was only 200 entries, my initial solution of brute force iteration worked well. 



Here's the code, also available on my [github](https://github.com/natedileas/advent-of-code). It took me almost exactly 3 minutes, 3 seconds from starting the challenge to finish.


	PS D:\code\advent\2020>; python
	Python 3.9.0 (tags/v3.9.0:9cf6752, Oct  5 2020, 15:34:40) [MSC v.1927 64 bit (AMD64)] on win32
	Type "help", "copyright", "credits" or "license" for more information.
	Executable: D:\Program Files\Python39\python.exe
	>>>  with open('input1-a.txt', 'r') as f:
	...  lines = f.readlines()
	...
	>>> 
	>>>  data = [int(l) for l in lines]
	>>>  data
	[1778, ... 1453]
	>>> 
	>>>  i = j = 0
	>>>  for i, ii in enumerate(data):
	...  for j, jj in enumerate(data):
	...   if ii + jj == 2020:
	...    print(i, ii, j, jj)
	...
	73 1472 152 548
	152 548 73 1472
	>>>  1472 * 548
	806656   # part 1 answer
	>>>  for i, ii in enumerate(data):
	...  for j, jj in enumerate(data):
	...   for k, kk in enumerate(data):
	...     if ii + jj + kk == 2020:
	...       print(ii * jj * kk)
	...
	230608320   # part 2 answer
	230608320
	230608320
	230608320
	230608320
	230608320
	>>> 


