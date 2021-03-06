---
layout: page
title: grep
permalink: /en/grep-command/
cat: text-manipulation
order: 16
ref: grep-command
lang: en
---

## Lesson Content

The `grep` command is quite possibly the most common text processing command you will use. It allows you to search files for characters that match a certain pattern. What if you wanted to know if a file existed in a certain directory or if you wanted to see if a string was found in a file? You certainly wouldn't dig through every line of text, you would use `grep`!

Let's use our `sample.txt` file as an example: 

`$ grep fox sample.txt`

You should see that `grep` found fox in the `sample.txt` file. 

You can also `grep` patterns that are case insensitive with the `-i` flag: 

`$ grep -i somepattern somefile`

To get even more flexible with grep you can combine it with other commands with `|`.

`$ env | grep -i User`

As you can see `grep` is pretty versatile. You can even use regular expressions in your pattern: 

`$ ls /somedir | grep '.txt$'`

Should return all files ending with `.txt` in somedir.

## Exercise

You may have heard of `egrep` or `fgrep`, these are deprecated `grep` calls and have since been replaced by grep `-E` and grep `-F`. Read the `grep` manpage to learn more.

## Quiz Question

What command do you use to find a certain pattern?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
## Quiz Answer

`grep`