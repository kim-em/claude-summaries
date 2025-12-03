---
source_path: /Users/kim/.claude/todos
generated: 2025-12-02T10:52:00Z
git_sha: 9cd355943c9ee394e789bd85f55b5b212d04f7a2
git_branch: master
status: complete
files_count: 2939
subdirs_count: 0
---

# todos

## Overview

Per-session todo list state storage for Claude Code sessions. Each file is named with a session/agent UUID and contains a JSON array of todo items with their status (pending/in_progress/completed). The vast majority (2931+ files) contain empty arrays representing completed sessions with no persisted todos. A small number contain active or archived todo lists from sessions where the TodoWrite tool was used to track multi-step tasks.

## Key Files

All 2939 files follow the same naming pattern: `<uuid>-agent-<uuid>.json` where the UUID identifies a specific Claude Code session. Each file contains a JSON array of todo objects with fields: `content` (task description), `status` (pending/in_progress/completed), and `activeForm` (present continuous description).

### Examples of Files with Content

| File | Purpose |
|------|---------|
| 7d2608b4-0bbd-47fd-b4b3-6b9d41e736cc-agent-*.json | Session proving properties for FiniteProbability.comp (2 tasks) |
| 205ee250-8df6-4dcb-85b6-71ec42ad9151-agent-*.json | Session minimizing a Lean grind tactic MWE (6 tasks) |
| 4aff9c66-b0fc-470a-b9ce-37b79ba88e7b-agent-*.json | Session with todo history (non-empty) |
| 97da7a2e-28c0-41e5-adf2-1e0ed74c23e2-agent-*.json | Session with todo history (non-empty) |
| 6c6d671e-dc20-48a4-895d-5afb9d483278-agent-*.json | Session with todo history (non-empty) |
| 9606477e-7e32-4f23-98b7-3dddbd246186-agent-*.json | Session with todo history (non-empty) |
| bef7d4a8-1f6d-49f3-a401-35bb4814de12-agent-*.json | Session with todo history (non-empty) |

Note: Only 8 files out of 2939 are larger than 2 bytes (empty array). The rest represent sessions where todos were either never used or all completed and cleared.

## Subdirectories

None - this is a leaf directory.

## Search Tags

claude-code todos task-tracking session-state json per-session-data todo-list workflow agent-state
