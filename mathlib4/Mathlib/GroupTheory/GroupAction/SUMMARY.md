---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/GroupAction
generated: 2026-01-24T22:58:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 22
subdirs_count: 2
---

# GroupAction

## Overview

The `GroupAction/` directory provides comprehensive formalization of group actions, including core definitions (orbits, stabilizers, fixed points), structural properties (transitivity, primitivity, multiple primitivity/transitivity), blocks and primitive actions, equivariant homomorphisms, quotient structures, and specialized constructions (conjugation actions, domain actions, sub-mul-actions). Notable advanced content includes Jordan's theorems on primitive permutation groups (Wielandt 1964), the orbit-stabilizer theorem, Burnside's lemma, and the class formula. The directory combines foundational action theory with sophisticated results from permutation group theory.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: orbit, fixedPoints, fixedBy, stabilizer for group actions |
| Basic.lean | Basic properties of orbits, stabilizers, and fixed points beyond algebraic manipulation |
| Blocks.lean | Block systems for group actions: IsBlock predicate, trivial/non-trivial blocks, cardinality results for finite actions |
| Primitive.lean | Primitive and preprimitive actions: IsPreprimitive, IsQuasiPreprimitive, relation with stabilizers |
| MultiplePrimitivity.lean | Multiple primitivity for group actions (higher-order primitivity conditions) |
| MultipleTransitivity.lean | Multiple transitivity for group actions (k-transitivity for k ≥ 1) |
| Transitive.lean | Pretransitive actions: characterizations via orbits and base points, equivariant preservation |
| Jordan.lean | Jordan's theorems on primitive permutation groups (Wielandt 13.1-13.3): 2-pretransitivity criteria, primitivity with swaps/3-cycles |
| Hom.lean | Equivariant homomorphisms: MulActionHom, DistribMulActionHom, SMulSemiringHom and their type classes |
| Quotient.lean | Group action properties via quotients: orbit-stabilizer theorem, class formula, Burnside's lemma |
| ConjAct.lean | Conjugation action: ConjAct type and conjugation by group elements |
| SubMulAction.lean | Sub-mul-actions: invariant subsets of group actions |
| FixedPoints.lean | Fixed point theory for group actions |
| FixingSubgroup.lean | Fixing subgroups: elements fixing a given set |
| Embedding.lean | Embeddings of group actions |
| Support.lean | Support of group actions |
| Iwasawa.lean | Iwasawa's lemma for group actions |
| Pointwise.lean | Pointwise operations on group actions |
| Period.lean | Period of elements under group actions |
| IterateAct.lean | Iteration of group actions |
| CardCommute.lean | Cardinality of commuting elements in group actions |
| Ring.lean | Ring-theoretic aspects of group actions |

## Subdirectories

- [x] `DomAct/` - Domain actions (specialized action type)
- [~] `SubMulAction/` - Sub-mul-action theory: closure, combinations, fixing subgroups, stabilizers, pointwise operations

## Search Tags

group-action orbit stabilizer fixed-points transitive primitive preprimitive blocks jordan-theorem equivariant-homomorphism quotient orbit-stabilizer burnside conjugation sub-mul-action multiple-transitivity multiple-primitivity iwasawa permutation-group
