---
source_path: /Users/kim/.claude
generated: 2026-01-24T23:30:00Z
git_sha: 028d0adcedbd2761d5cc0f11547d30984556ab29
git_branch: master
status: complete
files_count: 6
subdirs_count: 13
---

# .claude

## Overview

Claude Code user configuration directory, synchronized across machines via git. Contains global instructions (CLAUDE.md), custom slash commands, skills (reusable prompt libraries), per-project session history, and runtime data (debug logs, file history, plans, shell snapshots, telemetry). This enables consistent Claude Code behavior across multiple machines with shared preferences and accumulated context, while also storing operational state and caches.

## Key Files

| File | Purpose |
|------|---------|
| CLAUDE.md | Global instructions applied to all Claude sessions across all projects (~15KB of detailed guidance) |
| README.md | Documentation explaining the repository structure and sync workflow |
| settings.json | Claude Code settings: cleanup period (36500 days), permissions mode (bypassPermissions) |
| history.jsonl | Command/input history tracking |
| .gitignore | Excludes sensitive/machine-specific files: credentials, debug data, session caches, telemetry |
| test | Executable script to run all skill tests (unit tests and end-to-end activation tests) |

## Subdirectories

### Configuration & Extensions (4 directories)
- [x] `commands/` - Custom slash commands (reflect.md, coffee.md, update-log.md)
- [x] `skills/` - 21 custom skills with SKILL.md definitions and helper scripts (including zulip with FTS5 search and message sending, merge-conflict-helper with 10-step PR workflow, copying-conversation-logs)
- [x] `plugins/` - Plugin configuration with versioned plugin registries (v1/v2) and marketplaces subdirectory
- [x] `projects/` - Per-project session history and context (62 project directories)

### Runtime & State (9 directories)
- [x] `debug/` - Debug logs and diagnostic data
- [x] `file-history/` - File edit history and snapshots
- [x] `ide/` - IDE integration lock files tracking active Claude Code sessions
- [x] `plans/` - Plan mode artifacts and planning session data
- [x] `session-env/` - Session environment state (1348 session directories)
- [x] `shell-snapshots/` - Shell environment snapshots (3321 zsh state captures)
- [x] `statsig/` - Statsig feature flag cache
- [x] `telemetry/` - Telemetry data and usage tracking
- [x] `todos/` - Per-session todo list state (8684 JSON files)

## Search Tags

claude-code configuration dotfiles global-instructions skills commands plugins settings git-sync multi-machine preferences session-history history-jsonl
