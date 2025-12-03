---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/BialgCat
generated: 2025-12-02T18:30:00Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# BialgCat

## Overview

The `BialgCat/` directory defines the bundled category of bialgebras over a commutative ring `R`, where objects are `R`-bialgebras and morphisms are bialgebra homomorphisms (`BialgHom`). It provides the categorical infrastructure including forgetful functors to both `AlgCat` (algebras) and `CoalgCat` (coalgebras), reflecting the dual algebraic-coalgebraic nature of bialgebras. The directory also equips `BialgCat R` with a monoidal category structure using tensor products of bialgebras.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `BialgCat R` category structure with objects as `R`-bialgebras, morphisms as bialgebra homomorphisms; includes forgetful functors to `AlgCat R` and `CoalgCat R`, and establishes equivalence between categorical isomorphisms and `BialgEquiv` |
| Monoidal.lean | Equips `BialgCat R` with monoidal category structure where tensor product is `A ⊗[R] B`, induced from the monoidal structure on `AlgCat R`; makes both forgetful functors to `AlgCat R` and `CoalgCat R` monoidal |

## Subdirectories

None.

## Search Tags

category-theory bialgebras categorical-algebra bundled-categories tensor-products monoidal-categories forgetful-functors coalgebras algebras bialgebra-homomorphisms BialgCat BialgHom BialgEquiv
