# NeoVim Config

A basic NeoVim config for working in C.

## Installation

### Pre Install

Prior to installation, you will most likely want to install a nerd font configure your terminal to use it. Nerd fonts can be found [here](https://www.nerdfonts.com/font-downloads).

### Linux

To install this config on a Linux distrobution, follow the following steps:

1. Install NeoVim, which can be done on x86_64 Ubuntu/Debian distros by running `sudo apt install neovim -y`
2. Install ripgrep to enable the live-grepping functionality using `sudo apt install ripgrep -y`
3. Create a folder `~/.config/nvim`
4. Clone this repository in `~/.config/nvim` 
    - `git clone https://github.com/EhlOps/NeovimConfig.git .`
5. Run `nvim`

### Mac

To install this config on MacOS, follow the following steps:

1. Install NeoVim, which for arm64 Macs can be done with `brew install neovim`
2. Install ripgrep to enable the live-grepping functionality using `brew install ripgrep`
3. Create a folder `~/.config/nvim`
4. Clone this repository in `~/.config/nvim`
    - `git clone https://github.com/EhlOps/NeovimConfig.git .`
5. Run `nvim`

**Note:** On MacOS, the default `terminal.app` does not support true colors. Please use iTerm2 or another terminal app to use the color theme.

### Windows

To install NeoVim for Windows, consult a guide on installation and setup. Clone this repository in your config folder, and you should be good to go. If you would like to install `ripgrep`, then click [here](https://github.com/BurntSushi/ripgrep?tab=readme-ov-file#installation).

### Post Install

After installing, it will be useful to install your LSPs, your linters, and your formatters. Enter NeoVim, then type `:Mason`. This will bring Mason's menu up, and you can install these tools. The tools that are already configured are the following:

- black
- clang-format
- clangd
- eslint_d
- isort
- lua-language-server
- prettier
- stylua

If you would like to install more LSPs, linters, or formatters, configure LSPs in `lua/plugins/lsp-config.lua` and everything else in `lua/plugins/none-ls.lua`. 

## Commands

Here is a list of the most valuable commands that are added from extensions. Note that the `<leader>` is set to `<space>` ("` `") by default, but it can be changed in `init.lua`. 

- `<C-n>`: Opens the NeoTree folder browser
    - `a`: Add a new file or foler
    - `H`: Show hidden files
    - `<enter>`: Open the selected file
- `<C-p>`: File search
- `<leader>fg`: Live `grep` through your work
- `K`: When hovering over a value/function in normal mode, press (capital) `K` to show the documentation for that value/function
- `gd`: When hovering over a value, press `gd` to go to its definition
- `<leader>ca`: When hovering over some sort of error, press `<leader>ca` to open a list of code actions to resolve the issue
- `<leader>gf`: Format a file using a formatter "LSP" from Mason
