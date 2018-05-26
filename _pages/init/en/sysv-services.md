---
layout: page
title: System V Services
category: init
permalink: /en/sysv-services/
cat: init
order: 2
ref: sysv-services
lang: en
---

## Lesson Content

There are many command line tools you can use to manage Sys V services. 

**List services**

`$ service --status-all`

**Start a service**

`$ sudo service networking start`

**Stop a service**

`$ sudo service networking stop`

**Restart a service**

`$ sudo service networking restart`

These commands aren't specific to Sys V init systems, you can use these commands to manage Upstart services as well. Since Linux is trying to move away from the more traditional Sys V init scripts, there are still things in place to help that transition. 

## Exercise

Manage a couple of services and change their states, what do you observe?

## Quiz Question

What is the command to stop a service named peanut with Sys V?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
## Quiz Answer

`sudo service peanut stop`