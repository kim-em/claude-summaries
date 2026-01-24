---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Deprecated
generated: 2025-01-24T22:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 1
---

# Deprecated

## Overview

The `Deprecated/` folder serves as Mathlib's backward compatibility layer, containing definitions and theorems that have been superseded but are maintained during transition periods. The folder houses two categories of deprecated content: (1) standalone items like the `Estimator` typeclass for lazy bound computation and the `List.Sorted` alias for `List.Pairwise`, and (2) module shims that re-export imports for files that have been reorganized. The most substantial deprecated content relates to the removed `rw_search` tactic—both the `Estimator` typeclass (for computing improvable lower bounds on lazy `Thunk` values) and the `MLList/BestFirst.lean` search algorithm (priority queue with lazy estimate refinement) were purpose-built for that tactic's expensive edit-distance computations. All items carry explicit `@[deprecated]` attributes with dates and replacement guidance.

## Key Files

| File | Purpose |
|------|---------|
| Aliases.lean | Empty placeholder file for deprecated aliases no longer used in Mathlib; provides a dumping ground for aliases whose imports would otherwise be unnecessary |
| Estimator.lean | Deprecated typeclass framework for computing improvable lower bounds on lazy values; `Estimator a ε` provides iteratively refinable bounds for `a : Thunk α`, previously used by the removed `rw_search` tactic (deprecated 2025-09-11) |
| Order.lean | Deprecated module shim (deprecated 2025-09-02) that re-exports order-related tactics including `Tactic.Linter.DeprecatedModule`, `Tactic.Basic`, `Tactic.Bound.Init`, and `Util.CompileInductive` |
| RingHom.lean | Deprecated module shim (deprecated 2026-01-01) that re-exports ring homomorphism related imports including `Algebra.Divisibility.Hom`, `Algebra.Ring.Hom.Defs`, and `Data.Set.Insert` |
| Sort.lean | Deprecated `List.Sorted` alias for `List.Pairwise` (deprecated 2025-10-11) with recommendations to use `SortedLE`, `SortedLT`, `SortedGE`, or `SortedGT` for preorders; includes deprecated lemmas like `sorted_nil`, `sorted_cons`, and `sorted_singleton` |

## Subdirectories

- [x] `MLList/` - Deprecated lazy list search algorithms including best-first search with priority estimation, beam search via `maxQueued`, and duplicate detection; built for `rw_search` tactic's edit-distance computations (deprecated 2025-09-11)

## Search Tags

deprecated compatibility backward-compat aliases estimator bounds thunk sorted pairwise list rw_search tactic removed legacy mathlib4 best-first-search priority-queue beam-search mllist lazy-list
