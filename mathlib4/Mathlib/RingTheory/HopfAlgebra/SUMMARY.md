---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/HopfAlgebra
generated: 2026-01-26T19:35:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# HopfAlgebra

## Overview

This directory contains the formalization of Hopf algebras over commutative semirings. A Hopf algebra is a bialgebra equipped with an antipode (an R-linear endomorphism satisfying specific axioms). The theory includes: basic definitions and axioms for Hopf algebras; the group structure on group-like elements (elements whose comultiplication equals their tensor square); natural instances showing that commutative semirings, group algebras (monoid algebras over groups), and tensor products of Hopf algebras are themselves Hopf algebras; and the instance on Laurent polynomials which corresponds to the multiplicative group scheme 𝔾ₘ/R in algebraic geometry.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `HopfAlgebra` class and `antipode` map; axioms relating antipode, comultiplication, and counit; basic properties like `antipode 1 = 1` and `counit ∘ antipode = counit`; instance showing every commutative semiring is a Hopf algebra over itself with identity antipode |
| GroupLike.lean | Proves that group-like elements in a Hopf algebra form a group; shows antipode acts as inverse for group-like elements; includes `GroupLike.toUnits` converting group-like elements to units; proves commutativity when ambient algebra is commutative |
| MonoidAlgebra.lean | Hopf algebra structure on group algebras A[G] when A is a Hopf algebra and G is a group; defines antipode on `single g a` as `single g⁻¹ (antipode a)`; includes Laurent polynomial instance A[T;T⁻¹] where antipode sends T^n to T^(-n) |
| TensorProduct.lean | Hopf algebra structure on tensor products B ⊗[R] A when both are Hopf algebras; antipode is defined as `AlgebraTensorModule.map` of the component antipodes; includes helper `HopfAlgebra.ofAlgHom` for constructing Hopf algebras from algebra homomorphisms |

## Subdirectories

(none)

## Search Tags

Hopf-algebra antipode bialgebra coalgebra comultiplication counit group-like-elements monoid-algebra group-algebra Laurent-polynomial tensor-product algebraic-structures categorical-algebra quantum-groups group-schemes
