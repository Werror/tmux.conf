# tmux config

## Installation

```bash
ln -sf ~/dotfiles/tmux.conf/.tmux.conf ~/.tmux.conf
```

## Features

- Mouse support
- Windows and panes indexed from 1
- 10000 line scrollback buffer
- No escape delay (nvim-friendly)
- Vi keys in copy mode
- OSC52 clipboard passthrough (for local terminal, omit on servers)
- `Ctrl+b r` — reload config
- `|` / `-` — split window horizontally / vertically

## Status Bar

- Left: `[hostname:session]`
- Right: `[pane index/total]  date  time`
- Current window shows active command in parentheses
- Random color theme per session (dark bg + vivid fg)

## Server variant

Use `.tmux.conf.server` on remote machines — same config minus the OSC52 clipboard passthrough and without the hostname in the session label.
