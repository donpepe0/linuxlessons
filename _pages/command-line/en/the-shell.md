---
layout: page
title: The Shell
category: Command Line
permalink: /en/the-shell/
cat: command-line
order: 1
ref: the-shell
lang: en
---

## Lesson Content

The world is your oyster, or really the shell is your oyster. What is the shell? The shell is basically a program that takes your commands from the keyboard and sends them to the operating system to perform. If you’ve ever used a GUI, you’ve probably seen programs such as “Terminal” or “Console” these are just programs that launch a shell for you. Throughout this entire course we will be learning about the wonders of the shell. 

In this course we will use the shell program bash (Bourne Again shell), almost all Linux distributions will default to the bash shell. There are other shells available such as ksh, zsh, tsch, but we won’t get into any of those. 

Let’s jump right in! Depending on the distribution your shell prompt might change, but for the most part it should adhere to the following format:
```
username@hostname:current_directory  
pete@icebox:/home/pete $
```

Notice the `$` at the end of the prompt? Different shells will have different prompts, in our case the `$` is for a normal user using Bash, Bourne or Korn shell, you don't add the prompt symbol when you type the command, just know that it's there.

Let’s start with a simple command, `echo`. The `echo` command just prints out the text arguments to the display.

`$ echo Hello World`

## Exercise

Try some other Linux commands and see what they output:

1. `$ date`
2. `$ whoami`

## Quiz Question

What should be outputted to the display when you type `echo Hello World`?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
## Quiz Answer

Hello World
