*bat* (instead *cat*)
```
sudo apt install bat
mkdir -p ~/.local/bin
ln -s /usr/bin/batcat ~/.local/bin/bat
```

*lsd* (instead *ls*)
```
snap install lsd
```
replace ls with lsd
add to *~/.bashrc*
```
alias ls='lsd'
alias l='ls -l'
alias la='ls -a'
alias lla='ls -la'
alias lt='ls --tree'
```
