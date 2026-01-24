---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/Perm
generated: 2026-01-24T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 15
subdirs_count: 1
---

# Perm

## Overview

The `Perm/` directory contains the formalization of permutation groups (symmetric groups) and their properties. Core topics include permutation support (the set of elements moved by a permutation), disjointness of permutations, swap operations, sign/parity of permutations, cycles and cycle types, permutations of finite types (especially `Fin n`), permutations constructed from lists, and the algebraic structure of centralizers and maximal subgroups. The directory provides both the theoretical foundations for symmetric groups and computational machinery for working with specific permutations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Miscellaneous lemmas about `Equiv.Perm`, including image/preimage properties and bijections on sets |
| Support.lean | Support of permutations (elements not fixed), disjointness predicate, swap predicate, commuting properties |
| Sign.lean | Sign/parity homomorphism for permutations: `sign : Perm α →* ℤˣ`, sign computation via swap factorizations, sign properties |
| Finite.lean | Permutations on finite types: conjugation, order of elements, support properties for finite permutations |
| List.lean | Permutations constructed from lists via `formPerm`, cyclic permutations from rotations, support of list-based permutations |
| Fin.lean | Permutations of `Fin n`: decomposition lemmas, cycle ranges, rotation permutations, sign computations for `Fin` permutations |
| Centralizer.lean | Centralizer subgroups of permutations, conjugacy class cardinality via orbit-stabilizer theorem, action on cycle factors |
| MaximalSubgroups.lean | Maximal subgroups of symmetric groups, intransitive case of O'Nan-Scott classification via stabilizers |
| Closure.lean | Closure properties of permutation sets under group operations |
| ClosureSwap.lean | Generating symmetric groups from specific sets of swaps |
| ConjAct.lean | Conjugation action on permutations |
| DomMulAct.lean | Multiplicative action of permutations on their domain |
| Option.lean | Permutations of `Option α` types |
| Subgroup.lean | Subgroup properties specific to permutation groups |
| ViaEmbedding.lean | Permutations via embeddings between types |

## Subdirectories

- [x] `Cycle/` - Cycle decomposition: basic cycle theory, concrete cycles, cycle factorizations, cycle types

## Search Tags

permutation symmetric-group swap sign parity support disjoint cycle cycle-type conjugacy centralizer fin list formPerm maximal-subgroup transposition
