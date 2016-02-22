# VIM Basics

## Basic VIM Modes

* Command / Normal (default):
	Used to give commands to VIM and not edit text directly. 
* Edit:
	This is true edit mode
* Visual:
	visual selection, etc.

### Entering Edit Mode

To enter "edit mode", user can press **i** to insert or delete text. To exit from Edit mode, a user can press "Esc" key to return to Command mode. Vim supports various ways to enter this mode, some of them are:
- **a** - insert after current location (append)
- **I** - insert AT START of current line
- **A** - insert AFTER END of current line
- **o** - insert line below current line (open)
- **O** - insert line ABOVE current line  

Rest can be found in references below.

### Command Mode options

1. :w : Write
1. :q : quit
1. :wq : Write and Quit
1. :!<cmd> : Execute Command

### Other options

- When in command mode, a user can press **dd** to delete current line
- To copy a line in Vim (in Command mode), press **yy** key. This line can be pasted by pressing **p** key.
- To undo a change in file, enter Command mode by pressing "Esc" key, and then press **u** key. To redo something, **CTRL-R** can be pressed.
- History of all the inputs entered in Command mode is accessible by pressing Up and Down keys.
- Vim [Write with Sudo trick](http://garage4hackers.com/showthread.php?t=3100&page=2&p=13535&viewfull=1#post13535)

## References
* [VIM Tutorials](http://vim.wikia.com/wiki/Tutorial)
* [Working Efficiently with VIM](https://blog.anantshri.info/working-efficiently-with-vi-vim/)
* [Undo and Redo](http://vim.wikia.com/wiki/Undo_and_Redo)
