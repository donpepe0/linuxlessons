---
layout: page
title: /etc/group
permalink: /en/etc-group/
cat: user-management
order: 5
ref: etc-group
lang: en
---

## Lesson Content

Another file that is used in user management is the `/etc/group` file. This file allows for different groups with different permissions. 

```
$ cat /etc/group

root:*:0:pete
```

Very similar to the `/etc/password` field, the `/etc/group` fields are as follows:

* Group name
* Group password - there isn't a need to set a group password, using an elevated privilege like sudo is standard. A `*` will be put in place as the default value.
* Group ID (GID)
* List of users - you can manually specify users you want in a specific group

## Exercise

Run the command `groups`. What do you see?

## Quiz Question

What is the GID of root?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
## Quiz Answer

`0`