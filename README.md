# NeoVim Config

A basic NeoVim config for working in C.

## Installation

### Linux

To install this config on a Linux distrobution, follow the following steps:

1. Install NeoVim, which can be done on x86_64 Ubuntu/Debian distros by running `sudo apt install neovim -y`
2. Install ripgrep to enable the live-grepping functionality using `sudo apt install ripgrep -y`
3. Create a folder `~/.config/nvim`
4. Clone this repository in `~/.config/nvim`
5. Run `nvim`

### Mac

To install this config on a Linux distrobution, follow the following steps:

1. Install NeoVim, which for arm64 Macs can be done with `brew install neovim`
2. Install ripgrep to enable the live-grepping functionality using `brew install ripgrep`
3. Create a folder `~/.config/nvim`
4. Clone this repository in `~/.config/nvim`
5. Run `nvim`

### Windows

To install NeoVim for Windows, consult a guide on installation and setup. Clone this repository in your config folder, and you should be good to go. If you would like to install `ripgrep`, then click [here](https://github.com/BurntSushi/ripgrep?tab=readme-ov-file#installation).

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
