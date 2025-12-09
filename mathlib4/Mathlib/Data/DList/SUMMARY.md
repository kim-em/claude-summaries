---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/DList
generated: 2025-12-09T00:00:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 1
subdirs_count: 0
---

# DList

## Overview

The `DList/` directory provides Mathlib-specific instances and theorems for difference lists (`DList`), a data structure optimized for efficient list concatenation. Difference lists are implemented in Batteries, and this module extends them with a `Traversable` instance by establishing an equivalence with regular lists. This allows DLists to be used in generic traversable contexts while maintaining their performance characteristics for concatenation-heavy operations.

## Key Files

| File | Purpose |
|------|---------|
| Instances.lean | Defines the equivalence between `List α` and `DList α`, and provides `Traversable`, `LawfulTraversable`, and `Inhabited` instances for `DList` |

## Subdirectories

None.

## Search Tags

difference-lists dlist list-concatenation traversable batteries data-structures functional-programming performance-optimization
