---
source_path: /Users/kim/.claude/ide
generated: 2025-12-02T10:30:00Z
git_sha: ebe831cc1718246ffc866d2d1603aea2fc46574a
git_branch: master
status: complete
files_count: 8
subdirs_count: 0
---

# ide

## Overview

IDE integration lock files that track active Claude Code sessions. Each file is named by process ID (PID) and contains JSON metadata about the running session, including workspace folders, IDE name (Cursor), transport protocol (WebSocket), and authentication token. These lock files allow Claude Code to manage concurrent sessions and prevent conflicts between multiple running instances.

## Key Files

| File | Purpose |
|------|---------|
| 29115.lock | Session lock for PID 91609 in workspace `/Users/kim/projects/lean/mathlib4-2` |
| 42014.lock | Session lock for PID 91609 in workspace `/tmp/mathlib4-31926` |
| 17884.lock | Session lock file for another active Claude Code instance |
| 40938.lock | Session lock file for another active Claude Code instance |
| 42717.lock | Session lock file for another active Claude Code instance |
| 44998.lock | Session lock file for another active Claude Code instance |
| 54988.lock | Session lock file for another active Claude Code instance |
| 65245.lock | Session lock file for another active Claude Code instance |

## Subdirectories

None.

## Search Tags

ide integration lock-files session-management process-tracking cursor websocket authentication concurrency
