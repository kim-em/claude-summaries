---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Fourier
generated: 2025-12-05T13:15:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 10
subdirs_count: 1
---

# Fourier

## Overview

The `Fourier/` directory contains a comprehensive formalization of Fourier analysis across continuous, discrete, and finite settings. For continuous spaces, it develops Fourier transforms on finite-dimensional real vector spaces with respect to unitary additive characters and bilinear pairings, proving the Riemann-Lebesgue lemma (Fourier transforms vanish at infinity), the Fourier inversion theorem, Poisson's summation formula, and properties of derivatives of Fourier transforms. For periodic settings, it formalizes Fourier series on the additive circle `ℝ / ℤ • T` with Haar measure, proving density of Fourier monomials in L² spaces and uniform convergence results for continuous functions. For discrete settings, it covers discrete Fourier transforms on `ZMod N` with standard additive characters. The `FiniteAbelian/` subdirectory extends the theory to arbitrary finite abelian groups, establishing orthogonality of characters, Pontryagin duality (isomorphism between a finite abelian group and its double dual), and character-theoretic bases for function spaces.

## Key Files

| File | Purpose |
|------|---------|
| AddCircle.lean | Fourier series on the additive circle `ℝ / ℤ • T`; defines Haar measure, Fourier monomials, Fourier coefficients, and proves density of Fourier basis in L² spaces |
| AddCircleMulti.lean | Multivariate Fourier series on the d-dimensional unit circle; proves L² convergence and uniform convergence for continuous functions with summable Fourier coefficients |
| BoundedContinuousFunctionChar.lean | Defines bounded continuous character functions `char he hL w = fun v ↦ e (L v w)` for additive characters and bilinear maps; used for characteristic functions of measures |
| FourierTransform.lean | General Fourier transform theory for functions on finite-dimensional spaces; defines `fourierIntegral` with respect to bilinear pairings and unitary additive characters |
| FourierTransformDeriv.lean | Derivatives of Fourier transforms; proves Fourier transform is C^n if `‖v‖^n * ‖f v‖` is integrable; includes Fourier transform of derivatives |
| Inversion.lean | Fourier inversion formula `𝓕⁻ (𝓕 f) v = f v` for integrable functions on finite-dimensional real inner product spaces |
| Notation.lean | Type classes and notation for Fourier transforms; defines `𝓕` for Fourier transform and `𝓕⁻` for inverse Fourier transform with module and inversion properties |
| PoissonSummation.lean | Poisson's summation formula `∑ (n : ℤ), f n = ∑ (n : ℤ), 𝓕 f n` under convergence and integrability hypotheses; includes versions for Schwartz functions |
| RiemannLebesgueLemma.lean | Riemann-Lebesgue lemma: Fourier transform of L¹ functions tends to 0 along the cocompact filter on finite-dimensional real vector spaces |
| ZMod.lean | Discrete Fourier transform on `ZMod N` with standard additive character; includes Fourier inversion and Fourier transforms of Dirichlet characters |

## Subdirectories

- [x] `FiniteAbelian/` - Fourier theory on finite abelian groups: orthogonality of characters, linear independence, Pontryagin duality, and character bases for function spaces

## Search Tags

fourier-analysis fourier-transform fourier-series fourier-inversion additive-circle riemann-lebesgue-lemma poisson-summation fourier-coefficients haar-measure discrete-fourier-transform zmod character-theory gaussian-fourier hilbert-basis l2-space convergence
