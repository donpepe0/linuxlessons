---
layout: page
title: Process Details
permalink: /en/process-details/
cat: processes
order: 3
ref: process-details
lang: en
---

## Lesson Content

Before we get into more practical applications of processes, we have to first understand what they are and how they work. This part can get confusing since we are diving into the nitty gritty, so feel free to come back to this lesson if you don't want to learn about it now. 

A process like we said before is a running program on the system, more precisely it's the system allocating memory, CPU, I/O to make the program run. A process is an instance of a running program, go ahead and open 3 terminal windows, in two windows, run the `cat` command without passing any options (the `cat` process will stay open as a process because it expects stdin). Now in the third window run: `ps aux | grep cat`. You'll see that there are two processes for `cat`, even though they are calling the same program.

The kernel is in charge of processes, when we run a program the kernel loads up the code of the program in memory, determines and allocates resources and then keeps tabs on each process, it knows: 

* The status of the process
* The resources the process is using and receives
* The process owner
* Signal handling (more on that later)
* And basically everything else

All processes are trying to get a taste of that sweet resource pie, it's the kernel's job to make sure that processes get the right amount of resources depending on process demands. When a process ends, the resources it used are now freed up for other processes.

## Exercise

No exercises for this lesson.

## Quiz Question

What manages and controls processes?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /> 
## Quiz Answer

kernel