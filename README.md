# get good with vim

this repo is going to be where i place random vim tips and philosophies, hoping
to one day build a useful answer when people ask me how to get good at vim.

please contribute / make suggestions!

## philosophy

### modal editing

unlike most editors, vim is a modal editor - that means that there are several
"modes" that vim is in. the standard list is `normal`, `insert`, `visual`,
`command` and `ex`.

most of our time is spent browsing and editing code, not writing it. therefore
you should always be in `normal` mode (for fast editing and browsing) unless you
are writing text, in which case you are in `insert` mode.

### on speed

the bottleneck in your editing should be the speed of your brain, followed by
the speed of your typing.

your fingers should move as little as possible and stay anchored to the homerow
(f and j keys specifically) to save time. the mouse is the productivity killer.

get your programming workflow to have an immediate feedback loop - every second
spent waiting is a second lost. use something like
[entr](http://www.entrproject.org/) to automatically re-run commands when your
code changes

use a terminal window manager like tmux so there is no need for a mouse to move
between running processes

### improving yourself

learn one or two new things a week, try to incorporate them into daily practice.

be critical of yourself, always look for ways to improve

use the first few weeks or months of a job to improve your tools and workflow,
since your productivity is not expected to be high, anyway

## things to learn

### basics

* learn how to save / exit (:sav <filename>, :new, :w, :wq, :q, etc)
* learn how to use the help pages
* learn to use jkhl keys. disable the arrow keys, even in insert mode
* learn how to delete (d), change (c) and yank (y) line
* learn how to get into insert mode: oOiIaA
* learn motion commands: wWbBeE$_0
* map capslock to ctrl
* learn character motion commands: fFtT
* learn undo and redo: u and ctrl-r
* learn how to indent/unindent with \< and \>
* learn how to control your pastes with [p and ]p - use J to join the next line to current
* setup your vim config
* learn to search with /

### mediums

* learn to use :s and :%s command with regexes
* learn text objects: ci(, daw, ya', etc
* learn buffer management: :bn, :bp, :bd
* learn to use the verb+object vocabulary of vim ([see grokking vi SO answer](https://gist.github.com/nifl/1178878))
* use ctrl-[ instead of escape
* use larger motions: {}, [[, ]]
* use ctrl-a and ctrl-x in normal mode to increment numbers on the line
* learn about the delete / yank registers
* learn about :registers and "
* learn about window management, including :split, :vsplit, ctrl-w and so on
* install some plugins. uninstall some plugins
* use . to repeat yourself (when going into edit mode, do as much as possible in one go, then use . to repeat it)
* learn how the numbered registers work (history of recent yanks and deletes)
* use character motion with , and ; for repeating
* learn to use ctrl-x ctrl-f for file completion
* get a plugin manager, install some plugins
* learn to use ctrl-n and ctrl-p for keyword completion
* learn how to use jumplist with ctrl-o and ctrl-i. use m' to place a new mark in jumplist
* learn page movement: H, M, L, ctrl-u, ctrl-d, ctrl-f, ctrl-b
* learn useful g commands, like gf and gg and G
* learn how to use linewise visual mode (V)
* learn how to filter visual selection through external programs with !
* learn how to wrap lines using gq in visual mode
* learn to unindent / indent in insert mode (ctrl-d and ctrl-t)
* learn to use :r! for reading external commands in
* setup your vim config again
* use \<number\>G to jump to line (can also use :\<number\>)
* use xp to swap characters
* learn to use * and + registers (or use `!xsel -i` and `!xsel -o`) for system clipboard
* learn to navigate / create folds with zc, zo, etc
* learn to use ctrl-v to insert non-printing characters like \<CR\> or \<Esc\>
* use `/\cfoo` to search for foo with case insensitivity

### advanced

* learn how to use visual blocks (ctrl-v) and editing multiple lines with I
* learn how to record and apply macros (q<register> and @<register> to replay them)
* learn about special registers: "%, "w, "", etc
* learn about "= register (for expression register)
* learn about :later and :earlier
* learn about ctrl-r in insert mode
* learn about ctrl-o in insert mode
* learn to use ctrl-x ctrl-l for line completion
* learn what every key does in normal mode
* play some vimgolf
* learn more g commands like gd, gp, gv, gi, gu, gU, g^g, g_
* learn how to pipe visual selection to xargs
* learn what all shift numbers (!@#$%^&*()_+) do
* learn magic and advanced :s commands
* learn how to repeat :s commands with &
* learn how to use and manage marks
* learn to use :g command (and :g! or :v command)
* delete everything from your vim config except whats necessary
* learn how to jump to tag definitions with ctrl-] and use :ts
* write your own vimscript plugins
* learn to use quickfix window (:cw) with :make or other output
* learn to use :bufdo for executing commands on multiple windows

### movement

![vim movement background](https://raw.githubusercontent.com/LevelbossMike/vim_shortcut_wallpaper/master/vim-shortcuts_2560x1600.png)

## resources

![vim cheat sheet](http://www.viemu.com/vi-vim-cheat-sheet.gif)

### useful plugins

* surround.vim
* nerdtree
* bufexplorer
* tagbar
* ctrl-p
* auto-tags (auto generate tags files for you)
* syntastic


### vimrcs

* [okay's vimrc](https://github.com/okayzed/dotvim/blob/master/rc/vimrc)
* [tmc's vimrc](https://github.com/tmc/dotfiles/blob/master/.vimrc)
* [liorrozen's vimrc](https://gist.github.com/liorrozen/461db13cafe7f960c5fc)


### other people on vim

* [vim-galore](https://github.com/mhinz/vim-galore)
* [grokking vi](https://gist.github.com/nifl/1178878)
* [why oh why use vim?](http://www.viemu.com/a-why-vi-vim.html)
