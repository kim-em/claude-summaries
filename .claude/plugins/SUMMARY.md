---
source_path: /Users/kim/.claude/plugins
generated: 2026-01-24T21:00:00Z
git_sha: a7f9d0e5692aa0d2ec137abd8f2601dccd0a21ec
git_branch: master
status: complete
files_count: 4
subdirs_count: 1
---

# plugins

## Overview

Plugin configuration directory for Claude Code. Contains configuration files for plugin management including versioned plugin registries (v1 and v2 formats) and marketplace registry. Currently no plugins are installed, but the official Anthropic plugin marketplace is configured and cloned locally. The marketplaces subdirectory contains the cloned claude-plugins-official repository from GitHub.

## Key Files

| File | Purpose |
|------|---------|
| config.json | Plugin configuration file with empty repositories object |
| installed_plugins.json | Version 2 format plugin registry (empty plugins object) |
| known_marketplaces.json | Registry of configured marketplaces; currently tracks claude-plugins-official from anthropics/claude-plugins-official on GitHub, installed to marketplaces/claude-plugins-official |

## Subdirectories

- [x] `marketplaces/` - Contains cloned plugin marketplace repositories; hosts claude-plugins-official

## Search Tags

plugins configuration claude-code plugin-management repositories installed-plugins v2 marketplaces anthropic official-marketplace
