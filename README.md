# Configuration files

## VIM

### With plugins

Use the file `vimrcFull` and copy it at you `$HOME` with the name of `.vimrc`.

In order to make the plugins to work you must install
[vim-plug](https://github.com/junegunn/vim-plug), issue this command, it will
do just that.

```sh
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

Now, install the plugins, ignore the errors and warnings, they just show up
the first time you use VIM with the new configuration.

```sh
vim +PlugInstall
```

### Minimal

Use the file `vimrcMinimal` and copy it at you `$HOME` with the name of
`.vimrc`.

## ZSH

### With plugins

Use [ohmyzsh](https://ohmyz.sh/).

Copy the file `zshFull` to `$HOME/.zshrc`.

## TMUX

### With plugins

Install [ohmytmux](https://github.com/gpakosz/.tmux).

Copy the file `tmuxFull` to `$HOME/.tmux.conf.local`
