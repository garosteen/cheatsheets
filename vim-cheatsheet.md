# Vim Cheatsheet #

If you're looking for the basics, they might not be here.

# NAVIGATION

* `+`	- down - to first non-whitespace character
* `-` - up - to first non-whitespace character

* `w` - to beginning of next word
* `b`	- to beginning of previous word 

* `e` - to end of next word

* `L` -  To end of page
* `M` -  Middle of page
* `H` -  Top of page

* `G` - end of file
* `10G` - 10th line
* `:10` - 10th line
* `gg` - beginning of file

* `%` - move cursor to matching bracket
* `*`, `#` - move to next/previous occurence of word under cursor

* `ctl-b` - back one page
* `ctl-f` - forward one page
* `0` - move cursor to beginning of line
* `$` - move cursor to end of line

## Folding ##

* `zM` - Fold Max
* `zm` - Fold more
* `zR` - Fold Least (Reduce)
* `zr` - Fold less
* `:set foldlevel=1` - Or any number, will set the fold level.
* `:set foldlevel?` - Gives the current fold level.
    
## Editing ##

## Insert mode commands ##

* `CTRL-w` - delete back to beginning of previous word
* `CTRL-t` - indent current line
* `CTRL-d` - de-indent current line
(These two commands are GAME-CHANGING!!)
* `CTRL-v <tab>` - insert a hard tab, even if it would normally be converted to spaces
* `CTRL-n` - Find next keyword (autocomplete) 
* `CTRL-p` - Find previous keyword (autocomplete)

See `:help ins-special-keys` for more info

## Going into insert mode ##
* `a` - append AFTER cursor. (insert mode)
* `A` - append at end of line (insert mode)
* `o` - open a new line after cursor. (insert mode)
* `O` - open a new line above current line

## Replacing ##

* `r` - replace character
* `R` - replace characters from cursor onward - go into "REPLACE" mode

## Combined commands ##


## Misc ##

* `d/foo` - delete from cursor to next occurance of "foo" (non-inclusive)

* `CTRL-a` - Increment number at (end of) word under cursor
* `CTRL-x` - Decrement number at (end of) word under cursor

* `gU`, `gu` - Change case (upper/lower)
* `~` - Change case of character under cursor and move right one character
# SETTINGS #

* `:set number` - turn on line numbers
* `:set nonumber` - turn off line numbers

* `:syntax on` - turn on syntax highlighting
* `:syntax off` - turn off syntax highlighting

