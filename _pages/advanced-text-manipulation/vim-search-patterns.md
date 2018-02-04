---
layout: page
title: vim Search Patterns
permalink: /en/vim-search-patterns/
cat: advanced-text-manipulation
order: 4
ref: vim-search-patterns
lang: en
---

## Lesson Content

To search for an expression just type the `/` key and then your search result while you are in a vim session. Once you hit enter, you can press `n` to go forward or `N` to go backward in your search results.

My pretty file is very pretty.

`/pretty`

will find the `pretty` words in the text file.



The `?` search command will search the text file backwards, so in the previous example, the last pretty would come up first. 

My pretty file is very pretty.

`?pretty`

will find the `pretty` words in the text file.

## Exercise

Play with the search key, open a text file in vim with: `vim [textfile]` and start searching!

## Quiz Question

What key is used to search in vim?  
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
## Quiz Answer

`/`