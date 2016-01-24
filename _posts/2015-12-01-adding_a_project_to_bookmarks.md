---
layout: post
title:  "Adding a project to bookmarks"
date:   2015-11-25 21:30:27 +0100
categories: asciicast
---

<div class='asciicast-wrapper'>
    <script type="text/javascript" src="https://asciinema.org/a/29529.js" id="asciicast-29529" async>
    </script>
</div>

<!-- more -->

*Vim-CtrlSpace* allows you to bookmark your projects. When you run
*Vim-CtrlSpace* for the first time, the bookmark list is empty. It’s time to
change that! Fasten your seatbelts and add your first project to bookmarks
following the steps below!

1. <kbd>CTRL</kbd>+<kbd>SPACE</kbd>
2. <kbd>b</kbd>
3. <kbd>a</kbd>
4. *Vim-CtrlSpace* will ask you to type the path to the project
5. Confirm the path with <kbd>Enter</kbd>
6. Optionally you can change the bookmark name

After adding the project to bookmarks, choose the project from the list using
either:

- <kbd>j</kbd> and <kbd>k</kbd>
- toggling search mode with <kbd>/</kbd> when the list is long

Press <kbd>Enter</kbd> to confirm the choice. An unnamed tab should open.

```
> [1*No Name] ★
```

1. Press <kbd>o</kbd> to open project file list.
2. Press <kbd>r</kbd> to index all project files.

After indexing you should get this message:

```
⌗  Collecting files... Done (399).
```

Now you’re ready to feel the power of *Vim-CtrlSpace*!

## Common questions

### Re-indexing — do I need it?

Almost **each editor**, or *IDE* you have had experience with, **re-index
files**. Many of them do it automatically for you. This allows for faster
searching files. Some *IDE* like *RubyMine* can, in large projects, hang even
a powerful *Macbook Pro*.

*Vim-CtrlSpace* allows you to re-index files **manually**. Don’t worry about
forgetting to re-index as sooner or later it’ll become your habit.

### Re-indexing — when?

Usually when:

- Switching between *Git* (or any other *VCS*) branches
- Regenerating *Ctags*
- Adding or removing files

Remember that you can still open the files with:

- `:e file-name.rb`
- [The NERD Tree][1]
- [vinegar.vim][2]
- Your favourite tool, etc.

New files will not be available when **using fuzzy search** until you re-index
them. That’s it!


[1]: https://github.com/scrooloose/nerdtree
[2]: https://github.com/tpope/vim-vinegar
