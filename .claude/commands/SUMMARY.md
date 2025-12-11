---
source_path: /Users/kim/.claude/commands
generated: 2025-12-11T21:15:00Z
git_sha: dce44eb24f9a4be3f1c6b36d3787cea1dab9f904
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# commands

## Overview

Custom slash commands for Claude Code that automate common workflows. These are markdown files that define prompts and instructions invoked via `/command-name` in Claude sessions. The commands here support a daily workflow: morning startup routine with PR/TODO review, self-reflection for continuous improvement of CLAUDE.md instructions, and weekly activity logging with TODO cleanup.

## Key Files

| File | Purpose |
|------|---------|
| coffee.md | Morning startup routine (`/coffee`): runs weekly log check, syncs repos, checks nightly-testing branch status with failure analysis, reviews open PRs needing attention, displays TODO list with PR verification, and suggests actionable items |
| reflect.md | Self-reflection command (`/reflect`): reviews the conversation to identify genuine struggles and proposes targeted additions to CLAUDE.md files when prompting gaps caused real problems |
| update-log.md | Weekly log generator (`/update-log`): archives completed TODOs to weekly logs in metacortex, cleans TODO.md, runs automatically when Friday passes since last log |

## Subdirectories

None.

## Search Tags

slash-commands custom-commands morning-routine coffee reflect update-log todo-management weekly-log pr-review nightly-testing workflow automation claude-code
