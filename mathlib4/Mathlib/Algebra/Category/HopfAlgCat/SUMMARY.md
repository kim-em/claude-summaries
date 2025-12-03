---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/HopfAlgCat
generated: 2025-12-02T08:23:00Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# HopfAlgCat

## Overview

The `HopfAlgCat/` directory defines the category of Hopf algebras over a commutative ring `R`. It introduces the bundled category with morphisms as bialgebra homomorphisms, along with a forgetful functor to `BialgCat` and a monoidal category structure. The implementation provides conversions between categorical isomorphisms and algebraic equivalences (`BialgEquiv`).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `HopfAlgCat R` as the category of Hopf algebras over commutative ring `R` with morphisms as bialgebra homomorphisms; includes forgetful functor to `BialgCat` and bidirectional conversions between categorical isomorphisms and `BialgEquiv` algebraic equivalences |
| Monoidal.lean | Establishes monoidal category structure on `HopfAlgCat R` using tensor products of Hopf algebras; defines tensor object, whisker operations, associator, and unitors; proves the forgetful functor to `BialgCat` is monoidal |

## Subdirectories

None.

## Search Tags

hopf-algebras category-theory categorical-algebra bialgebras monoidal-categories tensor-products forgetful-functors categorical-isomorphisms algebraic-equivalences bundled-categories
