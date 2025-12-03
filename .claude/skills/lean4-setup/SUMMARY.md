---
source_path: /Users/kim/.claude/skills/lean4-setup
generated: 2025-12-01T13:15:00Z
git_sha: b75fd51d2702e678b15ef7ce28cf6993a31edb62
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# lean4-setup

## Overview

Critical setup skill that must be invoked immediately after cloning the lean4 repository, even before building. Provides step-by-step instructions for configuring elan toolchains so that tests use the freshly built stage1 compiler and source building uses the stage0 compiler. Without this setup, tests may run against the wrong Lean version, causing confusing failures with inconsistent error messages.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Complete skill definition with elan toolchain setup instructions, build commands, testing workflow, and technical details about Lean's two-stage bootstrap process |

## Subdirectories

No subdirectories.

## Search Tags

lean4 elan toolchain setup bootstrap stage0 stage1 repository clone cmake build testing lean4-repository compiler version-management directory-override elan-override build-system
