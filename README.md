# NeoVim Config

A basic NeoVim config for working in C.

## Installation

### Linux

To install this config on a Linux distrobution, follow the following steps:

1. Install NeoVim, which can be done on Ubuntu/Debain distros by executing thie following:

```bash
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux-x86_64.tar.gz
sudo rm -rf /opt/nvim
sudo tar -C /opt -xzf nvim-linux-x86_64.tar.gz
```

2. Add NeoVim to your path by adding `export PATH="$PATH:/opt/nvim-linux-x86_64/bin"` to your `~/.bashrc`, `~/.zshrc`, or equivalent.
3. Install ripgrep to enable the live-grepping functionality using `sudo apt install ripgrep -y`
4. Create a folder `~/.config/nvim`
5. Clone this repository in `~/.config/nvim`
6. Run `nvim`

## Commands

Here is a list of the most valuable commands that are added from extensions. Note that the `<leader>` is set to `<space>` ("` `") by default, but it can be changed in `init.lua`. 

- `<C-n>`: Opens the NeoTree folder browser
    - `a`: Add a new file or foler
    - `H`: Show hidden files
    - `<enter>`: Open the selected file
- `<C-p>`: File search
- `<leader>fg`: Live `grep` through your work
- `K`: When hovering over a value/function in normal mode, press (capital) `K` to show the documentation for that value/function.
- `gd`: When hovering over a value, press `gd` to go to its definition.
- `<leader>ca`: When hovering over some sort of error, press `<leader>ca` to open a list of code actions to resolve the issue.
