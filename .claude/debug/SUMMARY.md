---
source_path: /Users/kim/.claude/debug
generated: 2025-12-01T13:46:18Z
git_sha: ebe831cc1718246ffc866d2d1603aea2fc46574a
git_branch: master
status: complete
files_count: 2424
subdirs_count: 0
---

# debug

## Overview

Debug logs from Claude Code session initialization, with one timestamped text file per session (identified by UUID filename). Each log captures the initialization sequence: LSP manager setup, plugin loading, skill discovery, git repository detection, ripgrep configuration, and shell snapshot creation. Files range from ~6KB to several hundred KB, with most being 9-13KB. These logs are useful for diagnosing startup issues and understanding Claude Code's initialization process across different project directories.

## Key Files

2,424 debug log files, each named with a UUID corresponding to a Claude Code session. Representative patterns include:

| File Pattern | Purpose |
|--------------|---------|
| `{uuid}.txt` | Session initialization debug log with timestamped entries showing LSP setup, plugin loading (typically 0 plugins), skill discovery (7-17 skills), git repository detection, and shell snapshot creation |

Sample file sizes show variety: most logs are 9-13KB (standard initialization), some 20-30KB (more verbose), and a few larger files up to 4MB (likely long-running sessions with extensive logging).

## Subdirectories

None - this is a leaf directory containing only log files.

## Search Tags

claude-code debug logs session-initialization diagnostics lsp-manager plugin-loading skill-discovery git-detection shell-snapshots troubleshooting startup-sequence
