---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Interval
generated: 2026-01-26T22:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 3
subdirs_count: 2
---

# Interval

## Overview

The `Interval/` directory provides formalization of order intervals in multiple representations: as abstract data types (`NonemptyInterval` and `Interval`), as finite sets (`Finset`), as infinite sets (`Set`), and as multisets. The core `Basic.lean` file defines intervals as first-class objects with ordering and lattice structure, suitable for interval arithmetic. These interval types can be converted to their corresponding set/finset/multiset representations and provide consistent APIs across all representations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core interval types: `NonemptyInterval α` (pairs with `fst ≤ snd`) and `Interval α` (nonempty or empty); order structures, lattice operations, coercions to `Set α`, dual operations, map/map₂ pushforward |
| Lex.lean | Lexicographic total order on intervals compatible with inclusion ordering; orders intervals by reverse first endpoint then second endpoint (e.g., `[(3,3), (2,2), (2,3), (1,1), (1,2), (1,3)]` is sorted) |
| Multiset.lean | Intervals as multisets in `LocallyFiniteOrder`: `Multiset.Icc/Ico/Ioc/Ioo` for finite intervals, `Ici/Ioi/Iic/Iio` for infinite intervals; wrapper around `Finset` interval API |

## Subdirectories

- [x] `Finset/` - Intervals as finite sets
- [x] `Set/` - Intervals as infinite sets

## Search Tags

interval order-interval nonempty-interval closed-interval open-interval Icc Ico Ioc Ioo finite-interval locally-finite lexicographic-order interval-arithmetic multiset finset set order-theory
