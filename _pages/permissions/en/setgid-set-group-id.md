---
layout: page
title: Setgid
permalink: /en/setgid/
cat: permissions
order: 6
ref: setgid
lang: en
---

## Lesson Content

Similar to the set user ID permission bit, there is a set group ID (SGID) permission bit. This bit allows a program to run as if it was a member of that group. 

Let's look at one example: 

```
$ ls -l /usr/bin/wall
-rwxr-sr-x 1 root tty 19024 Dec 14 11:45 /usr/bin/wall
```

We can see now that the permission bit is in the group permission set. 

**Modifying SGID**  

```
$ sudo chmod g+s myfile
$ sudo chmod 2555 myfile
```

The numerical representation for SGID is 2.

## Exercise

No exercises for this lesson.

## Quiz Question

What number represents the SGID?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /> 
## Quiz Answer

2