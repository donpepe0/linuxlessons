---
layout: page
title: stdin
permalink: /en/stdin/
cat: text-manipulation
order: 2
ref: stdin
lang: en
---

## Lesson Content

In our previous lesson we learned that we have different stdout streams we can use, such as a file or the screen. Well there are also different standard input `stdin` streams we can use as well. We know that we have `stdin` from devices like the keyboard, but we can use files, output from other processes and the terminal as well, let's see an example. 

Let's use the peanuts.txt file in the previous lesson for this example, remember it had the text Hello World in it. 

`$ cat < peanuts.txt > banana.txt `

Just like we had `<` for stdout redirection, we can use `>` for stdin redirection. 

Normally in the `cat` command, you send a file to it and that file becomes the `stdin`, in this case, we redirected peanuts.txt to be our `stdin`. Then the output of cat peanuts.txt which would be Hello World gets redirected to another file called banana.txt.

## Exercise

Try out a couple of commands:
```
$ echo < peanuts.txt > banana.txt
$ ls < peanuts.txt > banana.txt
$ pwd < peanuts.txt > banana.txt
```

## Quiz Question

What redirector do you use to redirect `stdin`?

## Quiz Answer

`<`