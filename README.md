# tmux

I usually don't require tmux as frequently, given that I primarily use [dwm on Linux](https://github.com/dme86/dwm) and intend to transition to [aerospace on macOS](https://github.com/dme86/aerospace). However, there are times when it's beneficial to be familiar with this great terminal multiplexer.

My design is simple so that it should work on every machine.

|Split Terminal  | Open Window List |
|--|--|
| ![enter image description here](https://i.imgur.com/SylZdWl.png) |![enter image description here](https://i.imgur.com/9i0i1Mx.png) |

On the left side, you can observe a split terminal (vertical) - on the right side, there's a list view of open windows for selection. At the bottom is my straightforward status bar, which can be customized according to your requirements.

If no tmux session is running, tmux will start without showing its status bar with my default setup. You can always show/hide it via `Ctrl/Strg + b` & `&`.

#### Keybindings

I tried out multiple keybinds, but I faced issues due to OS or [neovim](https://github.com/dme86/neovim) defaults. As a result, I'm now using tmux defaults (besides cycling tabs). You have to use a prefix first, like `Ctrl + b`, before pressing a command key:

| Key | Description |
|--|--|
|`Ctrl/Strg + b` & `&`|Show / Hide statusbar at the bottom |
|`Ctrl/Strg + b` & `c`|Open a new tmux tab at the bottom |
|`Shift + Ctrl` & `->`|Go to right tab with Arrow key |
|`Shift + Ctrl` & `<-`|Go to left tab with Arrow key |
|`Ctrl/Strg + b` & `PgUp/PgDown`|Scroll up / down|
|`Ctrl/Strg + b` & `,`|Rename tab. Hit `Enter` after typing new name |
|`Ctrl/Strg + b` & `%`|Vertical split |
|`Ctrl/Strg + b` & `"`|Horizontal split |
|`Ctrl/Strg + b` & `Arrow Keys`|Move between splits |
|`Ctrl/Strg + b` & `x`|Close pane |
|`Ctrl/Strg + b` & `z`|Maximize/Minimize pane |
|`Ctrl/Strg + b` & `;`|go to the ‘last’ (previously used) pane |
|`Ctrl/Strg + b` & `[`|Enter **copy** mode. Exit with `q` |
|`Ctrl/Strg + b` & `w`|List all windows|

> In copy mode you can navigate via vim keys `j`  `k` etc. You can select text (`Shift+v`) and copy it to clipboard by pressing `Enter`.
> Scrolling in copy mode works via PgUp/Dn
> Searching in copy mode via  `Shift+/`  (classic vim binds)
> `q` exits copy mode.
