---
layout: post
title: AOC 2020 Day 9 - Hacks on a Plane
date: 2020-12-10 02:17
author: ndileas
comments: true
categories: [code, Uncategorized]
---

I like how the [puzzles](https://adventofcode.com/2020/day/9) went from "measure the tree-tobaggan collisions" to "dupe the customs officials with a fake passport" to "connect to potentially flight critical hardware and mess with it *while in the air*". Santa is apparently instilling a wonderful black hat spirit in the great white north (pole). Maybe he's the Red Green of hackers.


{% include image.html
            img="https://natedileas.files.wordpress.com/2020/12/day9_pithy_screenshot.png"
            title="I do what?"
            caption="I do what?" %}


In other news, I did this challenge at peak coffee time, and I did pretty well at 12:15! I did this one by just throwing together script stuff, trying to see if function-izing stuff was slowing me down significantly. I think the data is inconclusive; the varying level I have with the puzzles makes it hard to tell if it's reverse causality. Also, different puzzles lend themselves to be split up into reusable chunks more or less. This one in particular was two almost entirely separate tasks, which made it a good approach.



I'm thinking of maybe making a module to encapsulate input loading; there's a lot of common tasks I do for every day's input. It would probably slow me down more than it would save for timing. But it might help for common formats later in the challenges. I'll keep mulling it over.



Here are my times so far for the challenges. Honestly, not as bad as I feared. But there's still many challenges to go. [Obligatory code link](https://github.com/natedileas/advent-of-code/blob/main/2020/day9.py).



{% include image.html
            img="https://natedileas.files.wordpress.com/2020/12/newplot_stack.png?w=1024"
            title="I don't have individual challenge timing data for the first few days, unfortunately. It probably follows the general pattern of longer time on the first puzzle, shorter on the second."
            caption="I don't have individual challenge timing data for the first few days, unfortunately. It probably follows the general pattern of longer time on the first puzzle, shorter on the second." %}

