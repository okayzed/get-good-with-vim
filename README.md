# vim--


this repo is going to be where i place random vim tips and philosophies, hoping
to one day build a useful answer when people ask me how to get good at vim.

please contribute / make suggestions!

## philosophy

most of our time is spent browsing and editing code, not writing it. therefore
you should always be in normal mode (for fast editing and browsing) unless you
are writing text.

your fingers should move as little as possible and stay anchored to the homerow
to save time. the mouse is the productivity killer.

learn one or two new things a week, try to incorporate them into daily practice

the bottleneck in your editing should be the speed of your brain, followed by
the speed of your typing.

use a terminal window manager like tmux, get your programming workflow to have
an immediate feedback loop - every second spent waiting is a second lost




### basics

* learn how to save / exit (:sav <filename>, :new, :w, :wq, :q, etc)
* learn how to use the help pages
* learn to use jkhl keys. disable the arrow keys, even in insert mode
* learn how to delete (d), change (c) and yank (y) line
* learn how to get into insert mode: oOiIaA
* learn motion commands: wbe$_0
* map capslock to ctrl
* learn character motion commands: fFtT
* learn undo and redo: u and ctrl-r
* learn how to control your pastes with [p and ]p - use J to join the next line to current
* setup your vim config
* learn to search with /

### mediums

* learn how to use jumplist with ctrl-o and ctrl-i. use m' to place a new mark in jumplist
* learn to use :s and :%s command with regexes
* learn text objects: ci(, daw, ya', etc
* learn to use the verb+object vocabulary of vim (see grokking vi SO answer)
* use ctrl-[ instead of escape
* use larger motions: {}, [[, ]]
* learn about window management, including :split, :vsplit, ctrl-w and so on
* install some plugins. uninstall some plugins
* use . to repeat yourself (when going into edit mode, do as much as possible in one go, then use . to repeat it)
* learn page movement: H, M, L, ctrl-u, ctrl-d, ctrl-f, ctrl-b
* learn useful g commands, like gf and gg and G
* learn how to use linewise visual mode (V)
* learn how to filter visual selection through external programs with !

### advanced

* learn how to use visual blocks (ctrl-v) and editing multiple lines with I
* learn how to record and apply macros (q<register> and @<register> to replay them)
* learn about :registers and "
* learn about :later and :earlier
* learn about ctrl-r in insert mode
* learn about ctrl-o in insert mode
* learn what every key does in normal mode
* play some vimgolf
* learn more g commands like g^g
* learn how to pipe visual selection to xargs
* learn what all shift numbers (!@#$%^&*()_+) do
* learn magic and advanced :s commands
* learn to use :g command
* write your own vimscript plugins


### plugins

* get a plugin manager, install some plugins
* useful plugins: surround.vim, syntastic, nerdtree, bufexplorer, tagbar
