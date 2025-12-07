---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Functor/Derived
generated: 2025-12-07T17:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# Derived

## Overview

The `Derived/` directory formalizes derived functors in the general setting of category theory via localization and Kan extensions. This provides the foundation for both left and right derived functors as Kan extensions along localization functors, establishing that left derived functors are right Kan extensions while right derived functors are left Kan extensions. The directory includes the main theoretical development (definitions, uniqueness results, natural transformations between derived functors), pointwise constructions for right derived functors, and the derived adjunction theorem showing that adjoint functors induce adjoint derived functors under appropriate absoluteness conditions.

## Key Files

| File | Purpose |
|------|---------|
| RightDerived.lean | Right derived functors as left Kan extensions along localization functors: defines `IsRightDerivedFunctor` typeclass, `totalRightDerived` construction, uniqueness up to isomorphism, and natural transformations between derived functors |
| LeftDerived.lean | Left derived functors as right Kan extensions along localization functors: defines `IsLeftDerivedFunctor` typeclass, `totalLeftDerived` construction, uniqueness results (dual to RightDerived.lean) |
| PointwiseRightDerived.lean | Pointwise right derived functors via pointwise left Kan extensions: proves functors inverting `W` have pointwise right derived functors, provides `isPointwiseLeftKanExtensionOfIsoOfIsLocalization` construction |
| Adjunction.lean | Derived adjunction theorem: if `G ⊣ F` and `G'`, `F'` are absolute left/right derived functors respectively, then `G' ⊣ F'` with explicit unit/counit constructions (references Maltsiniotis 2007) |

## Subdirectories

(none)

## Search Tags

derived-functors category-theory localization kan-extensions left-derived right-derived adjunctions pointwise-derived maltsiniotis total-derived-functor
