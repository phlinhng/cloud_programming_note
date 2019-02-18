## Install `zsh` & change shell for macOS
```
brew install zsh zsh-completions zsh-syntax-highlighting zsh-autosuggestions
chsh -s /usr/local/bin/zsh
```
if can't change shell
`sudo vim /etc/shells`
add `/usr/local/bin/zsh` to the end

## Install `oh-my-zsh`
```
git clone https://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh

cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc
vim .zshrc

+# zsh-completions
+ fpath=(/usr/local/share/zsh-completions $fpath)

+# zsh-syntax-highlighting
+ source /usr/local/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh

+# zsh-autosuggestions
+ source /usr/local/share/zsh-autosuggestions/zsh-autosuggestions.zsh

#powerlevel9k theme
git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k
+ ZSH_THEME="powerlevel9k/powerlevel9k"
```

## restart zsh
```
rm -f ~/.zcompdump
compinit
```

## color profile for iTerm2
`git clone https://github.com/mbadolato/iTerm2-Color-Schemes.git`

## check
```
echo $SHELL
echo $ZSH_VERSION
zsh --version
which zsh
```