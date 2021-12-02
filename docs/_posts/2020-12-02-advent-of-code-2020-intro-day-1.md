---
layout: post
title: Advent of Code 2020 - Intro + Day 1
date: 2020-12-02 02:11
author: ndileas
comments: true
categories: [code, Uncategorized]
---

<p>I'm doing <a href="https://adventofcode.com/2020">advent of code</a> again this year. For the uninitiated, AOC (not that AOC) is a set of coding puzzles, where a new puzzle is released each day of advent at midnight. They feature delightful prose, fun story, and cool puzzles. </p>



<figure class="wp-block-image size-large"><img src="https://natedileas.files.wordpress.com/2020/12/advent_of_code_2019_day4_taken_12012020.png?w=852" alt="Text: You arrive at the Venus fuel depot only to discover it's protected by a password. The Elves had written the password on a sticky note, but someone threw it out." class="wp-image-85" /><figcaption>Apparently elves are bad at computer security.</figcaption></figure>



<p>Last year I did it for the first time, and I really enjoyed it, although I didn't finish all the days. I'm going to try and finish all the challenges this year, and do a little writeup on each day's solution. Here goes something (that I probably won't finish)!</p>



<p>Here's <a href="https://adventofcode.com/2020/day/1">day 1</a>'s puzzle! Backstory: I'm on vacation on a tropical island, and christmas will have to save itself this year. I need to do various things so that I can pay for my hotel room, in stars!, a local unconvertable currency. However, apparently Santa has a large bureaucracy, and somehow I always end up doing expense reports:</p>



<figure class="wp-block-image size-large"><img src="https://natedileas.files.wordpress.com/2020/12/advent_of_code_2020_day1_taken_12012020.png?w=866" alt="Text: Before you leave, the Elves in accounting just need you to fix your expense report (your puzzle input); apparently, something isn't quite adding up." class="wp-image-83" /><figcaption>Accounting is being run by elves. I always suspected.</figcaption></figure>



<p>It was a very easy puzzle. It boiled down to, find a set of size N of numbers that sum to 2020 from the input set, then find the product of that set. Part 1 was N=2, part 2 of the challenge was N=3. Since the input list was only 200 entries, my initial solution of brute force iteration worked well. </p>



<p>Here's the code, also available on my <a href="https://github.com/natedileas/advent-of-code">github</a>. It took me almost exactly 3 minutes, 3 seconds from starting the challenge to finish.</p>



<pre class="wp-block-syntaxhighlighter-code">PS D:\code\advent\2020&gt; python
Python 3.9.0 (tags/v3.9.0:9cf6752, Oct  5 2020, 15:34:40) [MSC v.1927 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
Executable: D:\Program Files\Python39\python.exe
&gt;&gt;&gt; with open('input1-a.txt', 'r') as f:
...  lines = f.readlines()
...
&gt;&gt;&gt;
&gt;&gt;&gt; data = [int(l) for l in lines]
&gt;&gt;&gt; data
[1778, ... 1453]
&gt;&gt;&gt;
&gt;&gt;&gt; i = j = 0
&gt;&gt;&gt; for i, ii in enumerate(data):
...  for j, jj in enumerate(data):
...   if ii + jj == 2020:
...    print(i, ii, j, jj)
...
73 1472 152 548
152 548 73 1472
&gt;&gt;&gt; 1472 * 548
806656   # part 1 answer
&gt;&gt;&gt; for i, ii in enumerate(data):
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
&gt;&gt;&gt;</pre>

