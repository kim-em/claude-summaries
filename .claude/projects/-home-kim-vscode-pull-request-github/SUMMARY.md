---
source_path: /Users/kim/.claude/projects/-home-kim-vscode-pull-request-github
generated: 2025-12-11T20:30:00Z
git_sha: dce44eb24f9a4be3f1c6b36d3787cea1dab9f904
git_branch: master
status: complete
files_count: 7
subdirs_count: 0
---

# -home-kim-vscode-pull-request-github

## Overview

Session history for the VS Code GitHub Pull Requests extension on a remote server (`/home/kim/vscode-pull-request-github`). Contains 2 main sessions and 5 agent sessions investigating GitHub issue #7403 - a critical bug where the extension prevents `workspace.onDidCloseTextDocument` events from firing, causing document leaks that affect other extensions like Lean 4. Sessions document the investigation, root cause analysis, and proposed fixes for the document lifecycle problem.

## Key Files

| File | Purpose |
|------|---------|
| 6c0b5b6f-0a3d-4007-8875-47fd18bb0057.jsonl | Primary investigation session (170KB) - deep dive into issue #7403, identified root causes in prefetching and comment thread code |
| 1dc9f6e9-1f0b-4d4f-a525-aeca3a07eccf.jsonl | Secondary investigation session (59KB) - continuation of issue analysis |
| agent-992a64ba.jsonl | Major agent session (598KB) - comprehensive codebase analysis for document leak causes |
| agent-50da7589.jsonl | Agent session investigating document patterns |
| agent-c9f7dcdc.jsonl | Agent session for additional analysis |
| agent-f6803764.jsonl | Small agent session |
| agent-fa0acfcf.jsonl | Small agent session |

## Subdirectories

None.

## Search Tags

vscode-pull-request-github document-leak onDidCloseTextDocument issue-7403 remote-server prefetching comment-threads document-lifecycle memory-leak language-server lean4
