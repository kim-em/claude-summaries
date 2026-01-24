---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/Perm
generated: 2026-01-24T23:35:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 15
subdirs_count: 1
---

# Perm

## Overview

The `Perm/` directory provides a comprehensive formalization of permutation groups (symmetric groups) and their properties, serving as a central component of Mathlib's group theory library. The directory spans from foundational concepts (permutation support, disjointness, swap operations) through advanced theory (cycle decomposition, cycle types, conjugacy classification) to specialized applications (permutations of `Fin n`, maximal subgroups, centralizers). At the core are 15 files covering support theory, sign/parity homomorphisms, finite permutations, list-based constructions, and group-theoretic structure. The `Cycle/` subdirectory contains the deep cycle theory, including the complete cycle decomposition theorem, cycle types as conjugacy invariants, and applications like Cauchy's theorem. Together, these provide both abstract theoretical foundations (conjugacy via cycle types, O'Nan-Scott classification fragments) and concrete computational machinery (converting between permutations and cycle notation, computing signs and orders).

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
