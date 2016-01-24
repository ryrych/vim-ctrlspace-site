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

Opening project

1. <kbd>CTRL</kbd> + <kbd>SPACE</kbd>
2. <kbd>B</kbd>
3. Enter project name `>ember<`
4. Confirm with <kbd>Enter</kbd>

Finding file and opening it in the first tab

1. <kbd>O</kbd>
2. Enter file name `>readme<` and confirm with <kbd>Enter</kbd>
3. Press <kbd>space</kbd> to add the file to the tab without closing the plugin window

Opening another 3 files in a separate tab

1. Open search mode with <kbd>/</kbd>
2. Press <kbd>CTRL</kbd> + <kbd>U</kbd> to clear the previous search term
3. Type `>computed<` to find new files
4. Open each found file with <kbd>Shift</kbd> + <kbd>T</kbd>

Adding a custom tab label

1. Press <kbd>Backspace</kbd> to exit search mode
2. Press <kbd>l</kbd> to open a list of tabs
3. Press <kbd>=</kbd> to change the default label
