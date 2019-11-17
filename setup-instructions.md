This information is taken from the following git-repositories:

* https://github.com/tmacwill/vimrc
* https://github.com/edkolev/promptline.vim

### Step-1
```
sudo apt-get install vim-nox
sudo apt-get install ruby ruby-dev
mkdir ~/.vim
git clone git://github.com/tmacwill/vimrc.git ~/.vim
git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim
ln -s ~/.vim/.vimrc ~/.vimrc
```
*Before continuing, replace the `.vimrc` with the `.vimrc` in this very repository*  

### Step-2
```
vim +BundleInstall +qall
cd ~/.vim/bundle/Command-T/ruby/command-t/ext/command-t
ruby extconf.rb
make
```

### Step-3

*Setup the bash prompt*

- open vim
- type the following
  ```
     esc
    :PromptlineSnapshot ~/.promptline.sh lightline
  ```
- In bash, type
  ```
    source ~/.promptline.sh
  ```
  

