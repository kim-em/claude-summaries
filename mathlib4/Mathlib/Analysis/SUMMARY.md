---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: preliminary
files_count: 18
subdirs_count: 24
---

# Analysis

## Overview

The `Analysis/` directory contains the formalization of real and complex analysis, including calculus, measure theory, functional analysis, and specialized analytical topics. It covers core concepts like bounded variation, seminorms, convolution, mean inequalities (AM-GM, Hölder, Minkowski), convergence of p-series, and constant-speed parameterizations. The directory is organized into major subdirectories for analytic functions, asymptotic analysis, calculus, complex analysis, convex analysis, normed spaces, special functions, and more specialized topics like C*-algebras, ODE theory, and Von Neumann algebras.

## Key Files

| File | Purpose |
|------|---------|
| BoundedVariation.lean | Almost everywhere differentiability of functions with locally bounded variation; proves that bounded variation and Lipschitz functions from ℝ to finite-dimensional vector spaces are differentiable almost everywhere |
| Seminorm.lean | Defines seminorms (positive-semidefinite, absolutely homogeneous, and subadditive functions to reals); closely related to convex sets and locally convex topological vector spaces |
| Convolution.lean | Defines convolution of functions `x ↦ ∫ f(t)g(x - t) ∂t` with vector-valued functions over additive groups with Haar measure; includes existence conditions and properties for functions with compact support |
| MeanInequalities.lean | Proves mean value inequalities for finite sums including weighted AM-GM, HM-GM, Young's inequality, Hölder inequality, and Minkowski inequality |
| MeanInequalitiesPow.lean | Power-specific versions of mean inequalities |
| PSeries.lean | Convergence of p-series `∑' k in ℕ, 1 / k ^ p` (converges iff p > 1); proves Schlömilch's generalization of the Cauchy condensation test |
| PSeriesComplex.lean | Complex version of p-series convergence |
| ConstantSpeed.lean | Defines constant and unit speed for functions `f : ℝ → E`; shows that functions with locally bounded variation can be reparameterized to unit speed via `naturalParameterization` |
| Hofer.lean | Hofer's lemma about complete metric spaces, motivated by bubbling-off analysis for holomorphic curves in symplectic topology |
| Oscillation.lean | Oscillation of functions (supremum of differences over neighborhoods) |
| Quaternion.lean | Analysis on quaternions |
| LConvolution.lean | L-convolution (alternative convolution definition) |
| MellinTransform.lean | Mellin transform (integral transform related to Fourier and Laplace transforms) |
| MellinInversion.lean | Mellin inversion theorem |
| Subadditive.lean | Subadditive functions and their properties |
| SumIntegralComparisons.lean | Comparisons between sums and integrals (integral test for series convergence) |
| SumOverResidueClass.lean | Summation over residue classes |
| Matrix.lean | Import file for matrix analysis subdirectory |

## Subdirectories

- [x] `AbsoluteValue/` - Absolute value functions and their analytical properties (complete)
- [x] `Analytic/` - Analytic functions (functions with power series expansions in normed spaces) (complete)
- [x] `Asymptotics/` - Asymptotic analysis (big-O notation, asymptotic equivalence, growth rates) (complete)
- [x] `BoxIntegral/` - Box integrals (Henstock-Kurzweil integration theory) (complete)
- [x] `CStarAlgebra/` - C*-algebras (Banach *-algebras with C* identity) and their analysis (complete)
- [x] `Calculus/` - Differential and integral calculus (derivatives, integrals, fundamental theorem) (complete)
- [x] `Complex/` - Complex analysis (holomorphic functions, Cauchy's theorem, residues) (complete)
- [x] `Convex/` - Convex analysis (convex functions, convex sets, Jensen's inequality) (complete)
- [x] `Distribution/` - Distribution theory (generalized functions, Schwartz distributions) (complete)
- [x] `Fourier/` - Fourier analysis (Fourier transforms, Fourier series, Poisson summation, Riemann-Lebesgue lemma, finite abelian group characters) (complete)
- [x] `FunctionalSpaces/` - Gagliardo-Nirenberg-Sobolev inequality for bounding Lᵖ norms of compactly-supported C¹ functions by norms of their derivatives (complete)
- [x] `InnerProductSpace/` - Inner product spaces (Hilbert spaces, orthogonality, projections) (complete)
- [x] `LocallyConvex/` - Locally convex topological vector spaces (seminorms, absorbent/balanced/absolutely convex sets, von Neumann boundedness, weak topologies, separation theorems, barrelled and Montel spaces) (complete)
- [x] `Matrix/` - Matrix analysis (matrix norms, matrix functions, spectral theory) (complete)
- [x] `Meromorphic/` - Meromorphic functions (functions holomorphic except at isolated poles) (complete)
- [x] `Normed/` - Normed spaces basics (complete)
- [x] `NormedSpace/` - Deprecated import layer for backward compatibility; forwards to reorganized `Mathlib.Analysis.Normed.*` hierarchy (complete)
- [x] `ODE/` - Ordinary differential equations (Grönwall's inequality, Picard-Lindelöf theorem for existence and uniqueness of solutions to initial value problems) (complete)
- [x] `Polynomial/` - Analysis on polynomials (asymptotic behavior, Cauchy root bounds, factorization, Mahler measure) (complete)
- [x] `RCLike/` - Abstraction over ℝ and ℂ (real and complex numbers treated uniformly) (complete)
- [x] `Real/` - Real analysis (properties specific to real numbers) (complete)
- [x] `SpecialFunctions/` - Special functions (exponential, logarithm, trigonometric, gamma, zeta, etc.) (complete)
- [x] `SpecificLimits/` - Specific limit computations and convergence results (includes arithmetic-geometric mean, Fibonacci limits, floor power limits, normed space limits) (complete)
- [ ] `VonNeumannAlgebra/` - Von Neumann algebras (weakly closed *-subalgebras of bounded operators) (pending)

## Search Tags

analysis real-analysis complex-analysis calculus measure-theory functional-analysis normed-spaces hilbert-spaces banach-spaces seminorms convolution mean-inequalities bounded-variation p-series fourier-analysis special-functions ode differential-equations integral-equations asymptotic-analysis convex-analysis cstar-algebras von-neumann-algebras distributions meromorphic holomorphic analytic-functions
