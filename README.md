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

Use the file `vimrcMinimal` and copy it at your `$HOME` with the name of
`.vimrc`.

## ZSH

Use [ohmyzsh](https://ohmyz.sh/).

Copy the file `zshFull` to `~/.zshrc`.

## TMUX

Copy the file `tmuxFull` to `~/.tmux.conf`.

Run this in your terminal, it will install some extensions for URxvt.

```zsh
git clone https://github.com/muennich/urxvt-perls && \
cd urxvt-perls && \
mkdir -p ~/.urxvt/ext && \
cp keyboard-select deprecated/url-select deprecated/clipboard ~/.urxvt/ext && \
cd .. && rm -rf urxvt-perls
```

Now, copy `Xresources` to your home directory as `.Xresources`, then run
`xrdb ~/.Xresources`, close your terminal and open it again.
