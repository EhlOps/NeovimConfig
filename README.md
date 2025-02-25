# NeoVim Config

A basic NeoVim config for working in C.

### Commands

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
