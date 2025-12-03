---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/AlgCat
generated: 2025-12-02T20:15:00Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# AlgCat

## Overview

The `AlgCat/` directory defines the category of algebras over a commutative ring `R`, where objects are R-algebras and morphisms are algebra homomorphisms. It provides the complete categorical infrastructure including forgetful functors to `RingCat` and `ModuleCat`, the free algebra construction with its adjunction to the forgetful functor, all limits and their preservation properties, and a monoidal (symmetric) category structure using tensor products of algebras.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines the bundled category `AlgCat R` with objects as R-algebras and morphisms as algebra homomorphisms; includes forgetful functors to `RingCat` and `ModuleCat`, free algebra functor, and free/forget adjunction |
| Limits.lean | Proves that `AlgCat R` has all limits constructed from sections subalgebras, and that forgetful functors to rings, modules, and types preserve all limits |
| Monoidal.lean | Defines monoidal category structure on `AlgCat R` using tensor products of algebras, with tensor unit `R` and structural isomorphisms from tensor product associativity/unit laws |
| Symmetric.lean | Proves that the monoidal structure on `AlgCat R` is symmetric (and braided) using the commutativity of tensor products |

## Subdirectories

(none)

## Search Tags

category-theory algebras algebra-category R-algebras algebra-homomorphisms forgetful-functors free-algebra adjunction limits monoidal-category symmetric-category tensor-products braided-category concrete-category
