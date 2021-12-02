---
layout: post
title: AOC 2020 Day 9 - Hacks on a Plane
date: 2020-12-10 02:17
author: ndileas
comments: true
categories: [code, Uncategorized]
---

<p>I like how the <a href="https://adventofcode.com/2020/day/9">puzzles </a>went from "measure the tree-tobaggan collisions" to "dupe the customs officials with a fake passport" to "connect to potentially flight critical hardware and mess with it <em>while in the air</em>". Santa is apparently instilling a wonderful black hat spirit in the great white north (pole). Maybe he's the Red Green of hackers.</p>



<figure class="wp-block-image size-large"><img src="https://natedileas.files.wordpress.com/2020/12/day9_pithy_screenshot.png?w=1024" alt="Screenshot of the puzzle text. It reads &quot;With your neighbor happily enjoying their video game, you turn your attention to an open data port on the little screen in the seat in front of you.

Though the port is non-standard, you manage to connect it to your computer through the clever use of several paperclips. Upon connection, the port outputs a series of numbers (your puzzle input).

The data appears to be encrypted with the eXchange-Masking Addition System (XMAS) which, conveniently for you, is an old cypher with an important weakness.&quot;" class="wp-image-157" /><figcaption>I do what?</figcaption></figure>



<p>In other news, I did this challenge at peak coffee time, and I did pretty well at 12:15! I did this one by just throwing together script stuff, trying to see if function-izing stuff was slowing me down significantly. I think the data is inconclusive; the varying level I have with the puzzles makes it hard to tell if it's reverse causality. Also, different puzzles lend themselves to be split up into reusable chunks more or less. This one in particular was two almost entirely separate tasks, which made it a good approach.</p>



<p>I'm thinking of maybe making a module to encapsulate input loading; there's a lot of common tasks I do for every day's input. It would probably slow me down more than it would save for timing. But it might help for common formats later in the challenges. I'll keep mulling it over.</p>



<p>Here are my times so far for the challenges. Honestly, not as bad as I feared. But there's still many challenges to go. <a href="https://github.com/natedileas/advent-of-code/blob/main/2020/day9.py">Obligatory code link</a>.</p>



<figure class="wp-block-image size-large"><img src="https://natedileas.files.wordpress.com/2020/12/newplot_stack.png?w=1024" alt="" class="wp-image-161" /><figcaption>I don't have individual challenge timing data for the first few days, unfortunately. <br>It probably follows the general pattern of longer time on the first puzzle, shorter on the second.</figcaption></figure>

