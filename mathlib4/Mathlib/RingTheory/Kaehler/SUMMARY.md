---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Kaehler
generated: 2026-02-01T08:15:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 4
subdirs_count: 0
---

# Kaehler

## Overview

This directory contains the formalization of Kähler differentials (also written Kahler or Kaehler differentials) for commutative ring theory. Kähler differentials provide a module `Ω[S⁄R]` that represents the "universal derivation" from an R-algebra S, capturing the algebraic analogue of differential forms. The implementation defines `Ω[S⁄R]` as the cotangent space `I/I²` where `I` is the kernel of the multiplication map `S ⊗[R] S → S`, establishes the universal property relating linear maps from `Ω[S⁄R]` to derivations, and proves key exact sequences including the Jacobi-Zariski sequence for algebra towers `R → S → T`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory of Kähler differentials: defines `KaehlerDifferential R S` (notation `Ω[S⁄R]`), the universal derivation `D : S → Ω[S⁄R]`, the isomorphism `Hom(Ω[S⁄R], M) ≃ Der(S, M)`, presentation via generators and relations (`kerTotal`), finiteness results for essentially finite type algebras, and the fundamental exact sequences `B ⊗[A] Ω[A⁄R] → Ω[B⁄R] → Ω[B⁄A] → 0` and `I/I² → B ⊗[A] Ω[A⁄R] → Ω[B⁄R]` for surjective `A → B` |
| JacobiZariski.lean | The Jacobi-Zariski exact sequence for algebra towers `R → S → T`: proves `H¹(L_{T/R}) → H¹(L_{T/S}) → T ⊗[S] Ω[S/R] → Ω[T/R] → Ω[T/S] → 0` is exact, using snake lemma applied to a diagram involving cotangent complexes and presentations via generators |
| Polynomial.lean | Kähler differentials for polynomial algebras: proves `Ω[R[X]⁄R] ≃ R[X]` for univariate polynomials, `Ω[R[σ]⁄R] ≃ (σ →₀ R[σ])` for multivariate polynomials (free module on `{dXᵢ}`), and establishes the connection between the universal derivation and polynomial derivatives |
| TensorProduct.lean | Kähler differentials under base change: proves `Ω[B⁄S] ≃ S ⊗[R] Ω[A⁄R]` when `B = S ⊗[R] A` (pushout square), establishes that Kähler differentials commute with localization (`Ω[Aₚ/Rₚ]` is localization of `Ω[A/R]`), and provides both `S`-linear and `B`-linear versions of the base change isomorphism |

## Subdirectories

(none)

## Search Tags

Kaehler-differential Kahler-differential differential-forms derivation universal-derivation cotangent-space tensor-product exact-sequence Jacobi-Zariski base-change localization polynomial multivariate-polynomial module-of-differentials I-over-I-squared algebraic-geometry deformation-theory smoothness formally-smooth
