# Neovim, Tmux, Kitty MacOS Setup

## Homebrew

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile

brew install git zsh-autosuggestions zsh-syntax-highlighting eza zoxide tmux bash neovim ripgrep fd gcc

source ~/.zprofile
```

### Installing OMZ

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```


**Note: Now Copy the .zshrc file to your path**

## Kitty

- Download and install kitty from here : https://github.com/kovidgoyal/kitty/tags
- Install the desired fonts :   DankMonoNerdFont
- Copy all the config files to .config

## Tmux

- Install TPM using ```git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm```
- Delete the ~/.tmux.conf and make sure latest tmux.conf is in .config

```
tmux
then press ctrl + b and then I
this will install all the tmux plugins
```


## NeoVim using LazyVim

```
rm -rf ~/.config/nvim
and copy the nvim folder to .config

nvim
this will open and install all the plugins and setup neovim for you
```

