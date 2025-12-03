---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Interval/Finset
generated: 2025-12-01T21:35:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Finset

## Overview

The `Finset/` directory provides algebraic properties and operations on finite set intervals (`Finset.Ixx`). It proves that addition operations (left and right translation) on closed, half-open, and open intervals (Icc, Ico, Ioc, Ioo) correctly shift endpoints in ordered cancel additive monoids. It also establishes relations between intervals in successor-predecessor orders, showing how intervals transform under addition/subtraction of one, and proving equivalences between different interval types (e.g., `Ico (a + 1) b = Ioo a b`).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Translation of finset intervals under addition: proves that mapping left/right addition over Finset intervals (Icc, Ico, Ioc, Ioo) correctly shifts both endpoints; includes both embedding-based `map` lemmas and decidable `image` lemmas for ordered cancel additive monoids |
| SuccPred.lean | Finset interval relations in successor-predecessor orders: proves equivalences between interval types under `+1`/`-1` operations (e.g., `Ico (a+1) b = Ioo a b`, `Icc a (b-1) = Ico a b`) and insertion lemmas for constructing intervals by inserting endpoints; handles both orders with/without maximal/minimal elements |

## Subdirectories

*(No subdirectories)*

## Search Tags

finset-intervals interval-translation finset-algebra ordered-cancel-additive-monoid interval-Icc interval-Ico interval-Ioc interval-Ioo addition-embedding successor-predecessor succ-add-order pred-sub-order interval-equivalence locally-finite-order interval-insertion
