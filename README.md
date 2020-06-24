# About ZSH
The Z shell (Zsh) is a Unix shell that can be used as an interactive login shell and as a command interpreter for shell scripting. Zsh is an extended Bourne shell with many improvements, including some features of Bash, ksh, and tcsh. (from christitustech with some new features, improvements and fixes)
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
Execute this after you finished the setup process for theming to apply :
```
git clone https://github.com/sindresorhus/pure.git "$HOME/.zsh/pure"

```
![j](https://raw.githubusercontent.com/sindresorhus/pure/master/screenshot.png)
# Update 1 
### added feature
  - Auto complete with case insenstivity.
  - use vim keys or arrow keys to move between files and directories provided by tab suggestions.                                                          
### optional dependancies  
  - zsh-you-should-use --> reminds you of your existing aliases for a command you just typed.
  - find-the-command --> Advanced command-not-found hook for bash and zsh using the power of pacman.
### Note
  to use optional dependancies after updating via command below and installing them please uncomment line 54 and 55 in .zshrc file located in your home folder.
### How to update
Execute this command (dont worry your aliases will be untouched) : 
```
wget https://github.com/Amirmohammadomidi/zsh/raw/master/.zshrc -O ~/.zshrc
```
   
## To make ZSH your default shell 
Execute this command :
```
sudo sed 's/bash/zsh/g' /etc/passwd -i
```


