---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/TensorProduct
generated: 2026-02-01T22:30:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: complete
files_count: 14
subdirs_count: 0
---

# TensorProduct

## Overview

The `TensorProduct/` directory provides comprehensive theory of tensor products of algebras and modules over commutative rings. It covers the algebraic structure on tensor products (multiplication, identity, structure isomorphisms), universal properties and lifting constructions, stability under base change, behavior with respect to direct limits and finite generation, interaction with quotients and products, and specialized results for polynomial algebras, monoid algebras, and free modules.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Fundamental algebra structure on `A ⊗[R] B` for R-algebras A and B; multiplication characterized by `(a₁ ⊗ₜ b₁) * (a₂ ⊗ₜ b₂) = (a₁ * a₂) ⊗ₜ (b₁ * b₂)`; base change lifting for linear maps |
| Maps.lean | Structure isomorphisms for tensor products: left/right unit laws (lid, rid), commutativity (comm), associativity (assoc); universal property liftEquiv; endomorphism algebra homomorphisms |
| Free.lean | Bases for tensor products: constructs basis for `A ⊗[R] M` from basis of M over R; proves freeness is stable under base change |
| Finite.lean | Finiteness properties: every element of `N ⊗ M` comes from finitely generated submodule; supremum of finitely generated subalgebras is finitely generated |
| DirectLimitFG.lean | Tensor products as direct limits of finitely generated submodules: `M ⊗[R] N` is direct limit of `P ⊗[R] N` for finitely generated P, and similarly for the other factor |
| MvPolynomial.lean | Tensor products of multivariate polynomial rings: linear equivalences between `MvPolynomial σ S ⊗[R] N` and `(σ →₀ ℕ) →₀ (S ⊗[R] N)`; algebra isomorphisms for polynomial base change |
| MonoidAlgebra.lean | Monoid algebras are stable under base change: algebra isomorphism `(A ⊗[R] B)[M] ≃ₐ[A] A ⊗[R] B[M]` showing monoid algebras commute with tensor products |
| Pi.lean | Tensor products commute with finite products: `A ⊗[R] (∀ i, B i) ≃ₐ[S] ∀ i, A ⊗[R] B i` when ι is finite; binary product variant and scalar product cases |
| Quotient.lean | Interaction of quotients with tensor products: `B ⧸ (I.map <| algebraMap A B) ≃ₐ[B] B ⊗[A] (A ⧸ I)` relating quotients by mapped ideals to tensoring with quotient algebras |
| Nontrivial.lean | Nontriviality results: if R injects into domains A and B, then `A ⊗[R] B` is nontrivial (uses fraction rings and faithfully flat theory) |
| IsBaseChangePi.lean | Base change commutes with products: proves `IsBaseChange` is preserved under binary products, finite products, and direct sums |
| IsBaseChangeFree.lean | Base change of free modules: constructs basis for base change of a module with a basis; proves freeness is preserved under base change using `IsBaseChange` interface |
| IsBaseChangeHom.lean | Base change for linear map modules: if M is finite free and P is base change of N, then `M →ₗ[R] P` is base change of `M →ₗ[R] N`; includes endomorphism module case |

## Subdirectories

*(none)*

## Search Tags

tensor-product algebra module base-change free-module finitely-generated direct-limit polynomial monoid-algebra quotient product pi-type universal-property structure-isomorphism lid rid comm assoc lift-equiv nontrivial fraction-ring IsBaseChange localization
