---
layout: post
title:  "Grouping files"
date:   2015-12-01 21:30:27 +0100
categories: asciicast
---

<div class='asciicast-wrapper'>
    <script type="text/javascript" src="https://asciinema.org/a/30059.js" id="asciicast-30059" async>
    </script>
</div>

<!-- more -->

Grouping files is a secret weapon of *Vim-CtrlSpace* that allows you to work in
a way that **vanilla Vim doesn’t**. I’ll spare you tricky details about *Vim*
buffers, tabs, and the like. Just **treat grouped files in tabs** as
a workspaces arrangement, OK? See example:

*Docs & Notes* tab groups all project notes and documentation.  Implementing
authentication you can group all related files under *Google OAuth 2.0* tab.
You can even keep files from any projects or directory as you’re not limited by
the project scope. This way a third tab, *Plans & goals* can be added. 

Will **learning Vim-CtrlSpace** land in your **2016 Plan & goals** list?

```console
$ vim

# Open Ember project
[CTRL]+[SPACE]
[B]
>ember<
[Enter]

# Search for `README.md` and open it in the current tab without closing the plugin window
[O]
>readme<
[enter][space]

# Open 3 files in a separate tab (note the `+3` indicator)
[/]
[CTRL]+[U]
>computed<

# Select each file with:
[SHIFT]+[T]

# Clear search term
[/]
[CTRL]+[U]
[/]

# Open list of tabs
[l]

# Give second tab custom label
[j]
[=]
>Computed feature + spec<
[Enter]
[ESC]
[qa]
```
