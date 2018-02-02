---
layout: page
title: uniq
permalink: /en/uniq-command/
cat: text-manipulation
order: 14
ref: uniq-command
lang: en
---

## Lesson Content

The `uniq` (unique) command is another useful tool for parsing text.

Let's say you had a file with lots of duplicates:

```
reading.txt
book
book
paper
paper
article
article
magazine
```

And you wanted to remove the duplicates, well you can use the `uniq` command:

```
$ uniq reading.txt
book
paper
article
magazine
```

Let's get the count of how many occurrences of a line:

```
$ uniq -c reading.txt
2 book
2 paper
2 article
1 magazine
```

Let's just get unique values:

```
$ uniq -u reading.txt
magazine
```

Let's just get duplicate values:

```
$ uniq -d reading.txt
book
paper
article
```

**Note**: `uniq` does not detect duplicate lines unless they are adjacent. For eg:

Let's say you had a file with duplicates which are not adjacent:

```
reading.txt
book
paper
book
paper
article
magazine
article
```

```
$ uniq reading.txt
reading.txt
book
paper
book
paper
article
magazine
article
```

The result returned by `uniq` will contain all the entries unlike the very first
example.

To overcome this limitation of `uniq` we can use `sort` in combination with `uniq`:

```
$ sort reading.txt | uniq
article
book
magazine
paper
```

## Exercise

What result would you get if you tried `uniq -uc`?

## Quiz Question

What command would you use to remove duplicates in a file?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
## Quiz Answer

`uniq`
