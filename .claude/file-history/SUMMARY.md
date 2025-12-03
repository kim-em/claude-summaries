---
source_path: /Users/kim/.claude/file-history
generated: 2025-12-02T09:59:00Z
git_sha: ebe831cc1718246ffc866d2d1603aea2fc46574a
git_branch: master
status: complete
files_count: 0
subdirs_count: 117
---

# file-history

## Overview

Stores version snapshots of files edited during Claude Code sessions. Each session (identified by UUID) gets its own directory containing timestamped versions of files that were modified. Files are named with a hash identifier followed by `@v{N}` for version number. Contains approximately 1,193 snapshot files across 117 session directories, providing an edit history and rollback capability for Claude Code sessions.

## Key Files

No files directly in this directory - all content is in session subdirectories.

## Subdirectories

All 117 subdirectories are session-specific directories (UUID-named):

- Session directories store file version snapshots in format `{hash}@v{version}`
- Each session contains snapshots of files edited during that specific Claude Code session
- Example: `7c3b5ff7-104c-4d34-84eb-91dd0eac9b3f/eb5995632de139cd@v10` contains version 10 of a file
- Sessions are retained for the configured cleanup period (36,500 days per settings.json)
- Sessions vary from having just 2-3 snapshot files to over 40 files for longer editing sessions

### Session Directory Sample

- `0166b49b-c333-4632-94a6-577b30321af1/` - Session snapshots
- `04bf83c4-16e9-4a2a-86bd-a0f4648dd480/` - Session snapshots
- `0548bfa6-3bf5-4306-8ee9-f001ac15a39b/` - Session snapshots
- `0624288a-3249-4601-ae5c-c700d55a5009/` - Session snapshots
- `09648446-bf50-4200-974b-45a7c0bbdd69/` - Session snapshots
- `09f2de3c-db15-4f25-b82d-d0618f7d998c/` - Session snapshots
- `0d070469-1c75-4b58-a7fe-80b79aead7e2/` - Session snapshots
- `0f44e5f2-0d12-47a8-b123-7907ac7fb187/` - Session snapshots
- `0f4bc1b9-d3b1-4d30-802e-fb8e44bcdb29/` - Session snapshots (70 files)
- `113f3889-9997-4cfe-aa32-018f78a0cc70/` - Session snapshots

*(117 total UUID-named session directories - listing abbreviated for brevity)*

## Search Tags

file-history version-control snapshots edit-history rollback claude-code sessions backups file-versions
