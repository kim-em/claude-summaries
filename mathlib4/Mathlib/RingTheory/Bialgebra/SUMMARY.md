---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Bialgebra
generated: 2026-01-26T21:55:37Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# Bialgebra

## Overview

The `Bialgebra/` directory contains the formalization of bialgebras, which are algebraic structures that are simultaneously algebras and coalgebras with compatible structure maps. This includes the basic definition with counit and comultiplication as algebra morphisms, homomorphisms and equivalences between bialgebras, group-like elements (elements whose comultiplication is the pure tensor), and concrete instances including monoid algebras, Laurent polynomials, and tensor products of bialgebras.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core bialgebra definition as algebra with coalgebra structure where counit and comultiplication are algebra morphisms; includes alternative constructors, proves commutative semirings are bialgebras over themselves, shows bialgebras are nontrivial over nontrivial rings |
| Hom.lean | Bialgebra homomorphisms `A →ₐc[R] B` preserving both algebra and coalgebra structure; composition, identity, counit as bialgebra homomorphism, extensionality theorems |
| Equiv.lean | Bialgebra equivalences `A ≃ₐc[R] B` as invertible bialgebra homomorphisms; symmetry, transitivity, construction from bijective homomorphisms |
| GroupLike.lean | Group-like elements in bialgebras (elements with `comul a = a ⊗ a` and `counit a = 1`); proves they form a monoid/commutative monoid, stability under multiplication and inverses |
| MonoidAlgebra.lean | Bialgebra instance on monoid algebras `A[M]` when `A` is a bialgebra; includes `mapDomain` as bialgebra homomorphism, Laurent polynomial bialgebra structure |
| TensorProduct.lean | Bialgebra instance on tensor products `A ⊗[R] B`; tensor product of bialgebra homomorphisms, associator, left/right identity equivalences |

## Subdirectories

(none)

## Search Tags

bialgebra coalgebra algebra counit comultiplication group-like monoid-algebra Laurent-polynomial tensor-product homomorphism equivalence isomorphism Hopf-algebra
