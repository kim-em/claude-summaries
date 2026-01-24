---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory
generated: 2026-01-24T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 38
subdirs_count: 19
---

# GroupTheory

## Overview

The `GroupTheory/` directory contains comprehensive formalization of group-theoretic concepts spanning foundational definitions through advanced theorems. Core topics include subgroup structure theory (complements, cosets, indices, quotients), classical theorems (Sylow theorems, Lagrange's theorem, Schur-Zassenhaus, class equation), group properties (nilpotent, solvable, p-groups, torsion, Archimedean), group constructions (free groups, free abelian groups, semidirect products, HNN extensions, coproducts), group actions (transitive, primitive, multiple primitivity, Jordan's theorem, Iwasawa), permutation groups, specific group families (cyclic, dihedral, quaternion, symmetric groups), and localization theory (monoid and Ore localization). The directory provides both the theoretical bedrock for algebraic structures and specialized machinery for concrete group-theoretic computations.

## Key Files

| File | Purpose |
|------|---------|
| Sylow.lean | Sylow theorems: existence of p-subgroups, conjugacy of Sylow subgroups, congruence properties of Sylow counts |
| OrderOfElement.lean | Order of group elements: IsOfFinOrder predicate, orderOf function, properties of finite/infinite order |
| Index.lean | Subgroup index theory and Lagrange's theorem: index definitions, divisibility properties, relative indices |
| Nilpotent.lean | Nilpotent groups: upper/central series, lower central series, nilpotency class, ascending/descending central series |
| Solvable.lean | Solvable groups: derived series, IsSolvable predicate, commutator subgroups |
| PGroup.lean | p-groups: IsPGroup definition, fixed point theorems, prime power order properties |
| FreeAbelianGroup.lean | Free abelian groups as abelianization of free groups, universal property, lift/map functoriality |
| Torsion.lean | Torsion groups and torsion-free groups: Monoid.IsTorsion, CommGroup.torsion subgroup, IsTorsionFree |
| Complement.lean | Subgroup complements: IsComplement, left/right transversals, coprime complement theorem |
| SchurZassenhaus.lean | Schur-Zassenhaus theorem: existence of complements for normal subgroups of coprime index |
| HNNExtension.lean | HNN extensions: construction adjoining stable letter with conjugation relations, Britton's lemma |
| Archimedean.lean | Archimedean ordered groups: cyclicity of subgroups with minimal positive elements, integer subgroups |
| ArchimedeanDensely.lean | Archimedean densely ordered groups (additional properties beyond basic Archimedean) |
| ClassEquation.lean | Class equation relating group order to conjugacy class sizes |
| Commensurable.lean | Commensurability of subgroups (finite index intersection) |
| CommutingProbability.lean | Commuting probability in finite groups |
| CosetCover.lean | Coset covering theory |
| CoprodI.lean | Indexed coproducts of groups |
| DedekindFinite.lean | Dedekind-finite groups (injective endomorphisms are surjective) |
| Divisible.lean | Divisible groups (equation solvability properties) |
| DivisibleHull.lean | Construction of divisible hull for abelian groups |
| DoubleCoset.lean | Double cosets HgK for subgroups H and K |
| EckmannHilton.lean | Eckmann-Hilton argument (two compatible monoid structures yield commutative group) |
| Exponent.lean | Group exponent (LCM of element orders) |
| Finiteness.lean | Finiteness conditions for groups |
| FixedPointFree.lean | Fixed-point-free group actions |
| Frattini.lean | Frattini subgroup (intersection of maximal subgroups) |
| Goursat.lean | Goursat's lemma on subgroups of direct products |
| IndexNormal.lean | Index-related properties for normal subgroups |
| NoncommCoprod.lean | Non-commutative coproduct (free product) of groups |
| NoncommPiCoprod.lean | Non-commutative product over indexed family |
| PresentedGroup.lean | Groups defined by generators and relations |
| PushoutI.lean | Indexed pushouts of groups |
| Rank.lean | Group rank (cardinality of minimal generating set) |
| RegularWreathProduct.lean | Regular wreath product construction |
| Schreier.lean | Schreier's subgroup theorem |
| SemidirectProduct.lean | Semidirect product of groups |
| Transfer.lean | Transfer homomorphism |

## Subdirectories

- [x] `Abelianization/` - Abelianization functor: definitions and finiteness properties
- [x] `Commutator/` - Commutator subgroups: basic theory and finiteness
- [x] `Congruence/` - Congruence relations on monoids and groups
- [x] `Coprod/` - Coproduct (free product) of two groups
- [x] `Coset/` - Coset theory: basic definitions and cardinality
- [x] `Coxeter/` - Coxeter groups and Coxeter systems
- [x] `FiniteAbelian/` - Structure theory of finite abelian groups
- [x] `FreeGroup/` - Free groups: constructions, reductions, normal forms
- [x] `GroupAction/` - Group actions: basic theory, blocks, conjugation, embeddings, fixed points, Jordan's theorem, primitivity, transitivity, quotients, support
- [x] `GroupExtension/` - Group extensions and extension theory
- [x] `MonoidLocalization/` - Localization of monoids (inverting elements)
- [x] `Order/` - Ordered groups
- [x] `OreLocalization/` - Ore localization for non-commutative rings/monoids
- [x] `Perm/` - Permutation groups: cycles, cycle types, sign, specific permutations
- [x] `QuotientGroup/` - Quotient groups by normal subgroups
- [x] `SpecificGroups/` - Concrete groups: cyclic, dihedral, quaternion, alternating, symmetric
- [ ] `Subgroup/` - Subgroup theory: basic operations, lattice structure, morphisms, products, normal subgroups
- [ ] `Submonoid/` - Submonoid theory (multiplicative substructures)
- [ ] `Subsemigroup/` - Subsemigroup theory (basic substructures)

## Search Tags

group-theory sylow lagrange nilpotent solvable p-group torsion free-group free-abelian-group group-action permutation coset quotient-group subgroup complement schur-zassenhaus hnn-extension semidirect-product coproduct archimedean cyclic element-order index abelianization commutator coxeter localization
