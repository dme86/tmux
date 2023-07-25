# tmux

[tmux](https://github.com/tmux/tmux) is a terminal multiplexer. It lets you switch easily between several programs in one terminal, detach them (they keep running in the background) and reattach them to a different terminal.

![enter image description here](https://i.imgur.com/IW1Xxbd.png)

## install

### Arch 

    pacman -S tmux


**Clone or copy tmux.conf from this repo**

    git clone https://github.com/dme86/tmux.git


**Execute tmux**

    tmux

#### Keybindings

I tried out multiple keybinds, but I faced issues due to OS or [neovim](https://github.com/dme86/neovim) defaults. As a result, I'm now using tmux defaults. You have to use a prefix first, like `Ctrl + b`, before pressing a command key:

| Key | Description |
|--|--|
|`Ctrl/Strg + b` & `c`|Open a new tmux tab at the bottom |
|`Ctrl/Strg + b` & `n`|Go to the `n`ext tab |
|`Ctrl/Strg + b` & `n`|Go to the `p`revious tab |
|`Ctrl/Strg + b` & `%`|Vertical split |
|`Ctrl/Strg + b` & `"`|Horizontal split |
|`Ctrl/Strg + b` & `x`|Close pane |
|`Ctrl/Strg + b` & `;`|go to the ‘last’ (previously used) pane |
|`Ctrl/Strg + b` & `w`|List windows|
