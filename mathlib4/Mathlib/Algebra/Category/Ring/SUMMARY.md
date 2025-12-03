---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/Ring
generated: 2025-12-03T10:55:00Z
git_sha: 5bfa1623542d7f245e45ac880c26cfe8f9ecc5ea
git_branch: heads/nightly-testing
status: preliminary
files_count: 11
subdirs_count: 1
---

# Ring

## Overview

The `Ring/` directory contains the categorical formulation of ring theory in Mathlib4, defining bundled categories for semirings, rings, commutative semirings, and commutative rings (`SemiRingCat`, `RingCat`, `CommSemiRingCat`, `CommRingCat`). It provides the complete categorical infrastructure including morphisms (ring homomorphisms), forgetful functors to other algebraic categories, limits and colimits constructions, adjunctions, and categorical properties specific to ring categories. The directory includes specialized functionality for finite presentations, filtered colimits, epimorphisms, topological structures on homomorphism sets, and constructions involving tensor products and algebras.

## Key Files

| File | Purpose |
|------|---------|
| Adjunctions.lean | Adjunctions in `CommRingCat`: free commutative ring functor `Type ⥤ CommRingCat` (mapping `X` to `ℤ[X]`), coyoneda adjunctions, monoid algebra adjunctions, and the adjunction between group rings and units |
| Basic.lean | Core definitions of bundled ring categories (`SemiRingCat`, `RingCat`, `CommSemiRingCat`, `CommRingCat`) with morphisms as ring homomorphisms, forgetful functors to monoids and additive structures, and basic categorical structure including concrete category instances |
| Colimits.lean | Construction of colimits in `RingCat` and `CommRingCat` using free ring constructions on disjoint unions modulo ring laws and diagram morphisms; proves these categories have all colimits |
| Constructions.lean | Explicit (co)limit constructions in `CommRingCat`: tensor product as pushout, tensor product over `ℤ` as binary coproduct, `ℤ` as initial object, `0` as strict terminal object, Cartesian products, Pi objects, and equalizers via `RingHom.eqLocus` |
| Epi.lean | Characterization of epimorphisms in `CommRingCat`: proves surjective ring homomorphisms are equivalent to epi + finite (via tensor product characterization `s ⊗ 1 = 1 ⊗ s`) |
| FilteredColimits.lean | Proves forgetful functors from `SemiRingCat`, `CommSemiRingCat`, `RingCat`, and `CommRingCat` preserve filtered colimits by showing filtered colimits in `MonCat` carry semiring/ring structure |
| FinitePresentation.lean | Theory of finitely presented rings in the categorical setting: rings that are quotients of polynomial rings `ℤ[X₁,...,Xₙ]` by finitely generated ideals; proves categorical equivalences and preservation properties |
| Instances.lean | Concrete instances showing specific categories (`SemiRingCat`, `RingCat`, `CommSemiRingCat`, `CommRingCat`) have forgetful functors to `CommMonCat` |
| Limits.lean | Construction of limits in all four ring categories using subsemiring/subring of sections; proves these categories have all limits and that forgetful functors preserve limits |
| LinearAlgebra.lean | Interplay between `ModuleCat` and ring categories: functoriality of base change for modules under ring homomorphisms, preservation of limits by these functors |
| Topology.lean | Topology on `Hom(A, R)` for topological rings `R` (coarsest topology making evaluation maps continuous); proves closed embedding properties, homeomorphisms for polynomial rings, and subspace topology for tensor products |

## Subdirectories

- [ ] `Under/` - API for the comma category `Under R` (equivalent to category of commutative `R`-algebras) including algebra homomorphisms and categorical constructions (pending)

## Search Tags

category-theory ring-categories semirings rings commutative-rings bundled-categories ring-homomorphisms forgetful-functors limits colimits adjunctions concrete-categories tensor-products algebras filtered-colimits epimorphisms finite-presentation topological-rings polynomial-rings initial-objects terminal-objects pushouts products coproducts equalizers categorical-algebra
