---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category
generated: 2025-12-02T12:00:00Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: preliminary
files_count: 3
subdirs_count: 13
---

# Category

## Overview

The `Category/` directory contains categorical aspects of algebraic structures, defining bundled categories for various algebraic objects (groups, rings, modules, algebras, bialgebras, etc.) with their morphisms, forgetful functors, and categorical properties. It provides the infrastructure for treating algebraic structures as objects in categories, enabling categorical constructions like limits, colimits, and equivalences. The directory includes both classical algebraic categories (groups, rings, modules) and more specialized structures (Hopf algebras, coalgebras, continuous cohomology).

## Key Files

| File | Purpose |
|------|---------|
| BoolRing.lean | Category of Boolean rings with morphisms as ring homomorphisms; defines forgetful functor to `CommRingCat` and equivalence with `BoolAlg` (Boolean algebras as categories) |
| CommBialgCat.lean | Category of commutative bialgebras over a commutative ring `R` with morphisms as bialgebra homomorphisms; includes forgetful functor to `CommAlgCat` and equivalence with comonoid objects in `(CommAlgCat R)ᵒᵖ` |
| GrpWithZero.lean | Category of groups with zero (`GroupWithZero`) with morphisms as monoid-with-zero homomorphisms; includes forgetful functors to `MonCat` and `Bipointed` |

## Subdirectories

- [x] `AlgCat/` - Category of algebras over rings (complete)
- [x] `AlgebraCat/` - Deprecated re-exports for symmetric monoidal structure on algebras (complete)
- [x] `BialgCat/` - Category of bialgebras (complete)
- [x] `CoalgCat/` - Category of coalgebras (complete)
- [x] `CommAlgCat/` - Category of commutative algebras (complete)
- [x] `ContinuousCohomology/` - Continuous cohomology categorical framework (complete)
- [x] `FGModuleCat/` - Category of finitely generated modules (complete)
- [x] `Grp/` - Category of groups and related group-theoretic categories (complete)
- [x] `HopfAlgCat/` - Category of Hopf algebras (complete)
- [~] `ModuleCat/` - Category of modules over rings (preliminary)
- [ ] `MonCat/` - Category of monoids (pending)
- [ ] `Ring/` - Category of rings and related categories (semirings, commutative rings, etc.) (pending)
- [ ] `Semigrp/` - Category of semigroups (pending)

## Search Tags

category-theory algebra categorical-algebra bundled-categories groups rings modules algebras bialgebras coalgebras hopf-algebras boolean-rings forgetful-functors categorical-equivalences monads concrete-categories morphisms
