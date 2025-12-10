---
source_path: /Users/kim/.claude/skills/zulip
generated: 2025-12-11T12:00:00Z
git_sha: 5a5c7bc8574841a2870eff76b15c9a7bf9b3c3fa
git_branch: master
status: complete
files_count: 11
subdirs_count: 0
---

# zulip

## Overview

A Claude Code skill for interacting with Zulip chat on leanprover.zulipchat.com (default) and lean-fro.zulipchat.com. Supports both reading and sending messages. The skill activates when users ask about Zulip messages, Lean Zulip discussions, or want to search Zulip channels - and should be used PROACTIVELY when discussing Lean/Mathlib topics where Zulip context might help. The primary search method is now `zulip-client search` with FTS5 full-text search across message content and AI-generated summaries, returning complete threads with context. Helper scripts handle URL-based message fetching, stream/topic browsing, and user's own message queries. All scripts can pipe through format-messages.py which strips HTML, displays relative timestamps, and reduces token usage by 80-90%. Credentials stored in ~/metacortex/.credentials/zulip.json support multiple sites with a configurable default.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Skill definition (name: zulip, allowed-tools: Bash/Read/Grep/Write) with complete documentation including FTS5 search via zulip-client as primary method, helper scripts for URL fetching, stream browsing, personal messages, direct API access via curl with narrow filters, and message sending capabilities |
| format-messages.py | Core formatter converting Zulip API JSON to human-readable output with HTMLStripper class, relative timestamps ("2m ago", "3h ago", "yesterday HH:MM"), compact and verbose modes. Reduces token usage by extracting only essential fields |
| fetch-url | Bash script to fetch messages from Zulip URLs by extracting message ID from /near/XXXXXX pattern. Takes URL and optional context window (default 5 before, 10 after) |
| send-message | Bash script to post messages to Zulip streams. Takes stream, topic, and message (or - to read from stdin). Supports heredocs for multi-line messages with markdown and @mentions |
| search | Python script for searching all messages across a Zulip instance with term, count, and site parameters |
| my-search | Python script to search only the authenticated user's own messages using sender filter |
| stream-topic | Python script to retrieve messages from a specific stream+topic combination |
| my-messages | Bash script to fetch the authenticated user's recent messages via direct API |
| my-messages-since | Bash script to get sent messages since a specific date (YYYY-MM-DD), filtering for stream messages only with unique stream/topic output |
| stream-summary | Script to get recent messages from an entire stream (all topics) |
| test | End-to-end test script validating Zulip integration functionality |
| .gitignore | Excludes credentials.json from version control |

## Subdirectories

This folder contains no subdirectories.

## Search Tags

zulip chat messaging lean leanprover lean-fro api-client search fts5 full-text-search stream topic python bash send-message html-formatter json credentials authentication token-reduction
