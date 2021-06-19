# vimrc
My vimrc file "~/.vimrc" for Linux

# Vim Configuration file for Ubuntu 20

Due to some reasons, Plugins are not working in Ubuntu 20.
So the plugins are loaded here using Vundle

> Vundle is short for Vim bundle and is a Vim plugin manager.
## How to use Vundle?
You can follow this [guide](https://github.com/VundleVim/Vundle.vim)

**--------OR--------**
### Follow These Steps

#### 1: Set Up Vundle
``` 
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
#### Step 2
Copy the contents of `config.vim` file into your `~/.vimrc` file. Save and quit.

#### Step 3
Launch `vim` and run `:PluginInstall`


## Want to use as Root user also? 

Exactly same procedure but instaed of copying contents, just make a soft link.

#### 1: Set Up Vundle
```
sudo -s
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```

#### Step 2: Create Softlink
```
ln -s /home/ajinzrathod/.vimrc ~/.vimrc
```

#### Step 3
Launch `vim` and run `:PluginInstall`


## To use in Fedora

[Source](https://dhilst.github.io/2019/01/19/vim-clipboard-on-fedora.html)
* Install vimx: 

```bash
sudo dnf install -y vim-X11
```

* Add `set clipboard=unnamedplus` to your .vimrc
```
set clipboard=unnamedplus
```

Add `alias vim=vimx` and `alias vi=vimx` to your **.bashrc** or **.zshrc**. This is important because vim binary isn’t built with +clipboard support.

To use mouse set `set mouse=a` in your **.vimrc**
