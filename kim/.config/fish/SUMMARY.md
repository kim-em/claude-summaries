---
source_path: /Users/kim/.config/fish
generated: 2025-12-01T19:50:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 2
subdirs_count: 3
---

# fish

## Overview

Fish shell (Friendly Interactive SHell) configuration directory containing minimal setup. The main config.fish sets up Homebrew paths for interactive sessions. The fish_variables file stores universal variables including color scheme settings, keybindings, and pager colors using Fish's default theme. The configuration is very lightweight with empty subdirectories for completions, conf.d, and functions, suggesting a minimal customization approach that relies on Fish's built-in defaults.

## Key Files

| File | Purpose |
|------|---------|
| `config.fish` | Main fish shell configuration - sets Homebrew path (/opt/homebrew/bin) and defines interactive session setup |
| `fish_variables` | Fish universal variables storing color scheme (autosuggestions, command colors, error colors, etc.), default keybindings, and pager appearance settings |

## Subdirectories

- [x] `completions/` - Directory for custom tab-completion definitions (currently empty)
- [x] `conf.d/` - Configuration snippets directory for modular config files (currently empty)
- [x] `functions/` - Custom fish functions directory (currently empty)

## Search Tags

fish-shell shell-configuration interactive-shell homebrew path-setup universal-variables color-scheme keybindings pager-config minimal-config xdg-config
