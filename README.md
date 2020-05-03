# About ZSH
The Z shell (Zsh) is a Unix shell that can be used as an interactive login shell and as a command interpreter for shell scripting. Zsh is an extended Bourne shell with many improvements, including some features of Bash, ksh, and tcsh. (from christitustech with some improvements and fixes)

## Get Dependancies 
  - zsh-syntax-highlighting --> syntax highlighting for ZSH in standard repos
  - autojump --> jump to directories with j or jc for child or jo to open in file manager (available in the AUR)
  ![j](https://user-images.githubusercontent.com/45071921/76967237-0ced4380-691f-11ea-85a6-905271353e72.gif)
  - zsh-autosuggestions --> Suggestions based on your history
## Setup
Just copy and past each line in order, to your preferred terminal emulator :
```
wget https://github.com/Amirmohammadomidi/zsh/raw/master/.zshrc -O ~/.zshrc
mkdir -p "$HOME/.zsh" && mkdir -p "$HOME/.cache/zsh" && touch "$HOME/.cache/zsh/history"
wget https://github.com/Amirmohammadomidi/zsh/raw/master/.zsh/aliasrc -O ~/.zsh/aliasrc
```
## Theming
Execute this after finishing the setup process for theming to apply :
```
git clone https://github.com/sindresorhus/pure.git "$HOME/.zsh/pure"

```
![j](https://raw.githubusercontent.com/sindresorhus/pure/master/screenshot.png)
## To make ZSH your default shell 
Execute this command :
```
sudo sed 's/bash/zsh/g' /etc/passwd -i
```


