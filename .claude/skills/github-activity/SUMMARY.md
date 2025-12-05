---
source_path: /Users/kim/.claude/skills/github-activity
generated: 2025-12-05T08:15:00Z
git_sha: 0bf6eafaf937840c8768c7c5c7cb40a66bbee861
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# github-activity

## Overview

A Claude Code skill that monitors GitHub activity including notifications, comments, mentions, PR review requests, and assignments. Provides a shell script wrapper around the GitHub Notifications API with intelligent defaults (activity since last Friday) and flexible filtering options (date range, participation level, read/unread status). Automatically activates when users ask about GitHub notifications or activity. Uses GitHub CLI authentication for the kim-em account.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Skill definition with activation triggers and tool permissions (Bash, Read) |
| README.md | User documentation with examples, options, and output format |
| gh-activity | Executable bash script that fetches and displays GitHub notifications grouped by reason |

## Subdirectories

None.

## Search Tags

github notifications activity mentions review-requests comments api github-cli gh authentication notification-types mention author comment review_requested assign team_mention state_change subscribed filtering date-range participating unread shell-script bash jq curl
