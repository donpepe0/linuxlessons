---
layout: page
title: sort
permalink: /en/sort-command/
cat: text-manipulation
order: 12
ref: sort-command
lang: en
---

## Lesson Content

The `sort` command is useful for sorting lines.

```
file1.txt
dog
cow
cat
elephant
bird
```
```
$ sort file1.txt
bird
cat
cow
dog
elephant
```

You can also do a reverse sort: 

```
$ sort -r file1.txt
elephant
dog
cow
cat
bird
```

And also sort via numerical value: 

```
$ sort -n file1.txt
bird
cat
cow
elephant
dog
```

## Exercise

The real power of `sort` comes with its ability to be combined with other commands, try the following command and see what happens?

`$ ls /etc | sort -rn`

## Quiz Question

What flag do you use to do a reverse sort?

## Quiz Answer

`-r`
