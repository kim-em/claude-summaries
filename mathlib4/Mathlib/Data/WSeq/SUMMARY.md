---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/WSeq
generated: 2025-12-11T12:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 4
subdirs_count: 0
---

# WSeq

## Overview

The `WSeq` (weak sequence) module provides a type for representing partially defined, possibly infinite lists where each element computation may involve an indeterminate amount of work, including potentially infinite loops. Unlike regular `Seq` which allows infinite lists but requires each element to be immediately available, `WSeq α` is defined as `Seq (Option α)` where `none` values represent ongoing computation ("thinking"). This model is appropriate for Haskell-style lazy lists and supports most interesting computation patterns on infinite data, though extracting elements requires `Computation` wrappers to handle potential non-termination.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `WSeq` type definition and fundamental operations: `nil`, `cons`, `think`, `destruct`, `head`, `tail`, `drop`, `get?`, `toList`, `append`, `join`, `map`, `bind`, plus the `Monad` instance (noting it doesn't satisfy monad laws exactly, only up to equivalence) |
| Defs.lean | Additional operations: `length`, `IsFinite` class, `get` for finite sequences, `updateNth`, `removeNth`, `filterMap`, `filter`, `find`, `zipWith`, `zip`, `findIndexes`, `findIndex`, `indexOf`, `indexesOf`, `union`, `isEmpty`, `compute`, `take`, `splitAt`, `any`, `all`, `scanl`, `inits`, `collect` |
| Relation.lean | Bisimulation and equivalence infrastructure: `LiftRelO` lifts relations to option pairs, `LiftRel` defines coinductive relation between sequences, `Equiv` (`~ʷ`) defines equivalence up to computation steps; includes congruence lemmas for all operations and proofs that `LiftRel` respects reflexivity, symmetry, transitivity |
| Productive.lean | `Productive` class for sequences that never stall forever (always finite `think`s between `cons`es); includes `toSeq` to convert productive weak sequences to regular sequences |

## Subdirectories

(none)

## Search Tags

weak-sequences lazy-lists coinductive infinite-lists computation partiality bisimulation equivalence monad productive sequences
