---
source_path: /Users/kim/.claude
generated: 2025-12-09T10:40:00Z
git_sha: d3c5486ba8cc6e05ec408002550fd039e067c322
git_branch: master
status: complete
files_count: 8
subdirs_count: 13
---

# .claude

## Overview

Claude Code user configuration directory, synchronized across machines via git. Contains global instructions (CLAUDE.md), custom slash commands, skills (reusable prompt libraries), per-project session history, and runtime data (debug logs, file history, plans, shell snapshots, telemetry). This enables consistent Claude Code behavior across multiple machines with shared preferences and accumulated context, while also storing operational state and caches.

## Key Files

| File | Purpose |
|------|---------|
| CLAUDE.md | Global instructions applied to all Claude sessions across all projects (~14KB of detailed guidance) |
| README.md | Documentation explaining the repository structure and sync workflow |
| settings.json | Claude Code settings: cleanup period (36500 days), permissions mode (bypassPermissions) |
| settings.local.json | Machine-specific settings overrides (not tracked in git) |
| .gitignore | Excludes sensitive/machine-specific files: credentials, debug data, session caches, telemetry |
| test | Executable script to run all skill tests (unit tests and end-to-end activation tests) |
| go | Quick launcher script |

## Subdirectories

### Configuration & Extensions (4 directories)
- [x] `commands/` - Custom slash commands (reflect.md, coffee.md, update-log.md)
- [x] `skills/` - 20 custom skills with SKILL.md definitions and helper scripts (new: aristotle for automated theorem proving, synchronizing-home-git-repo for home directory conflict resolution, acquiring-skills for skill creation workflow)
- [x] `plugins/` - Plugin configuration (currently empty repositories config)
- [x] `projects/` - Per-project session history and context (61 project directories, 5800+ total session files)

### Runtime & State (9 directories)
- [x] `debug/` - Debug logs and diagnostic data
- [x] `file-history/` - File edit history and snapshots
- [x] `ide/` - IDE integration lock files tracking active Claude Code sessions
- [x] `plans/` - Plan mode artifacts and planning session data
- [x] `session-env/` - Session environment state (389 empty session directories)
- [x] `shell-snapshots/` - Shell environment snapshots (1066 zsh state captures from Nov-Dec 2025)
- [x] `statsig/` - Statsig feature flag cache (50+ gates, 30+ experiments)
- [x] `telemetry/` - Telemetry data and usage tracking
- [x] `todos/` - Per-session todo list state (2939 JSON files, mostly empty arrays)

## Search Tags

claude-code configuration dotfiles global-instructions skills commands plugins settings git-sync multi-machine preferences session-history
