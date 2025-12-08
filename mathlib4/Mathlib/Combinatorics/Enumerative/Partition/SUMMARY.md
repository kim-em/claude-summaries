---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Enumerative/Partition
generated: 2025-12-08T15:50:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 2
subdirs_count: 0
---

# Partition

## Overview

The `Partition/` subdirectory formalizes integer partitions and their generating functions. A partition of `n` is a way of writing `n` as a sum of positive integers where order doesn't matter (contrast with compositions where order matters). The core structure `Partition n` is implemented as a multiset of positive integers summing to `n`. The directory includes foundational definitions, conversions between partitions and other structures (compositions, symmetric functions), special partition types (odd parts, distinct parts), and a complete theory of generating functions with infinite product formulas.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `Partition n` structure as multiset of positive naturals summing to `n`; conversions `ofComposition`, `ofMultiset`, `ofSym` (from symmetric functions); `toFinsuppAntidiag` embedding into finitely-supported functions; special partitions `indiscrete` (single part), `odds` (odd parts only), `distincts` (no repeated parts), `oddDistincts`; finiteness proof via surjection from compositions; unique partitions for 0 and 1 |
| GenFun.lean | Generating functions for partitions with character functions `f(i, c)` where `i` is a part and `c` its multiplicity; defines `genFun f` as power series with coefficient `∑ p : n.Partition, ∏ i, f(i, count i)` at `X^n`; proves infinite product formula `genFun f = ∏' i, (1 + ∑' j, f(i+1)(j+1) • X^((i+1)*(j+1)))` via `hasProd_genFun` with convergence in Pi topology; specializes to partition function, distinct parts, and odd parts generating functions |

## Subdirectories

*(No subdirectories)*

## Search Tags

integer-partitions partition-theory multisets enumerative-combinatorics generating-functions power-series infinite-products euler-partition-theorem odd-partitions distinct-partitions symmetric-functions composition-to-partition finsupp-antidiag character-functions partition-function
