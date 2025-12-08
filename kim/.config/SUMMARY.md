---
source_path: /Users/kim/.config
generated: 2025-12-01T20:00:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 1
subdirs_count: 4
---

# .config

## Overview

XDG Base Directory compliant configuration directory containing tracked application configs managed through the home directory git repo. This directory implements a minimal but effective approach to cross-machine configuration management: four subdirectories cover shell (Fish), version control (Git global ignore), GitHub CLI, and editor keybindings. The configurations are either used directly by XDG-aware applications (Fish, Git) or symlinked to traditional config locations (VSCode family editors) via the `~/bin/setup-machine` script. The approach emphasizes security by tracking only non-sensitive configs—authentication tokens like `gh/hosts.yml` are gitignored. The Fish configuration is notably minimal, relying on Fish's excellent built-in defaults with only Homebrew path setup. The Git config provides a single essential service: ignoring `.claude/settings.local.json` across all repositories. The GitHub CLI config uses HTTPS for git operations and defines a `co` alias for checking out PRs. The VSCode keybindings provide Claude Code integration across multiple editors (VSCode, Cursor, Antigravity).

## Key Files

| File | Purpose |
|------|---------|
| `README.md` | Documentation for the tracked config system, setup instructions, and list of currently managed configurations |

## Subdirectories

- [x] `fish/` - Fish shell configuration with minimal setup relying on built-in defaults, Homebrew path configuration, and universal variables
- [x] `gh/` - GitHub CLI configuration with HTTPS git protocol preference and command aliases
- [x] `git/` - XDG-compliant global gitignore for machine-specific files
- [x] `vscode/` - Shared keybindings for Claude Code integration across VSCode family editors

## Search Tags

xdg-configuration dotfiles application-configs fish-shell github-cli git vscode keybindings symlinks machine-setup configuration-management tracked-configs minimal-config homebrew claude-code editor-integration oauth git-ignore cross-machine https-git-protocol
