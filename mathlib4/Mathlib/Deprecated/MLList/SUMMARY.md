---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Deprecated/MLList
generated: 2025-01-24T11:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# MLList

## Overview

The `MLList/` folder contains deprecated lazy list search algorithms, specifically a best-first search implementation for tree and graph traversal. The search uses `MLList` (lazy lists from Batteries) with a priority queue that lazily refines priority estimates rather than computing exact priorities upfront. This design was created for the `rw_search` tactic where priorities were expensive edit distance computations; only the frontmost queue element's priority gets refined to full accuracy. The entire module was deprecated on 2025-09-11 when `rw_search` was removed from Mathlib.

## Key Files

| File | Purpose |
|------|---------|
| BestFirst.lean | Implements `BestFirstQueue` (priority queue with lazy estimation), `BestFirstNode` (queue nodes with estimator-based bounds), and `bestFirstSearch`/`bestFirstSearchCore` (graph search with configurable max depth, beam width via `maxQueued`, and duplicate detection via `RBSet`); depends on `Mathlib.Deprecated.Estimator` for the `Estimator` typeclass that provides improvable lower bounds |

## Subdirectories

*(none)*

## Search Tags

deprecated mllist lazy-list best-first-search priority-queue estimator beam-search graph-search tree-traversal rw_search tactic removed edit-distance thunk
