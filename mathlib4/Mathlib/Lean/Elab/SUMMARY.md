---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Lean/Elab
generated: 2026-01-24T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 2
subdirs_count: 1
---

# Elab

## Overview

The `Mathlib/Lean/Elab/` directory provides elaboration-related utilities that extend Lean 4's elaboration infrastructure. It contains helper functions for working with info trees (the data structure that stores elaboration information for IDE support), term elaboration (pattern elaboration, fresh level parameters), and tactic elaboration. These tools support Mathlib's metaprogramming needs during the elaboration phase, including IDE integration, suggestion collection, and custom elaboration strategies.

## Key Files

| File | Purpose |
|------|---------|
| InfoTree.lean | InfoTree utilities: `collectTryThisSuggestions` (extract all Try This suggestions from info trees), `findSomeM?`/`findSome?` (search infotree with context merging), `onHighestNode?` (evaluate on outermost node with context), `getDeclsByBody` (find declarations with elaborated bodies), `getTheorems` (extract theorem declarations from infotree) |
| Term.lean | Term elaboration utilities: `elabPattern` (elaborate patterns with TC failure tolerance, no errToSorry), `mkFreshLevelName` (generate fresh level names avoiding conflicts), `mkFreshLevelParam` (create and register fresh universe level parameters) |

## Subdirectories

- [x] `Tactic/` - Tactic elaboration utilities

## Search Tags

lean4 elaboration infotree term-elaboration tactic-elaboration ide-support try-this suggestions context-info pattern-elaboration universe-levels metaprogramming mathlib-infrastructure
