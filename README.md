# [Installation](https://www.lazyvim.org/installation)
- [lazyVim](https://www.lazyvim.org/configuration/lazy.nvim)

# vim_basics
- `which` - find the location of a programm=
- `-a` -show all locations
- `nvim --version` - to check which version of neovim is installed

## Vim basics
- `nvim` - to start neovim
- `:Tutor` - start the vim tutor
- `:help`

Let's play: Not-vim-tutor Speedrun

### Open a file / create a file
- `nvim /path/to/your/file.txt`  to open a file
- `nvim /path/to/file1.txt /path/to/file2.txt` to open multiple files
- `:e /path/to/your/another_file.txt` to open a file from a already opened neovim cli
- `:tabnew /path/to/new/file.txt`   to create a new file

### linux command
- :!  should be used before all linux command
- :!ls to get the all the files in the directory
- ` :!gcc <file_name> file.c ` to compile the C file
- :!/<file_name> to run the file

 ### Navigation and editing
 - ` [b ` previous tab
 - ` ]b ` next tab 
 - ` hjkl ` move around the cursor
 -  `:` command mode
     -  exit, save, open
 -  `:!` execution mode
 - `q` - quit
 - `q!` -forced quit with out save

 - `i` - insert mode at cursor
 - `a` - insert mode after cursor
 - `A` - insert mode at the end of the line
 - `o` - insert mode on new line below
 - `O` - insert mode on new line above
 - `ctl + o` - to change to Normal mode for one operation
 - `<esc>` - normal mode

 - `:%s/search_word/word_to_replace/g` replace search_word with wrod_to_replace and globally
 - `:%s/search_word/word_to_replace/gi` replace search_word with wrod_to_replace and globally and ignoring the case
 - `r` - replace character
 - `x` - delete character
 - `u` - undo

 - `d` -delete
   -    This is an operator, it is waiting for an motion
   -    `dX` - delete the next character
   -    `dw` - delete the next word
   -    `db` - delete the word before
   -    `dd` - delete a single line
   -    `4dd` - delete 4 consecutive lines
   -    `ndd` - delete **n** number of consecutive lines starting from the cursor
   -    `d$`  - cut/delete everything from the cursor to the end of the line
   -    `dG`  - delete all lines from the current cursor position to the end of the file
   -    `%d`  - delete everything from the files
   -    `dgg` - delete everything from the current line to the top of the text/file
   -    `g /linux/d` -delete all lines containing the word _linux_
   -    `g /^T/d` - delete lines that begin with a specific letter **T**
   -    `g /^$/d` - delete or remove all blank lines in your text file or code
     
- We can use motions on their own or with an operator
  - `w` - move to next word
  - `b` - move to begining of word
  - `e` - move to the end of the word
  - `0` - move to the begining of the line
  - `^` - move to first no-white-space character
  - `$` - move to the end of the line
  - `gg` - move to begining of the File
  - `G` - move to the end of the File
  - `f` - find character on line
  - `t` - find character on line, before
  - `F` - find character on line, backeards
  - `T` - find character on line, before, backeards
  - `;` - repeat last `f` `t` `F` `T`
  - `,` - repeat last `f` `t` `F` `T` in opposit direction
  - `}` - move to next paragraph
  - `{` - move to previous paragraph
  - `/` - search
  - `n` - next search result
  - `N` - previous search result

 - `y` - copy  
   - `yy`    - copy a single line 
   - `3yy`   - copy 3 lines
   - `y$`    - copy everything form the cursor to the end of the line
   - `y^`    - copy everything from the start of the line to the cursor
   - `yiw`   - copy the current word

 - `P` pasting/putting
   - `P(uppercase)` - Paste before the cursor
   - `p(lowercase)` - Paste after the cursor
  
- `V` visual mode and this also will select
   - `V(uppercase)` enter to visual-mode. This will select the entire line
   -  `v (lowercase)` to enter visual-mode. This will start selecting the line from the cursor is

 *** `CTRL+V` visual-block-mode. and move the cursor to the end of where you want to copy or cut.
 press `y` to copy or press `d` to cut. Move the cursor to where you want to paste your selection. ***
