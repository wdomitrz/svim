# svim
Simple script to mimic Visual Studio Code Remote - SSH in vim.

## Usage
```shell
svim [user@]host:[dir]
```

## Installation

### For current user
Put `svim` in `~/.local/bin/`.
```shell
mkdir -p ~/.local/bin
git clone https://github.com/wdomitrz/svim
cd svim
cp svim ~/.local/bin/
```

### Globally (for every user)
Put `svim` in `/usr/bin/`.
```shell
git clone https://github.com/wdomitrz/svim
cd svim
sudo cp svim ~/.local/bin/
```

## Functionality
Edit code on remote server locally using exactly one command.

### Remote terminal
For better terminal integration use [vim-terminal-help](https://github.com/skywind3000/vim-terminal-help).
Every terminal opened with help this plugin will connect through `ssh` to the remote server automatically.

#### Installation
Follow instructions from [vim-terminal-help](https://github.com/skywind3000/vim-terminal-help).

### Plugins
All plugins available locally for `vim` are also available for `svim`. That includes language servers installed locally.

## Not implemented
Using plugins on remote system.

## Possible problems
Libraries and packages installed remotely will not be detected by your local plugins and language servers.
