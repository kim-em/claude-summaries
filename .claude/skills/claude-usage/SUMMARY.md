---
source_path: /Users/kim/.claude/skills/claude-usage
generated: 2026-02-01T14:00:00Z
git_sha: 5ab0a683024feca845347c2f155eaf4d2e8ceb52
git_branch: master
status: complete
files_count: 7
subdirs_count: 0
---

# claude-usage

## Overview

A Claude Code skill for quota-aware Claude automation, providing query and shell control flow interfaces. The skill checks Claude Max subscription usage across three quotas (session, weekly all-models, weekly Sonnet-only) and returns structured data or model availability decisions. Includes bash scripts for shell automation and intelligent model selection that falls back from Opus to Sonnet based on quota health. Enhanced with fixed reset time parsing to handle same-day time-only resets correctly.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Skill definition with activation triggers, usage examples for all interfaces (JSON query, model selection), and detailed output format documentation |
| claude-usage | Core bash script using expect to spawn Claude session, capture /usage TUI output, parse and strip ANSI codes, calculate time-elapsed percentages with fixed same-day reset handling, output structured JSON |
| claude-available-model | Smart model selector that returns "opus" if session+weekly quotas excellent, "sonnet" if Sonnet quota excellent, exit 1 if no quota; supports --verbose for status display |
| claude-usage-ok | Legacy silent wrapper (exit 0 only if session+weekly excellent); deprecated in favor of claude-available-model for new scripts |
| test | Comprehensive test suite validating JSON schema, field ranges (0-99% for time_elapsed, enforcing future reset times), timeout handling with gtimeout fallback, and end-to-end skill activation |
| .gitignore | Git ignore file excluding the cache file from version control |
| .claude-usage-cache | JSON cache file storing recent quota query results (session, weekly all-models, weekly Sonnet-only usage percentages and reset times) |

## Subdirectories

None.

## Search Tags

claude-usage quota subscription limits reset pacing session weekly expect tui parsing json bash skill automation rate-limiting model-selection opus sonnet fallback
