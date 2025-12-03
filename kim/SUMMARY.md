---
source_path: /Users/kim
generated: 2025-12-02T18:00:00Z
git_sha: 0b9c4ded524bc589e2fb661dc7e146a6200fde94
git_branch: master
status: preliminary
files_count: 21
subdirs_count: 9
---

# kim

## Overview

This is Kim Morrison's home directory, configured as a git repository to track dotfiles, shell configurations, scripts, and select project directories. The setup includes shell environment configurations (bash and zsh), version control configs (git and mercurial), and API credentials for services like Zulip. The directory uses git submodules for the `.claude` configuration and `metacortex` (a personal TODO and logging system). Historical TODO files from 2021 document early Lean 4 development work including mathport, mathlib4 tactics, and Gröbner basis implementations.

## Key Files

| File | Purpose |
|------|---------|
| `.zshrc` | Zsh shell configuration with PATH setup, API keys (OpenAI, Aristotle), opam, Docker, and Antigravity integration |
| `.bash_profile` | Bash startup configuration sourcing `.profile` and `.bashrc`, setting up autojump, elan (Lean toolchain manager), hub, and rbenv |
| `.zshenv` | Zsh environment setup adding Homebrew to PATH |
| `.gitconfig` | Git configuration with user identity (Kim Morrison), editor (nano), LFS filter, and custom hooks path |
| `.gitignore` | Comprehensive ignore patterns for build artifacts, caches, IDE files, media files, and various development tool directories |
| `.gitignore_global` | Global git ignore patterns |
| `.gitmodules` | Git submodule configuration for `.claude` and `metacortex` repositories |
| `.bashrc` | Bash runtime configuration |
| `.profile` | Generic shell profile |
| `.zprofile` | Zsh profile configuration |
| `.zuliprc` | Zulip API configuration for leanprover.zulipchat.com |
| `zuliprc` | Duplicate Zulip configuration file (appears to be a copy without the leading dot) |
| `.hgrc` | Mercurial version control configuration |
| `.hgignore_global` | Global Mercurial ignore patterns |
| `.msmtprc` | SMTP mail transfer agent configuration |
| `.gitflow_export` | Git flow workflow configuration |
| `.claude.json` | Claude configuration file (86KB, likely contains session state or preferences) |
| `20210819-lean-todo.md` | Historical TODO list from August 19, 2021 covering mathport, mathlib4 tactics, ring profiling, documentation, and Gröbner bases |
| `20210820-lean-todo.md` | Historical TODO list from August 20, 2021 |
| `20210824-lean-todo.md` | Historical TODO list from August 24, 2021 |
| `Zhiqiang.nb` | Mathematica notebook (1MB) |
| `gravity.nb` | Mathematica notebook (82KB) on gravity-related calculations |

## Subdirectories

- [x] `.aws/` - AWS CLI configuration and credentials (complete)
- [x] `.config/` - XDG configuration directory for various applications (complete)
- [x] `.ec2/` - AWS EC2 credentials and SSL certificates (complete)
- [x] `.gnupg/` - GnuPG configuration and keyrings (complete)
- [x] `.ssh/` - SSH configuration, keys, and known_hosts (complete)
- [~] `Documents/` - Personal documents including Lean TODOs, mathematical research notes, caving guides, and subdirectories for Arduino, CV, Housing, Jobs, Medical, Money, and Travel (preliminary)
- [ ] `Sites/` - Web-related projects or sites (pending)
- [ ] `bin/` - Custom scripts and executables (pending)
- [ ] `projects/` - Software development projects (pending)

## Submodules

| Directory | Repository | Commit | Description |
|-----------|------------|--------|-------------|
| `.claude/` | https://github.com/kim-em/.claude | 90e5fe2 | (No description available) |
| `metacortex/` | git@github.com:kim-em/metacortex.git | 8dfc88a | Personal TODO list and activity log system |

See also: [.claude summary](../.claude/SUMMARY.md)

## Search Tags

home-directory dotfiles shell-configuration zsh bash git version-control api-credentials lean-development mathematica environment-setup path-configuration submodules kim-morrison personal-workspace configuration-management
