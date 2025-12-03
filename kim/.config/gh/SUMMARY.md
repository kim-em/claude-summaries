---
source_path: /Users/kim/.config/gh
generated: 2025-12-01T19:45:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# gh

## Overview

GitHub CLI (gh) configuration directory containing settings for git protocol preferences, command aliases, and authentication. Uses HTTPS for git operations and defines a convenient `co` alias for checking out pull requests. The tracked `config.yml` contains non-sensitive preferences, while `hosts.yml` (gitignored) stores OAuth tokens for GitHub authentication.

## Key Files

| File | Purpose |
|------|---------|
| `config.yml` | Main configuration for GitHub CLI including git protocol (https), prompt settings, and aliases (co = pr checkout) |
| `hosts.yml` | OAuth authentication tokens for GitHub (gitignored, not tracked) |

## Subdirectories

None.

## Search Tags

github-cli gh git-protocol oauth aliases pull-requests configuration cli-tools git-https authentication
