---
source_path: /Users/kim/.claude/skills/zulip
generated: 2025-12-07T19:54:00Z
git_sha: 20e6afa48c1d819500c6288f237c3e6d3ff64b29
git_branch: master
status: complete
files_count: 10
subdirs_count: 0
---

# zulip

## Overview

A Claude Code skill providing read-only access to Zulip chat messages from leanprover.zulipchat.com (default) and lean-fro.zulipchat.com. The skill activates when users ask about Zulip messages or Lean Zulip discussions. It features a comprehensive set of Python and bash helper scripts for searching messages, retrieving stream/topic discussions, and filtering by sender. All scripts output JSON piped through format-messages.py, which strips HTML, displays relative timestamps ("2h ago", "yesterday"), and reduces token usage by 80-90%. Credentials stored in ~/metacortex/.credentials/zulip.json support multiple sites with a configurable default. The skill demonstrates excellent separation of concerns: separate scripts for different query types, a dedicated formatting layer, and support for both convenience scripts and direct API access via curl with Zulip's narrow filter operators.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Skill definition (name: zulip, allowed-tools: Bash/Read/Grep/Write) with complete documentation of helper scripts, API usage patterns, narrow filter operators, and credential JSON format. Includes examples for all query types and curl-based direct API access |
| format-messages.py | Core formatter (129 lines) converting Zulip API JSON to human-readable output. HTMLStripper class removes HTML tags, format_timestamp() produces relative times ("2m ago", "3h ago", "yesterday HH:MM", or ISO date), format_message() offers compact and verbose modes. Reduces token usage by extracting only sender, content, stream, topic, timestamp |
| search | Python script accepting term, optional count (default varies), and site parameter to search all messages across a Zulip instance. Outputs raw JSON for piping to formatter |
| my-search | Python script to search only the authenticated user's own messages, with same interface as search (term, count, site). Uses sender filter to restrict results |
| stream-topic | Python script to retrieve messages from a specific stream+topic combination. Takes stream name, topic name, optional count and site. Essential for focused discussions |
| my-messages | Bash script using curl to fetch the authenticated user's recent messages. Demonstrates direct API usage pattern with credential extraction via jq |
| my-messages-since | Bash script to get sent messages since a specific date (YYYY-MM-DD format). Filters for stream messages only (skips DMs) and outputs unique stream/topic combinations for identifying active discussions |
| stream-summary | Script to get recent messages from an entire stream (all topics). Takes stream name, optional count and site |
| test | End-to-end test script validating the Zulip integration functionality, likely testing credential loading, API calls, and formatter output |
| .gitignore | Excludes credentials.json from version control to prevent accidental credential exposure |

## Subdirectories

This folder contains no subdirectories.

## Search Tags

zulip chat messaging lean leanprover lean-fro api-client search stream topic python bash html-formatter json credentials authentication token-reduction
