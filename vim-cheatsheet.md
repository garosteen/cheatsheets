# Vim Cheatsheet #

If you're looking for the basics, they might not be here.

# NAVIGATION

* `+` / `-`	- up/down - to first non-whitespace character

* `w` / `b` - to beginning of next/previous word

* `e` - to end of next word

* `L` -  To end of page
* `M` -  Middle of page
* `H` -  Top of page

* `G` - end of file
* `10G`, `:10` - 10th line
* `gg` - beginning of file

* `%` - move cursor to matching bracket
* `*`, `#` - move to next/previous occurence of word under cursor

* `ctl-b` - back one page
* `ctl-f` - forward one page
* `0` / `$` - move cursor to beginning/end of line

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
* `CTRL-v <tab>` - insert a hard tab, even if it would normally be converted to spaces
* `CTRL-n` - Find next keyword (autocomplete) 
* `CTRL-p` - Find previous keyword (autocomplete)
* `CTRL-r`+`"` - Paste from default register (Works on command line as well!)
  * + `CTRL-w` - Pastes the word under the cursor

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

## Finding ##

* `:vim[grep][!] /{pattern}/[g][j] {file} ...` - Search within files. Populates the quickfix list, shared between all windows.
  * `[g]` - Match all searches, not just one per line
  * `[j]` - Do not jump to first match automatically
  * `:lvimgrep` - Populate the location list instead, local to the current window.
* `:cw` or `:copen` - Open the quickfix list
  * `:colder`, `:lolder`, `:cnewer`, `lnewer` - Show older/newer searches for quickfix/location list.
* `:lw` or `:lopen` - Open the location list
# SETTINGS #

* `:set number` - turn on line numbers
* `:set nonumber` - turn off line numbers

* `:syntax on` - turn on syntax highlighting
* `:syntax off` - turn off syntax highlighting


