---
source_path: /Users/kim/.claude/skills/github-prs
generated: 2025-12-07T19:53:00Z
git_sha: 20e6afa48c1d819500c6288f237c3e6d3ff64b29
git_branch: master
status: complete
files_count: 5
subdirs_count: 0
---

# github-prs

## Overview

A Claude Code skill for monitoring GitHub pull requests with two complementary tools: `gh-prs` for tracking opened/merged PRs over time, and `gh-prs-attention` for identifying PRs that need immediate action. The skill defaults to showing activity since last Friday midnight and uses GitHub CLI (`gh`) for authentication. It intelligently filters for PRs needing attention by checking labels (awaiting-author, merge-conflict, awaiting-CI) and CI check status, while automatically excluding experimental/WIP PRs unless they have critical issues.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Skill definition with frontmatter (name, description, allowed-tools) and comprehensive usage documentation |
| README.md | User-facing documentation with quick start guide, features overview, and examples |
| gh-prs | Bash script to list opened/merged PRs with flexible date filtering (defaults to last Friday) |
| gh-prs-attention | Bash script to identify PRs needing attention based on labels and CI status |
| test | Test suite validating both scripts work correctly with GitHub CLI |

## Subdirectories

This folder contains no subdirectories.

## Search Tags

github pull-requests pr-monitoring ci-checks merge-conflicts code-review github-cli gh automation attention-tracking weekly-summary opened-prs merged-prs draft-prs experimental-prs wip bash-script claude-skill
