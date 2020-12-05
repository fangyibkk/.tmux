# .tmux
My tmux config

## Setup Guide
Shell profile makes tmux open by default. \
Add to your `.zshrc` or `.bash_profile`
```
if command -v tmux &> /dev/null && [ -n "$PS1" ] && [[ ! "$TERM" =~ screen ]] && [[ ! "$TERM" =~ tmux ]] && [ -z "$TMUX" ]; then
  exec tmux
fi
```

## Binding
Prefix are bind to `Ctrl+q`
| binding | action |
| ------- | ------ |
|`Alt + h` | move to left pane |
|`Alt + l` | move to right pane |
|`Alt + j` | move to below pane |
|`Alt + k` | move to above pane |
|`Alt + z` | Toggle maximize current pane |
|`Alt + '` | Vertical split |
|`Alt + ;` | Horizontal split |
|`Alt + e` | Show all pane |

Seeing all binding `tmux list-keys`

## Copy and paste
use `shift + middlemouse` to paste from primary
use `shift + ctrl + v` to paste from secondary

## Troubleshoot coloring
Not much to do when `xterm256` is on \
Set the gnome window color pallette instead.
