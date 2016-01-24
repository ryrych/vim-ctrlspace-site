---
layout: page
title: Getting Started
permalink: /getting-started/
---

## Intro

Below you can find information how to setup *Vim* with **basic config**. This
way:

- You can follow *asciicasts* and other tips
- You can try *Vim-CtrlSpace* without touching your everyday setup

## Learn *Vim-CtrlSpace* in 30 minutes

*Vim* is said to have **steep learning curve**. It’s not true. It’s rather an
urban legend.  [Ben Orenstein][1] says that **you can learn to use *Vim* in 30
minutes**:

> Over the years, the popular mythology around vim has become that it’s insanely
> difficult to learn; a task to be attempted by only those with the thickest of
> neck-beards. I’ve heard dozens of times from folks who are convinced it will
> take them months to reach proficiency.
>
> These beliefs are false.
>
—Ben Orenstein in [The Vim Learning Curve is a Myth][2]

We’re sure that **you can also learn Vim-CtrlSpace in 30 minutes**! Ready?

## Installation

### Getting Vundle

**Follow**: *Step 1* and *Step 2*
**Skip**: *Step 3* and *Step 4*

from [Vundle Quick Start Guide][3]

### Install *The Silver Searcher*

```
brew install the_silver_searcher
```

- [How to install in Linux and other systems][4]
- In case of problems see [how to configure The Silver Searcher for Vim-CtrlSpace][5]

### Get our basic vimrc config

To not mess up your original config, plugins will be installed in
`~/vim-ctrlspace-learning` You can [change that][6].

Copy the content and store it somewhere.

```vim
set nocompatible
filetype off

set rtp+=~/.vim/bundle/Vundle.vim
" Change path if necessary
call vundle#begin('~/vim-ctrlspace-learning')

Plugin 'VundleVim/Vundle.vim'
Plugin 'szw/vim-ctrlspace'
Plugin 'NLKNguyen/papercolor-theme'

call vundle#end()
filetype plugin indent on

set t_Co=256
set background=dark
colorscheme PaperColor

set nocompatible
set hidden
set wildignore=.git,.svn,CVS,*.o,*.a,*.class,*.mo,*.la,*.so,*.obj,*.swp,*.jpg,*.png,*.xpm,*.gif,*.pyc,tags,*.tags

if has("gui_running")
  " Settings for MacVim and Inconsolata font
  let g:CtrlSpaceSymbols = { "File": "◯", "CTab": "▣", "Tabs": "▢" }
endif

if executable("ag")
    let g:CtrlSpaceGlobCommand = 'ag -l --nocolor -g ""'
endif

let g:CtrlSpaceIgnoredFiles = '\v(tmp|temp|Godeps)[\/]'
```

### Install Vim-CtrlSpace and plugins

Open *Vim*:

```
mvim -u path-to-the-downloaded-config
```

Install plugins using *Vundle*:

```
:PluginInstall
```

Restart *Vim* (recommended).

## First try!

Now you can [add your first project to bookmarks!][7]


[1]: https://twitter.com/r00k
[2]: https://robots.thoughtbot.com/the-vim-learning-curve-is-a-myth
[3]: https://github.com/VundleVim/Vundle.vim#quick-start
[4]: https://github.com/ggreer/the_silver_searcher#linux
[5]: https://github.com/vim-ctrlspace/vim-ctrlspace#glob-command
[6]: https://gist.github.com/ryrych/895bbabd3f6c40bf7d29#file-vim-ctrlspace-vimrc-L6
[7]: asciicast/2015/11/25/adding_a_project_to_bookmarks.html
