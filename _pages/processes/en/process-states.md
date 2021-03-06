---
layout: page
title: Process States
permalink: /en/process-states/
cat: processes
order: 9
ref: process-states
lang: en
---

## Lesson Content

Let's take a look at the `ps aux` command again:

`$ ps aux`

In the `STAT` column, you'll see lots of values. A linux process can be in a number of different states. The most common state codes you'll see are described below:

* `R`: running or runnable, it is just waiting for the CPU to process it
* `S`: Interruptible sleep, waiting for an event to complete, such as input from the terminal
* `D`: Uninterruptible sleep, processes that cannot be killed or interrupted with a signal, usually to make them go away you have to reboot or fix the issue
* `Z`: Zombie, we discussed in a previous lesson that zombies are terminated processes that are waiting to have their statuses collected
* `T`: Stopped, a process that has been suspended/stopped

## Exercise

Take a look at the running processes on your system and check out their process states.

## Quiz Question

What `STAT` code is used to represent an uninterruptible sleep?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />  
## Quiz Answer

`D`