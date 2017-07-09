# Dotfiles

Managing dotfiles between boxes.

## Setup

Clone the repo to your home directory.

```
~/$ git clone https://github.com/natemeier/dotfiles
```

I use [GNU Stow](https://www.gnu.org/software/stow/) to manage symbolic links between files in this repository and the home directory, inspired by [this](http://brandon.invergo.net/news/2012-05-26-using-gnu-stow-to-manage-your-dotfiles.html). 

### Install stow

Use the package manager for your system. I pretty much stick to OSX and Ubuntu.

#### OSX
```
$ brew install stow
```

#### Debian
```
$ sudo apt-get install stow
```

### Using Stow

Change into the dotfiles directory and use `stow` to selectively symlink files.
You may need to re/move existing copies to make room for you new, version-controlled files.

```
~/$ cd dotfiles
~/dotfiles/$ stow git
~/dotfiles/$ stow vim
~/dotfiles/$ stow zsh
```