# Dependencies

This vim setup uses [vim-plug](https://github.com/junegunn/vim-plug)

## To install

```sh
ln -s ~/your/directory/.vim ~/.vim
ln -s ~/your/directory/.vimrc ~/.vimrc

vim +PlugInstall +qall

# For Terraform Syntax
git clone https://github.com/hashivim/vim-terraform.git ~/.vim/pack/plugins/start/vim-terraform

# this command installs spicy code's entire dotfiles -- not just vim specific configuration
# cd bundle/ctrlp-cmatcher && ./install.sh && cd - 

# set up coc for auto complete
cd .vim/plugged/coc.nvim/
yarn install
```

## Per user config

To have your very own custom vimrc additions or custom gvimrc just create these files ala:

    touch ~/.vim/custom_vimrc
    touch ~/.vim/custom_gvimrc

Then, sprinkle to taste with your defaults, undoing my craziness, etc.  These files are ignored by git and enable fun for all.

## On first run

If you see errors, but this is just Vim complaining about not having the plugins it wants installed.   Simply run:

    :PlugInstall
