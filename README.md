# vim_basics
-`which` - find the location of a programm=
  - `-a` -show all locations
- `nvim --version` - to check which version of neovim is installed

## Vim basics
- `nivim` - to start neovim
- `:Tutor` - start the vim tutor
- `:help`

Let's play: Not-vim-tutor Speedrun

 ### Navigation adn editing

 -  hjkl` move around the cursor
 -  `:` command mode
     -  exit, save, open
 - `q` - quit
 - `q!` -forced quit with out save

 - `i` - insert mode at cursor
 - `a` -insert mode after cursor
 - `A` -insert mode at the end of the line
 - `o` - insert mode on new line below
 - `O` - insert mode on new line above
 - `<esc>` - normal mode

 - `r` - replace character
 - `x` - delete character
 - `u` - undo

 - `d` -delete
   -    This is an operator, it is waiting for an motion
   -    `dw` - delete the next word
   -    `db` - delete the word before
     
- We can use motions on their own or with an operator
  - `w` - move to next word
  - `b` - move to begining of word
  - `e` - move to the end of the word
  - `0` - move to the begining of the line
  - `^` - move to first no-white-space character
  - `$` - move to the end of the line
  - `gg` - move to begining of the line
  - `G` - move to the begining of the File
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