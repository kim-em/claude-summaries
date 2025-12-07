---
source_path: /Users/kim/.claude/skills/new-claude-sessions
generated: 2025-12-07T20:15:00Z
git_sha: cebfbc124ad636335256159ee28dd0fe48d30e73
git_branch: master
status: complete
files_count: 9
subdirs_count: 0
---

# new-claude-sessions

## Overview

A Claude Code skill that provides automation scripts to spawn new Claude Code sessions in various modes: background (fire-and-forget), interactive (iTerm2 tabs), and inspect (Cursor windows with file browsing). The skill includes a unified spawning script with machine-aware defaults, support for both local and SSH-remote Cursor sessions, git repository cloning with automatic Mathlib cache fetching, and AppleScript-based window automation. This enables parallel Claude workflows where one Claude instance can spawn additional sessions for concurrent tasks.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Skill definition with usage documentation for all spawning modes and examples |
| spawn-session.sh | Unified entry point script with --type flag (background/interactive/inspect), --repo cloning, --target overrides, and machine-aware behavior |
| machine-config.sh | Machine configuration mapping hostnames (carica, arguta, chonk, chonk2) to preferred targets and methods |
| spawn-iterm.sh | AppleScript automation to create iTerm2 tab, cd to workdir, and start Claude with prompt |
| spawn-cursor-local.sh | Launch local Cursor window, open workdir, start Claude Code via Cmd+@ |
| spawn-cursor-remote.sh | Launch Cursor connected to SSH remote, create remote directory, start Claude with longer timeouts (60s/120s) |
| wait-and-prompt-cursor.sh | Helper to poll for Cursor window readiness, focus window, close sidebars (Cmd+B/Cmd+Opt+B), start Claude, and type prompt from temp file |
| test | End-to-end test suite spawning background, iTerm, local Cursor, and remote Cursor sessions to verify file creation |

## Subdirectories

None.

## Search Tags

claude-code session-spawning parallel-workflows iterm2 cursor automation applescript ssh-remote machine-aware git-clone mathlib-cache background-tasks window-automation skill
