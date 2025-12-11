---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Vector
generated: 2025-12-11T13:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 6
subdirs_count: 0
---

# Vector

## Overview

This folder provides `List.Vector α n`, the type of lists with statically-known length `n`. Unlike the root namespace `Vector α n` (which is array-based and optimized for programming), `List.Vector` is subtype-based (`{l : List α // l.length = n}`) and designed for mathematical reasoning. The folder establishes a comprehensive API including constructors, accessors, mapping operations, accumulator functions, membership lemmas, and induction principles for vectors.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `List.Vector α n` type, `nil`, `cons`, `head`, `tail`, `get`, `map`, `pmap`, `map₂`, `replicate`, `drop`, `take`, `eraseIdx`, `ofFn`, `mapAccumr`, `mapAccumr₂`, shift primitives, and basic theorems about `toList` |
| Basic.lean | Extended API: `::ᵥ` notation for cons, extensionality, induction principles (`inductionOn`, `inductionOn₂`, `inductionOn₃`), `reverse`, `scanl`, monadic operations (`mOfFn`, `mmap`), `Traversable` instance, `insertIdx`, `set`, and additional simp lemmas |
| MapLemmas.lean | Normalization lemmas for `map`/`mapAccumr` operations: folding nested operations, bisimulation proofs for equality, redundant state optimization, unused input optimization, and commutativity/flip lemmas |
| Mem.lean | Membership theorems: `get_mem`, `mem_iff_get`, `mem_cons_iff`, `mem_succ_iff`, `head_mem`, `mem_of_mem_tail`, and related lemmas for `map` |
| Snoc.lean | Right-append operation `snoc : Vector α n → α → Vector α (n+1)`, reverse induction principles (`revInductionOn`, `revInductionOn₂`, `revCasesOn`), and simp lemmas showing how operations reduce on `snoc` |
| Zip.lean | `zipWith : (α → β → γ) → Vector α n → Vector β n → Vector γ n` operation with simp lemmas and a theorem relating products to zipWith for commutative monoids |

## Subdirectories

(none)

## Search Tags

vector list-vector fixed-length-list length-indexed cons snoc head tail get map mapAccumr zipWith traversable induction reverse scanl membership subtype
