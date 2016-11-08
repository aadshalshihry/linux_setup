# ubuntu_setup
My Ubuntu Setup where it has every thing I like to use in ubuntu
### Add flashback:
* Easy to use
* Everything is accessable

```bash
sudo apt-get update
sudo apt-get install gnome-session-flashback
```

====================================================

### Install git:

```bash
sudo apt-get install git
```
#### Config git:

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@domain.com"
```
#### List git configuration:

```bash
git config --list
```
#### Config git in file:
```bash
vim ~/.gitconfig
```
> ### ~/.gitconfig contents
> > [user]<br />
> > >	 name = Your Name <br /> 
> > >	 email = youremail@domain.com

#### Caching your GitHub password in Git:
* To use caching:
```bash
git config --global credential.helper cache
```
* To change the default password cache timeout:

```bash
git config --global credential.helper 'cache --timeout=3600'
``` 


#### Git gitignore file
* You need to set up your global ```bash core.excludesfile ``` configuration file to point to this global ignore file.

```bash
git config --global core.excludesfile '~/.gitignore'
```

1. Download the file from github to another folder  
2. make soft link to home 

```bash
cd folder_name
git clone https://github.com/aadshalshihry/gitignore.git
cd gitignore
ln -s .gitignore ~
```

##### Links:
1. https://help.github.com/articles/caching-your-github-password-in-git/
2. http://stackoverflow.com/questions/7335420/global-git-ignore

==================================================


### Guake
* Guake is a dropdown terminal

```bash
sudo apt-get install guake
```

##### Links:
1. http://guake.org

==================================================


### Oh-My-Zsh
* It will give batter appearance and more functionality

```bash
sudo apt-get install zsh
sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
chsh -s /bin/zsh

```
> These command will install and setup it to work with Guake


```python

ZSH_THEME="agnoster"
```
> Chage the Defualt interperter in the Guake Preference to */bin/zsh*

> To make agnoster them work visit the following websites:
>   * https://powerline.readthedocs.org/en/latest/installation/linux.html#font-installation
>     * install powerline fonts
>   
##### Links
1. http://ohmyz.sh/


==================================================


#### Tmux 
> tmux is a terminal multiplexer. It allows you to access a tmux terminal using multiple virtual terminals.

```bash
sudo apt-get install tmux
```

##### Links
1. https://www.digitalocean.com/community/tutorials/how-to-install-and-use-tmux-on-ubuntu-12-10--2

==========================================================

#### Dual screen:

```bash
sudo apt-get install compizconfig-settings-manager compiz-plugins
```

##### Links:
1. http://askubuntu.com/questions/519651/add-workspaces-with-gnome-classic-and-ubuntu-14-04



====================================================================


#### Vim Setup

```bash
cd Download
git clone https://github.com/aadshalshihry/dotfiles.git
cd dotfiles
cp .vimrc ~
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```

* Install the colorscheme
```bash
cd ~/.vim/bundle
git clone git://github.com/altercation/vim-colors-solarized.git
mv vim-colors-solarized ~/.vim/bundle/
```

##### Links: 
1. https://github.com/VundleVim/Vundle.vim
2. http://ethanschoonover.com/solarized/vim-colors-solarized

=========================================================

#### Installing Microsoft Fonts
```bash
  sudo apt-get install ttf-mscorefonts-installer
```
##### Links:
1. https://community.linuxmint.com/tutorial/view/29

==============================================================

##### Install Node and NPM
* V6
```
curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
sudo apt-get install -y nodejs
```

* V7
```
curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -
sudo apt-get install -y nodejs
```

* express, gulp, bower, grunt
```
npm install -g express gulp bower grunt
```
