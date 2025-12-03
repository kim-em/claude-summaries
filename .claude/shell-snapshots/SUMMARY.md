---
source_path: /Users/kim/.claude/shell-snapshots
generated: 2025-12-01T23:41:06Z
git_sha: ebe831cc1718246ffc866d2d1603aea2fc46574a
git_branch: master
status: complete
files_count: 1066
subdirs_count: 0
---

# shell-snapshots

## Overview

Shell environment snapshots captured by Claude Code at session start. Each snapshot is a ~5KB executable shell script that preserves the complete zsh environment state: all functions (including completion system), shell options, aliases, and PATH. Files are named `snapshot-zsh-{timestamp}-{random-id}.sh` and can be sourced to restore a shell environment. Collection spans from November 20, 2025 to December 2, 2025, with 1066 snapshots total.

## Key Files

| File | Purpose |
|------|---------|
| snapshot-zsh-1764632453547-9pnv7p.sh | Most recent shell snapshot (Dec 2, 2025) - 213 lines capturing zsh environment |
| snapshot-zsh-1763620603951-duut0r.sh | Oldest snapshot (Nov 20, 2025) - marks beginning of snapshot collection |
| *(1064 other snapshots)* | Historical shell environment states captured during Claude Code sessions |

**Snapshot file structure:**
- Header: Comments and alias unset
- Functions: zsh completion system (compaudit, compdef, etc.) and user-defined functions
- Shell Options: setopt configurations (e.g., nohashdirs, login)
- Aliases: Command aliases including run-help, which-command, and rg fallback
- Environment: Exported PATH and other environment variables

**File size distribution:**
- 797 files at 5.1K (most common)
- 207 files at 5.3K
- 53 files at 5.2K
- 9 files at 5.0K

## Subdirectories

*(none)*

## Search Tags

shell-snapshots zsh environment-state session-snapshots functions completion aliases path claude-code runtime-state shell-environment restoration debugging
