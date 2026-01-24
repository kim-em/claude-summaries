---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/FreeGroup
generated: 2026-01-24T22:48:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 0
---

# FreeGroup

## Overview

The `FreeGroup/` directory contains a comprehensive formalization of free groups, including their fundamental construction, reduction algorithms, and key structural theorems. The core definition implements free groups as words over generators modulo the relation `x * x⁻¹ ~ 1`, with a quotient construction using the Church-Rosser reduction system. The directory provides both the concrete `FreeGroup α` construction and abstract characterizations via `IsFreeGroup` typeclass, algorithmic word reduction and normal forms, the Nielsen-Schreier theorem (subgroups of free groups are free), and specialized results on cyclically reduced words, group actions, and basis equivalences. This provides both computational machinery for working with explicit free group elements and abstract infrastructure for reasoning about free group properties.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core free group construction: defines `FreeGroup α` as quotient of `List (α × Bool)` by reduction relation, reduction steps, Church-Rosser theorem, canonical injection `of : α → FreeGroup α`, universal property `lift`, monad structure, and isomorphism `freeGroupUnitEquivInt` between `FreeGroup Unit` and `ℤ` |
| IsFreeGroup.lean | Abstract free group interface: `FreeGroupBasis ι G` structure recording isomorphism between `G` and `FreeGroup ι`, `IsFreeGroup G` typeclass for groups admitting free bases, generators and universal property, uniqueness of lifts, and conversions between concrete and abstract free group presentations |
| NielsenSchreier.lean | Nielsen-Schreier theorem: proves that every subgroup of a free group is itself free using groupoid-theoretic methods (analogous to covering space proof), defines `IsFreeGroupoid`, and establishes `subgroupIsFreeOfIsFree` instance |
| Reduce.lean | Maximal reduction algorithm: computable `reduce` function computing normal forms of words (requires `DecidableEq α`), `norm` function for word length after reduction, proofs that `reduce L` is the unique reduced form of `L`, and characterization theorems for the reduction process |
| CyclicallyReduced.lean | Cyclically reduced words: `IsCyclicallyReduced` predicate for words where first and last letters don't cancel, properties of cyclic reduction, proof that free groups are strongly torsion-free (`IsMulTorsionFree`), and power injectivity results |
| GeneratorEquiv.lean | Basis equivalence theorems: proves isomorphic free groups have equivalent generator sets via abelianization and linear algebra, `Equiv.ofFreeGroupEquiv` for concrete free groups, `Equiv.ofIsFreeGroupEquiv` for abstract free groups, using strong rank condition for ℤ-modules |
| Orbit.lean | Group action orbits: defines `startsWith w` as elements beginning with letter `w`, analyzes orbit structure under free group actions, proves `Orbit.duplicate` theorem relating orbits under different starting letters, disjointness and injectivity properties of `startsWith` sets |

## Subdirectories

(none)

## Search Tags

free-group word-reduction church-rosser nielsen-schreier universal-property group-basis cyclically-reduced torsion-free normal-form reduction-algorithm group-action orbit generators lift monad quotient
