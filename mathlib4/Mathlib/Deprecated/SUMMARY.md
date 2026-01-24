---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Deprecated
generated: 2025-01-24T10:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: preliminary
files_count: 5
subdirs_count: 1
---

# Deprecated

## Overview

The `Deprecated/` folder contains definitions and theorems that have been deprecated from the main Mathlib library but are maintained for backward compatibility during transition periods. Each file contains aliases, shims, or entire deprecated modules with explicit `@[deprecated]` attributes indicating when they were deprecated and what (if anything) replaces them. These items were typically used in removed features (like the `rw_search` tactic) or superseded by better alternatives (like `List.Sorted` being replaced by `List.Pairwise`).

## Key Files

| File | Purpose |
|------|---------|
| Aliases.lean | Empty placeholder file for deprecated aliases no longer used in Mathlib; provides a dumping ground for aliases whose imports would otherwise be unnecessary |
| Estimator.lean | Deprecated typeclass framework for computing improvable lower bounds on lazy values; `Estimator a ε` provides iteratively refinable bounds for `a : Thunk α`, previously used by the removed `rw_search` tactic (deprecated 2025-09-11) |
| Order.lean | Deprecated module shim (deprecated 2025-09-02) that re-exports order-related tactics including `Tactic.Linter.DeprecatedModule`, `Tactic.Basic`, `Tactic.Bound.Init`, and `Util.CompileInductive` |
| RingHom.lean | Deprecated module shim (deprecated 2026-01-01) that re-exports ring homomorphism related imports including `Algebra.Divisibility.Hom`, `Algebra.Ring.Hom.Defs`, and `Data.Set.Insert` |
| Sort.lean | Deprecated `List.Sorted` alias for `List.Pairwise` (deprecated 2025-10-11) with recommendations to use `SortedLE`, `SortedLT`, `SortedGE`, or `SortedGT` for preorders; includes deprecated lemmas like `sorted_nil`, `sorted_cons`, and `sorted_singleton` |

## Subdirectories

- [x] `MLList/` - Deprecated lazy list search algorithms including best-first search with priority estimation

## Search Tags

deprecated compatibility backward-compat aliases estimator bounds thunk sorted pairwise list rw_search tactic removed legacy mathlib4
