---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Fourier
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 10
subdirs_count: 1
---

# Fourier

## Overview

The `Fourier/` directory contains the formalization of Fourier analysis, including Fourier transforms, Fourier series, and the Fourier inversion theorem. It covers both continuous Fourier transforms on finite-dimensional real vector spaces and discrete Fourier transforms on `ZMod N`. The directory includes fundamental results like the Riemann-Lebesgue lemma (Fourier transforms vanish at infinity), Poisson's summation formula, properties of derivatives of Fourier transforms, and convergence of Fourier series on the additive circle `ℝ / ℤ • T`.

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

- [ ] `FiniteAbelian/` - Fourier theory on finite abelian groups (pending)

## Search Tags

fourier-analysis fourier-transform fourier-series fourier-inversion additive-circle riemann-lebesgue-lemma poisson-summation fourier-coefficients haar-measure discrete-fourier-transform zmod character-theory gaussian-fourier hilbert-basis l2-space convergence
