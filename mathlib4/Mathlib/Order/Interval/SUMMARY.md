---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Interval
generated: 2026-01-26T23:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 2
---

# Interval

## Overview

The `Interval/` directory provides a comprehensive three-layer formalization of order intervals in Mathlib: abstract interval objects, finite set intervals, and infinite set intervals. At the top level, `Basic.lean` defines intervals as first-class algebraic objects (`NonemptyInterval` and `Interval`) with ordering, lattice operations, and coercions to sets, suitable for interval arithmetic. `Lex.lean` provides lexicographic ordering on these interval objects, and `Multiset.lean` wraps the finset API for locally finite orders.

The `Finset/` subdirectory (7 files) implements intervals as finite sets via the `LocallyFiniteOrder` typeclass, which axiomatizes orders where all bounded intervals are finite. It provides concrete implementations for ℕ and `Fin n`, proves that linear locally finite orders cannot be densely ordered (unless trivial), and establishes relationships between interval types in successor orders. The `SuccPred.lean` module shows how adjacent intervals relate (`Ico (succ a) b = Ioo a b`), while `Box.lean` demonstrates decomposition of ordered rings into hollow interval "boxes" for counting arguments.

The `Set/` subdirectory (25 files) is the most comprehensive component, providing the foundational theory of intervals as infinite sets. Starting from core definitions and the fundamental `OrdConnected` typeclass (sets containing all intermediate points), it covers all standard interval notations (`Icc/Ico/Ioc/Ioo` for bounded, `Ici/Iic/Ioi/Iio` for unbounded), unordered intervals (`uIcc`) that work regardless of endpoint ordering (useful for bounding boxes), and extensive theory on how intervals interact with monotone functions, projections, order embeddings, successor/predecessor structure, and type constructors (`Fin`, `Pi`, `WithBot`, `WithTop`). This layer provides the theoretical foundation that the other representations build upon.

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
