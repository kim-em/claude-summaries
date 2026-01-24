---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Lean/Elab
generated: 2026-01-24T23:50:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 1
---

# Elab

## Overview

The `Mathlib/Lean/Elab/` directory provides elaboration-related utilities that extend Lean 4's elaboration infrastructure. At the top level, it contains helper functions for working with info trees (the data structure that stores elaboration information for IDE support) and term elaboration (pattern elaboration, fresh level parameters). The `Tactic/` subdirectory extends this with utilities for tactic goal management and tactic execution in MetaM contexts. Together, these tools support Mathlib's metaprogramming needs during the elaboration phase, including IDE integration (Try This suggestions, theorem extraction), custom elaboration strategies (pattern elaboration with typeclass failure tolerance), and seamless integration between tactic and meta-level programming.

## Key Files

| File | Purpose |
|------|---------|
| InfoTree.lean | InfoTree utilities: `collectTryThisSuggestions` (extract all Try This suggestions from info trees), `findSomeM?`/`findSome?` (search infotree with context merging), `onHighestNode?` (evaluate on outermost node with context), `getDeclsByBody` (find declarations with elaborated bodies), `getTheorems` (extract theorem declarations from infotree) |
| Term.lean | Term elaboration utilities: `elabPattern` (elaborate patterns with TC failure tolerance, no errToSorry), `mkFreshLevelName` (generate fresh level names avoiding conflicts), `mkFreshLevelParam` (create and register fresh universe level parameters) |

## Subdirectories

- [x] `Tactic/` - Tactic elaboration utilities

## Search Tags

lean4 elaboration infotree term-elaboration tactic-elaboration ide-support try-this suggestions context-info pattern-elaboration universe-levels metaprogramming mathlib-infrastructure
