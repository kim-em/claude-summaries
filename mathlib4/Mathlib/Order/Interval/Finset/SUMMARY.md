---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Interval/Finset
generated: 2026-01-26T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 0
---

# Finset

## Overview

The `Finset/` subdirectory implements intervals as finite sets in locally finite orders. It defines the `LocallyFiniteOrder` typeclass (orders where all bounded intervals are finite), provides implementations for concrete types (ℕ, Fin n), and proves properties about interval operations. Key functionality includes converting intervals to finsets (`Finset.Icc/Ico/Ioc/Ioo`), proving relationships between interval types in successor orders, and establishing that linear locally finite orders cannot be densely ordered (unless trivial).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core `LocallyFiniteOrder` typeclass: defines `finsetIcc/Ico/Ioc/Ioo` for bounded intervals, `LocallyFiniteOrderTop/Bot` for unbounded intervals (`Ici/Ioi/Iic/Iio`); instance constructors from order embeddings, subtypes, products; unordered intervals `uIcc` |
| Basic.lean | General properties of finset intervals: nonemptiness conditions, emptiness characterizations, transitive closure theorems (`le_iff_transGen_wcovBy`, `lt_iff_transGen_covBy`), monotonicity characterizations via covers |
| Nat.lean | `LocallyFiniteOrder ℕ` instance using `List.range'`; cardinality formulas (`card_Icc a b = b + 1 - a`); singleton interval lemmas; equivalence `Finset.range = Ico 0` |
| Fin.lean | `LocallyFiniteOrder (Fin n)` instance via `attachFin` from ℕ intervals; `LocallyFiniteOrderBot/Top` instances; cardinality formulas; image and preimage lemmas under `Fin.val` |
| SuccPred.lean | Relations between intervals in successor/predecessor orders: `Ico (succ a) b = Ioo a b`, `Icc (succ a) b = Ioc a b` (when not max), insertion lemmas (`insert a (Icc (succ a) b) = Icc a b`) |
| DenselyOrdered.lean | Proves linear locally finite orders are densely ordered iff subsingleton (`denselyOrdered_iff_subsingleton`); extends result to `WithBot` and `WithTop` sets; explains why `DenselyOrdered` appears in API despite impossibility |
| Box.lean | Decomposition of locally finite ordered rings into "boxes" (hollow intervals): `box n = Icc (-n) n \ Icc (-(n-1)) (n-1)`; cardinality formula for `ℤ × ℤ` boxes (`card_box n = 8 * n`); unique box membership |

## Subdirectories

None.

## Search Tags

locally-finite-order finset interval Icc Ico Ioc Ioo Ici Ioi Iic Iio finite-interval natural-numbers fin successor-order predecessor-order densely-ordered box-decomposition cardinality transitive-closure covers wcovby covby monotone
