---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Seq
generated: 2025-12-11T09:00:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 6
subdirs_count: 0
---

# Seq

## Overview

The `Seq/` directory provides coinductive types for possibly infinite computations and sequences. It defines `Computation α` for unbounded computations that may never terminate, and `Seq α` for possibly infinite lists (sequences). These types use coinductive encoding as infinite streams of `Option` values with termination properties. The module also includes parallel computation of sequences of computations via diagonal enumeration.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions for `Seq α` (possibly infinite lists) and `Seq1 α` (nonempty sequences); provides constructors (`nil`, `cons`), destructors (`head`, `tail`, `destruct`), corecursion (`corec`), bisimulation principles, termination predicates, membership, conversions (to/from `List`, `Stream'`, `MLList`), and operations (`map`, `append`, `join`, `zip`, `fold`, `drop`, `take`, `enum`, `Pairwise`) |
| Basic.lean | Additional lemmas for `Seq α` including length properties (`length`, `length'`), termination conditions, and various utility theorems building on `Defs.lean` |
| Computation.lean | Defines `Computation α` as the type of unbounded computations returning `α`; provides constructors (`pure`, `think`, `thinkN`), destructor (`destruct`), coroutine operations, termination predicates, bind/map/join operations for monadic composition, and equivalence relations on computations |
| Parallel.lean | Parallel computation of a computable sequence of computations via diagonal enumeration; the key theorems are `terminates_parallel` and `exists_of_mem_parallel`; this operation is nondeterministic (does not honor sequence equivalence) |
| Seq.lean | Deprecated module file (since 2025-08-26) that re-exports `Basic.lean` |
| WSeq.lean | Deprecated module file (since 2025-04-13) that re-exports the `WSeq` modules (weak sequences moved to `Mathlib/Data/WSeq/`) |

## Subdirectories

*(none)*

## Search Tags

seq sequence possibly-infinite-list computation coinductive corecursion bisimulation parallel-computation unbounded-computation streams termination
