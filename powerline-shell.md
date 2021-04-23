### Install

Based on * https://github.com/b-ryan/powerline-shellx *

```
pip install powerline-shell
```


*add the following to the ~/.bashrc file
```
function _update_ps1() {
    PS1=$(powerline-shell $?)
}

if [[ $TERM != linux && ! $PROMPT_COMMAND =~ _update_ps1 ]]; then
    PROMPT_COMMAND="_update_ps1; $PROMPT_COMMAND"
fi
```

```
source ~/.bashrc
```

### Install fonts
```
sudo apt-get install fonts-powerline
~/.config/fontconfig/conf.d
fc-cache -vf
```

### Create config file
```
mkdir -p ~/.config/powerline-shell && \
powerline-shell --generate-config > ~/.config/powerline-shell/config.json
```
*Update config file*
```
{
  "segments": [
    "virtual_env",
    "ssh",
    "cwd",
    "git",
    "git_stash",
    "jobs",
    "set_term_title",
    "svn",
    "newline",
    "root"
  ],
  "mode": "flat",
  "cwd": {
    "mode": "plain",
    "max_depth": 2
  },
  "theme": "gruvbox"
}
```
