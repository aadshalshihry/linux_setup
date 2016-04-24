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
sudo apt-get intall git
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
> > [user]
> > 	name = Your Name <br /> 
> > 	email = youremail@domain.com

#### Caching your GitHub password in Git:
* To use caching:
```bash
git config --global credential.helper cache
```
* To change the default password cache timeout:

```bash
git config --global credential.helper 'cache --timeout=3600'
``` 
https://help.github.com/articles/caching-your-github-password-in-git/

==================================================


### Guake
* Guake is a dropdown terminal

```bash
sudo apt-get install guake
```
http://guake.org

==================================================


### Oh-My-Zsh
* It will give batter appearance and more functionality

```bash
sudo apt-get install zsh
chsh -s /bin/zsh
git clone https://github.com/aadshalshihry/oh-my-zsh.git ~/.oh-my-zsh
cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc
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

http://ohmyz.sh/


==================================================






