---
source_path: /Users/kim/.config/git
generated: 2025-12-01T18:35:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# git

## Overview

XDG-compliant Git configuration directory containing a global gitignore file. This follows the XDG Base Directory specification for Git configuration, placing shared ignore patterns in `~/.config/git/ignore` rather than the legacy `~/.gitignore` location. The configuration is tracked in the home directory git repo and shared across machines via the `~/bin/setup-machine` workflow.

## Key Files

| File | Purpose |
|------|---------|
| `ignore` | Global gitignore patterns - currently ignores `.claude/settings.local.json` files across all repositories to prevent committing machine-specific Claude Code settings |

## Subdirectories

*(No subdirectories)*

## Search Tags

git xdg-configuration global-gitignore dotfiles ignore-patterns claude-code machine-specific tracked-config
