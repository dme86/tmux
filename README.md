# tmux

I usually don't require tmux as frequently, given that I primarily use [dwm on Linux](https://github.com/dme86/dwm) and intend to transition to [aerospace on macOS](https://github.com/dme86/aerospace). However, there are times when it's beneficial to be familiar with this great terminal multiplexer.

My design is simple so that it should work on every machine.

|Split Terminal  | Open Window List |
|--|--|
| ![enter image description here](https://i.imgur.com/SylZdWl.png) |![enter image description here](https://i.imgur.com/9i0i1Mx.png) |

On the left side, you can observe a split terminal (vertical) - on the right side, there's a list view of open windows for selection. At the bottom is my straightforward status bar, which can be customized according to your requirements.

If no tmux session is running, tmux will start without showing its status bar with my default setup. 

## Installation

I am using a plugin manager for tmux. On the first startup, you need to press `Ctrl/Strg + y` followed by `I` to initialize the plugin manager. Then press `Enter` to load all the plugins.

#### Keybindings

I tried out multiple keybinds, but I faced issues due to OS or [neovim](https://github.com/dme86/neovim) defaults. As a result, I'm now using tmux defaults (besides cycling tabs). You have to use a prefix first, like `Ctrl + y`, before pressing a command key:

| Key | Description |
|--|--|
|`Ctrl/Strg + c` & `c`|Open a new tmux tab at the bottom |
|`Shift + Ctrl` & `->`|Go to right tab with Arrow key |
|`Shift + Ctrl` & `<-`|Go to left tab with Arrow key |
|`Ctrl/Strg + c` & `PgUp/PgDown`|Scroll up / down|
|`Ctrl/Strg + c` & `,`|Rename tab. Hit `Enter` after typing new name |
|`Ctrl/Strg + c` & `&`|Close tab |
|`Ctrl/Strg + c` & `%`|Vertical split |
|`Ctrl/Strg + c` & `"`|Horizontal split |
|`Ctrl/Strg + ` & `Arrow Keys`|Move between splits |
|`Ctrl/Strg + c` & press & hold `opt` + Arrow Keys|Resize splits |
|`Ctrl/Strg + c` & `{`|Swap splits|
|`Ctrl/Strg + c` & `x`|Close pane/split |
|`Ctrl/Strg + c` & `z`|Maximize/Minimize pane |
|`Ctrl/Strg + c` & `;`|go to the ‘last’ (previously used) pane |
|`Ctrl/Strg + c` & `[`|Enter **copy** mode. Exit with `q` |
|`Ctrl/Strg + c` & `w`|List all windows|
|`Ctrl/Strg + c` & `p`|Open Scratchpad (current dir)|
|`Ctrl/Strg + c` & `d`|Hide Scratchpad|

> In copy mode you can navigate via vim keys `j`  `k` etc. You can select text (`Shift+v`) and copy it to clipboard by pressing `Enter`.
> Scrolling in copy mode works via PgUp/Dn
> Searching in copy mode via  `Shift+/`  (classic vim binds)
> `q` exits copy mode.


