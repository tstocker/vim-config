# Install

Clone the project to `~/.vim/`

```shell
git clone git@github.com:tstocker/vim-config.git ~/.vim/
```

Install `vim-plug`
```shell
# using taskfile
task install -t ~/.vim/Taskfile.yml

# using command line
curl -fLo ~/.vim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

Please notice that you need remove the `~/.vimrc` file  if you already have one either `~/.vim/virmc will not be use`


Now we are going to install plugins

open vimrc
```
vim ~/.vim/vimrc
```

run in vim 
```vim
:PLugInstall
```

If you need to update plugins run
```vim
:PlugUpdate
```

# VIM Commands

## Fold commands

`zo` to open a single fold under the cursor.

`zc` to close the fold under the cursor.

`zR` to open all folds.

`zM` to close all folds.

vim-open-close-fold.gif
Type `:help folding` for more information.

## search in current file
`/`

`*` on word to search forward 
`#` on word to search backward

## NERDTree
Open NERDTree
`<F3>` or `:NERDTreeToggle`

navigate between file and NERDTree
`Ctrl+w` `w` cycle though all windows
`Ctrl+w` `h` takes you left a window
`Ctrl+w` `j` takes you down a window
`Ctrl+w` `k` takes you up a window
`Ctrl+w` `l` takes you right a window

in file tree
`o` - open files in previous window
`i` - open files in horizontally split windows
`s` - open files in vertically split windows
`t` - open files in new tabs

refresh tree :
`r` on directory in NERDTree to refresh directory
`R` in NERDTree for refresh all the tree


## JsDoc

plugin : [vim-jsdoc](https://github.com/heavenshell/vim-jsdoc)

 `:JsDoc`  on function keyword to add jsdoc

 `:JsDocFormat` add jsDoc to all function
