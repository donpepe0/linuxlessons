---
layout: page
title: Kernel Logging 
permalink: /en/kernel-logging/
cat: logging
order: 4
ref: kernel-logging
lang: en
---

## Lesson Content

`/var/log/dmesg`  
On boot-time your system logs information about the kernel ring buffer. This shows us information about hardware drivers, kernel information and status during bootup and more. This log file can be found at `/var/log/dmesg` and gets reset on every boot, you may not actually see any use in it now, but if you were to ever have issues with something during bootup or a hardware issue, dmesg is the best place to look. You can also view this log using the dmesg command. 

`/var/log/kern.log`  
Another log you can use to view kernel information is the `/var/log/kern.log` file, this logs the kernel information and events on your system, it also logs dmesg output.

## Exercise

Look at your dmesg and kern logs, what differences do you notice?

## Quiz Question

What command can be used to view kernel bootup messages?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /> 
## Quiz Answer

`dmesg`