---
layout: page
title: Power States
category: init
permalink: /en/power-states/
cat: init
order: 7
ref: power-states
lang: en
---

## Lesson Content

Hard to believe we haven't actually discussed ways to control your system state through the command line, but when talking about init, we not only talk about the modes that get us starting our system, but also the ones that stop our system.

To shutdown your system:

`$ sudo shutdown -h now`

This will halt the system (power it off), you must also specify a time when you want this to take place. You can add a time in minutes that will shutdown the system in that amount of time.

`$ sudo shutdown -h +2`

This will shutdown your system in two minutes. You can also restart with the shutdown command: 

`$ sudo shutdown -r now`

Or just use the reboot command:

`$ sudo reboot`

## Exercise

What do you think is happening with init when you shutdown your machine?

## Quiz Question

What is the command to poweroff your system in 4 minutes?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
## Quiz Answer

`sudo shutdown -h +4`