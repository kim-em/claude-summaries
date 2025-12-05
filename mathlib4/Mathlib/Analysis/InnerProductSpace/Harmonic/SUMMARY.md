---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/InnerProductSpace/Harmonic
generated: 2025-12-05T10:15:32Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# Harmonic

## Overview

This directory defines harmonic functions on real finite-dimensional inner product spaces and proves that complex-analytic functions are harmonic. A function is harmonic at a point if it is twice continuously differentiable and its Laplacian vanishes in a neighborhood. The theory includes vector space operations on harmonic functions, compatibility with linear maps, and constructions of harmonic functions from complex-analytic functions (including real/imaginary parts, conjugates, and logarithms of norms).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of harmonic functions (`HarmonicAt`, `HarmonicOnNhd`) and fundamental properties including vector space structure (sums, scalar multiples) and compatibility with continuous linear maps |
| Constructions.lean | Proves that complex-analytic functions are harmonic; shows real part, imaginary part, complex conjugate, and `log ‖f‖` of analytic functions are harmonic |
| Analytic.lean | Deprecated module that re-exports `Mathlib.Analysis.Complex.Harmonic.Analytic` (deprecated since 2025-09-16) |

## Subdirectories

(none)

## Search Tags

harmonic-functions laplacian inner-product-space complex-analysis analytic-functions partial-differential-equations pde continuously-differentiable real-inner-product-space vector-space-operations linear-maps logarithm-of-norm holomorphic-functions
