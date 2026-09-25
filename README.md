# tmux

A clean, keyboard-first tmux setup with Catppuccin styling, persistent sessions, and TPM plugin management.

## Features

- `Ctrl-a` prefix with Vim-style pane navigation
- Mouse support and vi copy mode
- Catppuccin Mocha status bar
- Session persistence with tmux-resurrect and tmux-continuum
- Clipboard integration with tmux-yank
- Vim and tmux navigation with vim-tmux-navigator

## Install

### 1. Install TPM

```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

### 2. Install the configuration

From the repository root:

```bash
mkdir -p ~/.tmux
cp tmuxs/~/.tmux.conf ~/.tmux.conf
```

Start tmux:

```bash
tmux
```

Inside tmux, press `Ctrl-a` then `I` to install the configured plugins.

## Usage

| Key | Action |
| --- | --- |
| `Ctrl-a` | Prefix key |
| `Ctrl-a` `c` | New window in the current directory |
| `Ctrl-a` `|` | Split pane horizontally |
| `Ctrl-a` `-` | Split pane vertically |
| `Ctrl-a` `h` `j` `k` `l` | Move between panes |
| `Ctrl-a` `H` `J` `K` `L` | Resize the active pane |
| `Ctrl-a` `r` | Reload the configuration |
| `Ctrl-a` `[` | Enter vi copy mode |

## Updating

Update plugins from inside tmux with `Ctrl-a` then `U`.

The configuration is stored in [`tmuxs/~/.tmux.conf`](tmuxs/~/.tmux.conf). After editing it, reload tmux with:

```bash
tmux source-file ~/.tmux.conf
```

## Requirements

- tmux 3.2 or newer
- Git
- A terminal with true-color support