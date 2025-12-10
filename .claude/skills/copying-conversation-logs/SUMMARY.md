---
source_path: /Users/kim/.claude/skills/copying-conversation-logs
generated: 2025-12-11T12:00:00Z
git_sha: 5a5c7bc8574841a2870eff76b15c9a7bf9b3c3fa
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# copying-conversation-logs

## Overview

A skill for copying Claude Code conversation logs to a local directory. Explains the storage structure (`~/.claude/projects/` with path-to-dash naming convention), provides commands for finding the right directory for a given project path, and includes a bash loop pattern that copies main conversation files (UUID-named .jsonl files) while skipping agent subconversation files (`agent-*.jsonl`).

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Skill definition with directory naming conventions, copy commands, and filtering pattern to exclude agent logs |

## Subdirectories

This folder contains no subdirectories.

## Search Tags

conversation-logs copying archiving backup jsonl session-history project-directories claude-code local-storage uuid bash-scripting
