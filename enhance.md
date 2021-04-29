*bat* (instead *cat*)
```
sudo apt install bat
mkdir -p ~/.local/bin
ln -s /usr/bin/batcat ~/.local/bin/bat
```

*lsd* (instead *ls*)
```
sudo dpkg -i https://github.com/Peltoche/lsd/releases/download/0.20.1/lsd_0.20.1_amd64.deb
```
replace ls with lsd
add to *~/.bashrc*
```
alias ls='/usr/bin/lsd'
alias l='ls -l'
alias la='ls -a'
alias lla='ls -la'
alias lt='ls --tree'
alias ll='la
```
