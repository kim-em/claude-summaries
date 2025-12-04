---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Azumaya
generated: 2025-12-04T18:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Azumaya

## Overview

The `Azumaya/` directory contains the formalization of Azumaya algebras, a class of noncommutative algebras that generalize central simple algebras over commutative rings. An Azumaya algebra over a commutative ring `R` is defined as a finitely generated, projective, and faithful R-algebra where the tensor product `A ⊗[R] Aᵐᵒᵖ` is isomorphic to the R-endomorphisms of A. The directory establishes foundational definitions, proves basic properties (including that R is Azumaya over itself and that the property is preserved under algebra isomorphisms), demonstrates that matrix algebras are Azumaya, and shows that Azumaya algebras are necessarily central algebras.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of Azumaya algebras via the `IsAzumaya` typeclass requiring finite generation, projectivity, faithfulness, and bijectivity of the canonical map `AlgHom.mulLeftRight : (A ⊗[R] Aᵐᵒᵖ) →ₐ[R] Module.End R A` sending `a ⊗ b ↦ (x ↦ a * x * b.unop)` |
| Basic.lean | Basic properties including `IsAzumaya.id` (R is Azumaya over itself), `IsAzumaya.of_AlgEquiv` (Azumaya property preserved under algebra isomorphisms), commutativity of mulLeftRight diagrams under conjugation, and proof that Azumaya algebras are central (center equals base ring image) |
| Matrix.lean | Proves that nontrivial matrix algebras `Matrix n n R` are Azumaya over commutative semiring R by constructing explicit inverse `AlgHom.mulLeftRightMatrix_inv` mapping endomorphism `f` to `∑ᵢₗₛₜ f(Eₛₜ)ᵢₗ • Eᵢₛ⊗Eₜₗ` and verifying bijectivity via basis calculations |

## Subdirectories

None

## Search Tags

azumaya-algebra central-algebra noncommutative-algebra brauer-group tensor-product bimodule projective-module faithful-module matrix-algebra central-simple-algebra morita-equivalence separable-algebra
