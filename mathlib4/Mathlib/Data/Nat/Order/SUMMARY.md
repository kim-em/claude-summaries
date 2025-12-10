---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat/Order
generated: 2025-12-11T22:45:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 1
subdirs_count: 0
---

# Order

## Overview

The `Order/` directory contains additional order-theoretic lemmas for natural numbers, primarily focused on set-theoretic properties. It provides `OrderBot` and `SemilatticeSup` instances for subtypes of `Nat`, enabling lattice operations on subsets of natural numbers. The file also includes lemmas about characterizing when a set of naturals equals the universe, and existence lemmas for finding elements satisfying predicates.

## Key Files

| File | Purpose |
|------|---------|
| Lemmas.lean | Order-theoretic lemmas for sets of naturals: `OrderBot` instance for nonempty decidable subsets (with bot = smallest element via `Nat.find`), `SemilatticeSup` for any subset, and lemmas like `set_eq_univ` characterizing when S = univ via induction |

## Subdirectories

None.

## Search Tags

natural-numbers order lattice orderbot semilattice-sup subtype set nat-find induction
