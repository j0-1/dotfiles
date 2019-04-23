# dotfiles
Just my personal dotfiles

## Symlinks
From homedir:
* `ln -s dotfiles/vim/vimrc .vimrc`
* `ln -s dotfiles/ag/agignore .agignore`

## Colors
* Lucius2 https://github.com/maksimr/Lucius2
* Jellybeans https://github.com/nanotech/jellybeans.vim

```
mkdir -p ~/.vim/colors
cd ~/.vim/colors
curl -O https://raw.githubusercontent.com/nanotech/jellybeans.vim/master/colors/jellybeans.vim
curl -O https://raw.githubusercontent.com/maksimr/Lucius2/master/colors/lucius.vim
```

## minpac
* Install minpac to opt
```
mkdir -p ~/.vim/pack/minpac/opt
cd ~/.vim/pack/minpac/opt
git clone https://github.com/k-takata/minpac.git
```
* Make sure the following is in vimrc
```
packadd minpac
call minpac#init()
```
* Add packages
```
call minpac#add('tpope/vim-surround')
call minpac#add('k-takata/minpac', {'type':'opt'})
```
* restart

NOTE: this is already in this vimrc, just being specific for the init work on a new system
