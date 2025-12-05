---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Distribution
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 7
subdirs_count: 0
---

# Distribution

## Overview

This directory contains the foundational theory of distributions (generalized functions) and the Schwartz space in functional analysis. It defines Schwartz functions (smooth functions with rapidly decaying derivatives), test functions (smooth compactly supported functions), and establishes the topological and analytical machinery needed for distribution theory. The implementation includes temperate growth conditions, Fourier transforms on Schwartz spaces, and fundamental theorems connecting distributions to integration against test functions.

## Key Files

| File | Purpose |
|------|---------|
| SchwartzSpace.lean | Defines the Schwartz space `𝓢(E, F)` of smooth functions with rapidly decaying derivatives; constructs the locally convex topology via seminorms `‖x‖^k * ‖iteratedFDeriv ℝ n f x‖`; provides composition, differentiation, and integration as continuous linear maps |
| TestFunction.lean | Defines test functions `𝓓^{n}(Ω, F)` as bundled n-times continuously differentiable functions with compact support in an open set Ω; establishes the canonical LF topology (locally convex inductive limit); dual space gives distributions on Ω |
| ContDiffMapSupportedIn.lean | Defines `ContDiffMapSupportedIn E F n K` for n-times continuously differentiable functions vanishing outside compact set K; provides uniform convergence topology on functions and derivatives; building block for test function topology |
| FourierSchwartz.lean | Constructs Fourier transform as continuous linear map and continuous linear equivalence on Schwartz functions; shows Fourier transform preserves Schwartz space structure |
| TemperateGrowth.lean | Defines temperate growth for smooth functions (all iterated derivatives polynomially bounded); proves characterizations via big-O notation; used for composition with Schwartz functions |
| AEEqOfIntegralContDiff.lean | Proves that locally integrable functions with zero integral against all smooth compactly supported functions are almost everywhere zero; fundamental connection between distributions and functions on manifolds |
| DerivNotation.lean | Type classes and notation for line derivatives (partial derivatives): `∂_{v}` for directional derivative, `∂^{m}` for iterated derivatives; provides linear structure and continuity for derivative operators |

## Subdirectories

None.

## Search Tags

distribution-theory schwartz-space test-functions generalized-functions functional-analysis locally-convex fourier-transform temperate-growth compact-support smooth-functions continuous-differentiable seminorms topology line-derivatives partial-derivatives manifolds distributions-on-manifolds lf-topology inductive-limit
