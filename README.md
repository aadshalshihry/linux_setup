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






