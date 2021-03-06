---
layout: page
title: stderr
permalink: /en/stderr/
cat: text-manipulation
order: 3
ref: stderr
lang: en
---

## Lesson Content

Let's try something a little different now, let's try to list the contents of a directory that doesn't exist on your system and redirect the output to the peanuts.txt file again.

`$ ls /fake/directory > peanuts.txt `

What you should see is: 

`ls: cannot access /fake/directory: No such file or directory`

Now you're probably thinking, shouldn't that message have been sent to the file? There is actually another I/O stream in play here called standard error `stderr`. By default, `stderr` sends its output to the screen as well, it's a completely different stream than stdout. So you'll need to redirect its output a different way. 

Unfortunately the redirector is not as nice as using `<` or `>` but it's pretty close. We will have to use file descriptors. A file descriptor is a non-negative number that is used to access a file or stream. We will go in depth about this later, but for now know that the file descriptor for `stdin`, `stdout` and `stderr` is `0`, `1`, and `2` respectively. 

So now if we want to redirect our `stderr` to the file we can do this: 

`$ ls /fake/directory 2> peanuts.txt`

You should see just the `stderr` messages in peanuts.txt. 

Now what if I wanted to see both `stderr` and `stdout` in the peanuts.txt file? It's possible to do this with file descriptors as well: 

`$ ls /fake/directory > peanuts.txt 2>&1`

This sends the results of `ls /fake/directory` to the peanuts.txt file and then it redirects `stderr` to the `stdou` via `2>&1`. The order of operations here matters, `2>&1` sends stderr` to whatever `stdout` is pointing to. In this case `stdout` is pointing to a file, so `2>&1` also sends `stderr` to a file. So if you open up that peanuts.txt file you should see both `stderr` and `tdout`. In our case, the above command only outputs `stderr`.

There is a shorter way to redirect both `stdout` and `stderr` to a file:

`$ ls /fake/directory &> peanuts.txt`

Now what if I don't want any of that cruft and want to get rid of `stderr` messages completely? Well you can also redirect output to a special file call `/dev/null` and it will discard any input.

`$ ls /fake/directory 2> /dev/null`

## Exercise

What is the following command doing? 

`$ ls /fake/directory >> /dev/null 2>&1`

## Quiz Question

What is the redirector for `stderr`?

## Quiz Answer

`2>`
