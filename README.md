This tutorial is for macOS.

## Building environment for the course

### 1. Install Java & Eclipse for JEE
```
brew cask install java brew eclipse-jee
```
### 2. Install AWS-CLI & Boto3 for Python 3
pip3 install Boto3 awscli

## 3. Install [AWS Toolkit for Eclipse](https://docs.aws.amazon.com/toolkit-for-eclipse/v1/user-guide/getting-started.html)

## Prerequest
* [Xcode](https://itunes.apple.com/us/app/xcode/id497799835?mt=12)
* Homebrew (A must-have powerful package manager for developers using macOS)
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
* Python 3 & pip3 (Homebrew version)
```
brew install python3
```
Use `python3` & `pip3` to call python3, and `python` and `pip` for built-in python2.
* (optional) zsh
```
brew install zsh zsh-completions zsh-syntax-highlighting zsh-autosuggestions

chsh -s /usr/local/bin/zsh
# sudo vim /etc/shells
# add /usr/local/bin/zsh to the end

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

#restart zsh
rm -f ~/.zcompdump
compinit

#color profile for iTerm2
git clone https://github.com/mbadolato/iTerm2-Color-Schemes.git

#check
echo $SHELL
echo $ZSH_VERSION
zsh --version
which zshbrew install zsh zsh-completions zsh-syntax-highlighting zsh-autosuggestions

chsh -s /usr/local/bin/zsh
# sudo vim /etc/shells
# add /usr/local/bin/zsh to the end

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

#restart zsh
rm -f ~/.zcompdump
compinit

#color profile for iTerm2
git clone https://github.com/mbadolato/iTerm2-Color-Schemes.git

#check
echo $SHELL
echo $ZSH_VERSION
zsh --version
which zsh
```
* (optional) iTerm 2
`brew cask install iTerm 2`