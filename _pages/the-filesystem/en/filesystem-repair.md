---
layout: page
title: Filesystem Repair
category: The Filesystem
permalink: /en/filesystem-repair/
cat: the-filesystem
order: 10
ref: filesystem-repair
lang: en
---

## Lesson Content

Sometimes our filesystem isn't always in the best condition, if we have a sudden shutdown, our data can become corrupt. It's up to the system to try to get us back in a working state (although we sure can try ourselves). 

The `fsck` (filesystem check) command is used to check the consistency of a filesystem and can even try to repair it for us. Usually when you boot up a disk, `fsck` will run before your disk is mounted to make sure everything is ok. Sometimes though, your disk is so bad that you'll need to manually do this. However, be sure to do this while you are in a rescue disk or somewhere where you can access your filesystem without it being mounted.

`$ sudo fsck /dev/sda`

## Exercise

Look at the manpage for `fsck` to see what else it can do.

## Quiz Question

What command is used to check the integrity of a filesystem?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
## Quiz Answer

`fsck`
