---
source_path: /Users/kim/.claude/skills/lean4-bootstrap
generated: 2025-12-01T13:30:00Z
git_sha: b75fd51d2702e678b15ef7ce28cf6993a31edb62
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# lean4-bootstrap

## Overview

A Claude Code skill that provides comprehensive guidance for handling Lean4 bootstrapping changes that require `update-stage0`. This skill activates when making changes to environment extensions, .olean format, interpreter behavior, or ParserDescr constructors—any change where stage0 (pre-built compiler) needs updating to understand stage1's new format. It implements a documented two-PR workflow to handle the bootstrapping cycle safely, including test adjustments, CI trigger mechanisms, and local development procedures.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Complete bootstrapping workflow documentation covering the two-PR pattern, local development, rebasing with stage0 updates, and splitting existing PRs |

## Subdirectories

This directory contains no subdirectories.

## Search Tags

lean4 bootstrapping update-stage0 stage0 stage1 compiler two-pr-workflow environment-extensions olean-format interpreter ci-automation stdlib_flags.h rebase-stage0 bootstrap-transition test-adjustment cherry-pick pr-splitting
