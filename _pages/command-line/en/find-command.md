---
layout: page
title: find
permalink: /en/find-command/
cat: command-line
order: 14
ref: find-command/
lang: en
---

## Lesson Content

With all these files we have on the system it can get a little hectic trying to find a specific one. Well there’s a command we can use for that, `find`! 

`$ find /home -name puppies.jpg`

With `find` you’ll have to specify the directory you’ll be searching it, what you’re searching for, in this case we are trying to find a file by the name of puppies.jpg. 

You can specify what type of file you are trying to find. 

`$ find /home -type d -name MyFolder`

You can see that I set the type of file I’m trying to find as `d` for directory and I’m still searching by the name of MyFolder. 

One cool thing to note is that find doesn’t stop at the directory you are searching, it will look inside any subdirectories that directory may have as well.

## Exercise

1. Find a file from the root directory that has the word net in it.


## Quiz Question

What option should I specify for find if I want to search by name?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />

## Quiz Answer

`-name`
