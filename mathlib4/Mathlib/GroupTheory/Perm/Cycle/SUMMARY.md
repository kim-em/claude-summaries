---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/Perm/Cycle
generated: 2026-01-24T23:25:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Cycle

## Overview

The `Cycle/` directory contains a comprehensive formalization of cycle theory for permutations, including cycle decomposition, cycle types, and related properties. It provides both the abstract theory of cycles (the `SameCycle` equivalence relation, `IsCycle` and `IsCycleOn` predicates) and concrete computational machinery (converting between permutations and cycle representations via lists). The directory covers cycle factorization into disjoint cycles, cycle types as multisets of support cardinalities, conjugacy classification via cycle types, and applications including Cauchy's theorem for finite groups.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core cycle theory: `SameCycle` equivalence relation, `IsCycle` and `IsCycleOn` predicates, cycle properties under conjugation and powers, support relationships, fixed points |
| Concrete.lean | Concrete cycle representations via lists/cycles: `Cycle.formPerm` for constructing permutations from cycles, `Equiv.Perm.toList`/`toCycle` for converting permutations to cycle notation, bijection between cyclic permutations and nontrivial cycles |
| Factors.lean | Cycle decomposition: `cycleOf` (the cycle containing a given element), `cycleFactorsFinset` (disjoint cycle factorization), properties of cycle factors, commutativity and disjointness of cycles |
| Type.lean | Cycle types: `cycleType` (multiset of cycle lengths), partition correspondence, sign formulas via cycle type, lcm/orderOf relationships, conjugacy classification theorem (`isConj_iff_cycleType_eq`), Cauchy's theorem, three-cycles |
| PossibleTypes.lean | Characterization of realizable cycle types: proves permutations exist with cycle type `m` iff `m.sum ≤ Fintype.card α` and all entries `≥ 2` |

## Subdirectories

(none)

## Search Tags

cycle permutation cycle-type cycle-decomposition disjoint-cycles cycleOf cycleFactorsFinset SameCycle IsCycle IsCycleOn formPerm toList toCycle conjugacy partition sign orderOf lcm Cauchy-theorem three-cycle isSwap cycleType support fixed-point
