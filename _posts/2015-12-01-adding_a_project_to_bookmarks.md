---
layout: post
title:  "Adding a project to bookmarks"
date:   2015-11-25 21:30:27 +0100
categories: asciicast
---

<div class='asciicast-wrapper'>
    {% asciicast 29529 %}
</div>

<!--more-->

*vim-ctrlspace* allows you to bookmark your projects. When you run
*vim-ctrlspace* for the first time, the bookmark list is empty. It’s time to
change that! Fasten your seatbelts and add your first project to bookmarks
following the steps below!

{% gist ryrych/5e4ec3fb8ccad17e04d8 %}

After adding the project to bookmarks, you choose the project from the list
using <kbd>j</kbd> and <kbd>k</kbd> keys. Press <kbd>Enter</kbd> to confirm.

An unnamed tab should open.

```
> [1*No Name] ★
```

Press <kbd>o</kbd> to open project file list. Press <kbd>r</kbd> to index all files from the
project. After indexing you should get this message:

```
⌗  Collecting files... Done (399).
```
