---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Ordmap
generated: 2025-12-11T12:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 3
subdirs_count: 0
---

# Ordmap

## Overview

This directory implements weight-balanced binary search trees (ordered maps/sets) for Lean 4, based on Adams' "Efficient sets: a balancing act" algorithm. The implementation provides a verified ordered set data structure with O(log n) operations for lookup, insertion, and deletion. The files progress from raw operations (`Ordnode`) to invariant definitions (`Invariants`) to a fully verified wrapper type (`Ordset`).

## Key Files

| File | Purpose |
|------|---------|
| Ordnode.lean | Core `Ordnode α` inductive type and operations: singleton, size, membership, insert, erase, find, split, merge, union, diff, intersection, filter, map, fold, and list conversions. Ported from Haskell's `Data.Set`. Operations assume but do not verify tree invariants. |
| Invariants.lean | Defines correctness invariants for `Ordnode`: `Sized` (size fields match actual sizes), `Balanced` (subtree sizes differ by at most δ=3), `Bounded` (BST property with elements in strictly increasing order). Proves basic lemmas about `dual`, `toList`, balance operations, and `All`/`Any` predicates. |
| Ordset.lean | The verified `Ordset α` wrapper type (subtype of `Ordnode` satisfying `Valid`). Defines `Valid'` predicate combining `Bounded`, `Sized`, and `Balanced`. Proves correctness of `insert`, `insert'`, `erase`, `merge`, `glue`, and `map` operations. Exposes safe API: `nil`, `singleton`, `size`, `insert`, `mem`, `find`, `erase`, `map`. |

## Subdirectories

(none)

## Search Tags

ordmap ordered-map ordered-set binary-search-tree weight-balanced-tree data-structure verified-programming bst insertion deletion balanced-tree
