# ZSH
My ZSH Config (from christitustech with some improvements and fixes)

## Get Dependancies 
  - zsh-syntax-highlighting --> syntax highlighting for ZSH in standard repos
  - autojump --> jump to directories with j or jc for child or jo to open in file manager (available in AUR)
  - zsh-autosuggestions --> Suggestions based on your history
## Setup
```
wget https://github.com/ChrisTitusTech/zsh/raw/master/.zshrc -O ~/.zshrc
mkdir -p "$HOME/.zsh"
mkdir -p "$HOME/.cache/zsh" && touch "$HOME/.cache/zsh/history"
wget https://github.com/ChrisTitusTech/zsh/raw/master/.zsh/aliasrc -O ~/.zsh/aliasrc
git clone https://github.com/sindresorhus/pure.git "$HOME/.zsh/pure"
```
## To set aliases: 
```
nano /bin/zsh/aliaserc
```

## To make ZSH your default shell: 
  - simply change /bin/zsh in /etc/passwd to /bin/bash

