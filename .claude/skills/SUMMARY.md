---
source_path: /Users/kim/.claude/skills
generated: 2025-12-05T01:17:34Z
git_sha: 89c460152720d80c143ce200122a66beb6d858d9
git_branch: master
status: complete
files_count: 0
subdirs_count: 17
---

# skills

## Overview

A comprehensive collection of 17 custom Claude Code skills that significantly extend Claude's capabilities across five major domains: Lean4/Mathlib development, GitHub integration, session management, communication platforms, and personal productivity. Each skill combines a SKILL.md definition (with activation triggers and tool permissions) with specialized helper scripts, providing both declarative knowledge and executable automation.

The skills demonstrate sophisticated design patterns: expect-based TUI automation (claude-usage), two-phase workflow documentation (lean4-bootstrap), API response optimization (github-api-large-responses), style codification from corpus analysis (kim-writing-style), and systematic reduction methodologies (lean-mwe). The collection includes both simple single-file skills (mathlib-build, folder-summary) and complex multi-script systems (zulip with 10 files, new-claude-sessions with 9 files), showing the skill framework's flexibility from quick configuration flags to full automation stacks.

## Key Files

This directory contains no files at the top level; all content is organized into subdirectories, one per skill.

## Subdirectories

### Lean4 & Mathlib Development (6 skills)
- [x] `lean4-setup/` - Critical post-clone setup configuring elan toolchains for stage0/stage1 bootstrap (1 file)
- [x] `lean4-bootstrap/` - Two-PR workflow for changes requiring update-stage0 (environment extensions, .olean format) (1 file)
- [x] `mathlib-build/` - Quiet mode build flags (`-q --log-level=info`) to suppress per-file progress in large projects (1 file)
- [x] `lean-mwe/` - Systematic 500-line error minimization methodology: guard-first discipline, proof irrelevance exploitation, progressive sorry-ification, attribute removal strategies, structure simplification, universe polymorphism replacement, with test cases and validated examples (3 files)
- [x] `merge-conflict-helper/` - 9-step workflow for auto-resolving PR merge conflicts (imports, versions, sequential additions) (1 file)
- [x] `folder-summary/` - References claude-summary tooling for two-phase directory indexing (1 file)

### GitHub Integration (3 skills)
- [x] `github-activity/` - Fetch notifications/mentions via API with intelligent defaults (since last Friday) (3 files)
- [x] `github-prs/` - Track opened/merged PRs and identify PRs needing attention via labels/CI status (5 files)
- [x] `github-api-large-responses/` - `jq` filtering patterns to prevent response truncation (1 file)

### Session & Workflow Management (2 skills)
- [x] `new-claude-sessions/` - Spawn parallel Claude sessions (background, iTerm2, local/remote Cursor) with git cloning and machine-aware defaults (9 files)
- [x] `claude-usage/` - Expect-based TUI automation to check subscription quotas with pacing indicators (6 files)

### Communication Platforms (2 skills)
- [x] `zulip/` - Read-only Zulip access with HTML stripping and 80-90% token reduction via custom formatter (10 files)
- [x] `whatsapp/` - Send-only WhatsApp messaging via Baileys library with QR authentication (8 files)

### Personal Productivity (3 skills)
- [x] `todo/` - Manage ~/metacortex/TODO.md with emoji status and linked notes (1 file)
- [x] `log/` - Daily activity logs in ~/metacortex/logs/ (YYYY-MM/DD.md format) (1 file)
- [x] `kim-writing-style/` - Writing style guide derived from 3,000+ Zulip messages (1 file)

### Web Automation (1 skill)
- [x] `browser-automation/` - Playwright MCP fallback for JavaScript-heavy sites with Chrome profile reuse (3 files)

## Search Tags

skills claude-code automation lean4 mathlib github zulip whatsapp session-management todo-list activity-logs browser-automation mwe minimal-working-example bootstrapping merge-conflicts iterm2 cursor writing-style pr-monitoring playwright puppeteer mcp web-scraping javascript spa chrome-profile authentication headless quota subscription limits reset pacing expect tui parsing json bash folder-summary summarization indexing catalog directory-tree two-phase preliminary final notifications mentions review-requests api jq filtering pagination elan toolchain stage0 stage1 update-stage0 environment-extensions olean-format compiler build-flags verbosity lake quiet diagnostics errors warnings technical-communication pr-descriptions documentation announcements hedging collaborative-language progressive-disclosure guard_msgs tactic-failures kernel-errors grind compiler-panics reduction backtracking git-merge conflict-analysis auto-resolution import-conflicts version-conflicts build-verification spawning parallel-workflows applescript ssh-remote machine-aware git-clone mathlib-cache window-automation task-management metacortex notes linked-notes emoji-status git-sync planning-sessions priorities due-dates baileys qr-code nodejs esm unofficial send-message phone-number chat messaging leanprover lean-fro api-client search stream topic html-formatter credentials token-reduction forum-scraping network-interception auto-wait locator-api
