---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Coalgebra
generated: 2026-01-26T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# Coalgebra

## Overview

The `Coalgebra/` directory contains the formalization of coalgebras, which are the categorical dual of algebras. A coalgebra over a commutative semiring `R` is an `R`-module equipped with a coassociative comultiplication `Δ : A → A ⊗[R] A` and a counit `ε : A → R` satisfying left and right counitality laws. This directory includes the basic definitions, homomorphisms and isomorphisms, tensor products, convolution products, group-like elements, and coalgebra structures on various constructions (products, finitely-supported functions, monoid algebras, and opposite algebras).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core coalgebra definitions: `CoalgebraStruct`, `Coalgebra` class with coassociativity and counitality axioms; coalgebra representations; instances for commutative semirings, products, finsupp, and pi types |
| Hom.lean | Coalgebra homomorphisms `A →ₗc[R] B`: linear maps preserving comultiplication and counit; includes `CoalgHom` structure and `CoalgHomClass` typeclass |
| Equiv.lean | Coalgebra isomorphisms `A ≃ₗc[R] B`: invertible coalgebra homomorphisms; defines `CoalgEquiv` structure and `CoalgEquivClass` typeclass |
| TensorProduct.lean | Tensor products of coalgebras: comultiplication and counit on `A ⊗[R] B` when `A` and `B` are coalgebras; monoidal structure including tensor products of coalgebra morphisms |
| Convolution.lean | Convolution product on linear maps `C → A` where `C` is a coalgebra and `A` an algebra: multiplication defined as `(f * g)(x) = ∑ f(x₍₁₎) * g(x₍₂₎)` in Sweedler notation |
| GroupLike.lean | Group-like elements in coalgebras: elements `a` satisfying `ε(a) = 1` and `Δ(a) = a ⊗ₜ a`; proves linear independence of group-like elements over domains |
| MonoidAlgebra.lean | Coalgebra structure on monoid algebras `A[X]` and Laurent polynomials `A[T;T⁻¹]` when `A` is an `R`-coalgebra; inherited from coalgebra structure on coefficients |
| MulOpposite.lean | Coalgebra structure on the opposite algebra `Aᵐᵒᵖ` when `A` is an `R`-coalgebra; defines comultiplication and counit via opposite linear equivalences |

## Subdirectories

(No subdirectories)

## Search Tags

coalgebra comultiplication counit coassociative counitality tensor-product dual-algebra Sweedler-notation coalgebra-homomorphism coalgebra-equivalence convolution-product group-like-elements monoid-algebra Laurent-polynomial opposite-algebra finsupp categorical-dual linear-map module representation
