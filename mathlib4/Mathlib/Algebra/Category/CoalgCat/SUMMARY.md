---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/CoalgCat
generated: 2025-12-02T00:42:30Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# CoalgCat

## Overview

The `CoalgCat/` directory defines the category of coalgebras over a commutative ring `R`, along with its structure as a monoidal category and its equivalence with comonoid objects in the category of modules. It establishes coalgebras as a concrete category with morphisms given by coalgebra homomorphisms, provides a forgetful functor to `ModuleCat`, and proves that coalgebras form a monoidal category via tensor products with the same structure as the underlying modules.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines bundled category `CoalgCat R` of coalgebras over commutative ring `R` with morphisms as coalgebra homomorphisms; includes forgetful functor to `ModuleCat R`, conversion between categorical isomorphisms and coalgebra equivalences, and reflection of isomorphisms |
| ComonEquivalence.lean | Establishes category equivalence between `CoalgCat R` and `Comon(ModuleCat R)` (comonoid objects in R-modules); defines auxiliary monoidal structure transported from comonoid objects; proves compatibility of comultiplication and counit on tensor products with the standard coalgebra tensor product |
| Monoidal.lean | Defines the `MonoidalCategory` instance on `CoalgCat R` using tensor product of coalgebras as monoidal product; proves monoidal structure is induced from `ModuleCat R` via the forgetful functor with definitionally good equalities; includes associator, left/right unitors as coalgebra equivalences |

## Subdirectories

(none)

## Search Tags

coalgebras category-theory monoidal-categories comonoid-objects tensor-products categorical-equivalence modules forgetful-functors comultiplication counit coalgebra-homomorphisms concrete-categories isomorphism-reflection categorical-algebra
