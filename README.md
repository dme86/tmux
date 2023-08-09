# tmux

I usually don't require tmux as frequently, given that I primarily use [dwm on Linux](https://github.com/dme86/dwm) and intend to transition to [yabai on macOS](https://github.com/koekeishiya/yabai). However, there are times when it's beneficial to be familiar with this great terminal multiplexer.

My design is simple so that it should work on every machine.

|Split Terminal  | Open Window List |
|--|--|
| ![enter image description here](https://i.imgur.com/SylZdWl.png) |![enter image description here](https://i.imgur.com/9i0i1Mx.png) |

On the left side, you can observe a split terminal (vertical) - on the right side, there's a list view of open windows for selection. At the bottom is my straightforward status bar, which can be customized according to your requirements.

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
|`Ctrl/Strg + b` & `w`|List all windows|
