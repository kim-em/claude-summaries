---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/ContDiff
generated: 2025-12-04T08:45:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 11
subdirs_count: 0
---

# ContDiff

## Overview

The `ContDiff/` directory contains the formalization of continuously differentiable functions (C^n smoothness classes) in normed spaces. It provides the foundational definitions and theory for C^n functions, including the predicates `ContDiff`, `ContDiffOn`, `ContDiffAt`, and `ContDiffWithinAt` for various smoothness levels. The directory includes the core definition via formal Taylor series (`HasFTaylorSeriesUpTo`), composition results via Faà di Bruno's formula, operations preserving smoothness, quantitative bounds on iterated derivatives, and specialized results for finite-dimensional spaces, real/complex fields, polynomials, and different norm structures (WithLp).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of C^n smoothness: `ContDiff`, `ContDiffOn`, `ContDiffAt`, `ContDiffWithinAt` predicates; uses `HasFTaylorSeriesUpTo` to express existence of Taylor series up to rank n; includes detailed implementation notes on handling non-uniqueness of derivatives in general fields |
| FTaylorSeries.lean | Defines iterated Fréchet derivatives (`iteratedFDeriv`, `iteratedFDerivWithin`) and the predicate `HasFTaylorSeriesUpTo` that formalizes a sequence of multilinear maps as iterated derivatives of a function; includes infrastructure for working with n-multilinear maps and the "left composition" approach to handle universe polymorphism |
| Basic.lean | Proves that composition of C^n functions is C^n (`ContDiff.comp`); establishes basic properties like smoothness of constants and fundamental operations; builds on Faà di Bruno formula for composition |
| FaaDiBruno.lean | Implements Faà di Bruno's formula for the n-th derivative of a composition g ∘ f in terms of ordered finpartitions; defines `OrderedFinpartition`, `compAlongOrderedFinpartition`, and `taylorComp` to express iterated derivatives of compositions; proves `HasFTaylorSeriesUptoOn.comp` |
| Operations.lean | Proves that standard operations preserve C^n smoothness: addition, multiplication, Pi-types, bilinear operations, and inverse operations; includes smoothness preservation for functions to product spaces and dependent products |
| Bounds.lean | Establishes quantitative bounds on iterated derivatives; main result `norm_iteratedFDeriv_comp_le` bounds the n-th derivative of g ∘ f by `n! * C * D^n` when derivatives of g are bounded by C and i-th derivative of f is bounded by D^i; includes norm estimates for bilinear operations |
| RCLike.lean | Proves C^n smoothness results specific to ℝ and ℂ (fields satisfying `RCLike`); uses mean value theorem to show that `HasFTaylorSeriesUpToOn` with n ≥ 1 implies `HasStrictFDerivAt`; establishes strict differentiability for C^n functions |
| FiniteDimension.lean | Proves finite-dimensional specific results for C^n functions; main result: a family of continuous linear maps E →L[𝕜] F is C^n if and only if all point evaluations are C^n (uses finite rank to decompose via basis) |
| CPolynomial.lean | Proves that continuously polynomial functions (functions that are locally polynomial) are C^∞; shows `CPolynomialOn` implies `ContDiffOn` and `CPolynomialAt` implies `ContDiffAt`; establishes that continuous multilinear maps are C^∞ |
| RestrictScalars.lean | Establishes scalar restriction results for iterated Fréchet derivatives; proves that when restricting scalars from 𝕜' to 𝕜 ⊆ 𝕜', the n-th iterated derivative with respect to 𝕜 equals the scalar restriction of the n-th iterated derivative with respect to 𝕜'; analogous to results in FDeriv.RestrictScalars |
| WithLp.lean | Proves C^n smoothness results for functions involving `WithLp` (p-norm structures on products and Pi-types); establishes that `ContDiff(WithinAt/At/On) f` is equivalent to `ContDiff(WithinAt/At/On)` for each component; proves `PiLp.ofLp` and `PiLp.toLp` are C^∞ |

## Subdirectories

*(This directory contains no subdirectories)*

## Search Tags

continuously-differentiable smooth C^n higher-differentiability formal-taylor-series iterated-derivatives iterated-fderiv frechet-derivative has-ftaylor-series composition faa-di-bruno ordered-finpartition operations bounds quantitative-estimates rclike mean-value finite-dimensional cpolynomial multilinear-maps restrict-scalars withlp pilp normed-spaces smoothness-preservation
