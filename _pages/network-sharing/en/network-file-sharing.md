---
layout: page
title: File Sharing Overview 
permalink: /en/network-file-sharing/
cat: network-sharing
order: 1
ref: network-file-sharing
lang: en
---

## Lesson Content

You usually are not the only computer on your network, this is especially the case if you're working in a commercial environment. When we want to transfer data from one machine to another, sometimes it maybe easier to connect a USB drive and manually copy them. But for the most part, if you're working with machines on the same network, the way to transfer data is through network file sharing. 

In this course we'll go over a couple of different methods to copy data to and from different machines on your network. We'll discuss some simple file copies, then we'll talk about mounting entire directories on your machine that act as a separate drive. 

One simple file sharing tool is the **scp** command. The scp command stands for secure copy, it works exactly the way the cp command does, but allows you to copy from one host over to another host on the same network. It works via ssh so all your actions are using the same authentication and security as ssh. 

**To copy a file over from local host to a remote host**

`$ scp myfile.txt username@remotehost.com:/remote/directory`

**To copy a file from a remote host to your local host**

`$ scp username@remotehost.com:/remote/directory/myfile.txt /local/directory`

**To copy over a directory from your local host to a remote host**

`$ scp -r mydir username@remotehost.com:/remote/directory`

## Exercise

Try to copy a file over with scp from one machine to another.

## Quiz Question

What command can you use to securely copy files from one host to another?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /> 
## Quiz Answer

`scp`
