---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 21
subdirs_count: 10
---

# SpecialFunctions

## Overview

The `SpecialFunctions/` directory contains formalized theory for important mathematical special functions, including exponential, logarithmic, trigonometric, power, gamma, hypergeometric, and various other classical functions. It provides core definitions, analytical properties (continuity, differentiability, analyticity), asymptotic behavior, integrability results, and specific evaluations. The directory covers fundamental functions like exp/log/sqrt, inverse hyperbolic functions (arsinh), smooth approximation tools (Bernstein polynomials, sigmoid, smooth transitions), coordinate transformations (polar coordinates), combinatorial functions (binomial coefficients, Pochhammer, Stirling's formula), and information-theoretic functions (binary/q-ary entropy). Special attention is given to properties needed for analysis: derivatives, limits, bounds, growth comparisons, and improper integrals.

## Key Files

| File | Purpose |
|------|---------|
| Exp.lean | Continuity and basic properties of complex and real exponential functions; Lipschitz bounds and limits at infinity |
| ExpDeriv.lean | Derivatives of exponential functions in Banach algebras; Fréchet derivatives for exp in commutative and non-commutative settings |
| Exponential.lean | Calculus results on exponential map in Banach algebras; strict derivatives at zero and arbitrary points |
| Sqrt.lean | Smoothness (infinite differentiability) of Real.sqrt at all points x ≠ 0; uses local homeomorphism between (0,∞) and (0,∞) via squaring |
| Arsinh.lean | Inverse hyperbolic sine function; proves sinh is bijective with continuous, differentiable, and smooth inverse arsinh |
| Bernstein.lean | Bernstein polynomial approximations and Weierstrass approximation theorem; proves uniform convergence of Bernstein approximations to continuous functions on [0,1] |
| BinaryEntropy.lean | Shannon binary entropy function and q-ary entropy; continuity, differentiability, and convexity properties for information theory |
| Sigmoid.lean | Sigmoid function (1 + exp(-x))⁻¹ and its properties; includes order/topological/measurable embeddings from ℝ to [0,1] |
| JapaneseBracket.lean | Japanese bracket (1 + ‖x‖²)^(1/2) bounds and integrability; shows (1 + ‖x‖²)^(-r/2) is integrable when r exceeds dimension |
| Stirling.lean | Stirling's formula for factorial growth: n! ~ √(2πn)(n/e)^n; includes proof using logarithms and Wallis' product for π |
| Pochhammer.lean | Analysis of Pochhammer polynomials (falling factorials); differentiability, convexity, and Jensen's inequality applications |
| PolarCoord.lean | Polar coordinate transformation as open partial homeomorphism; change of variables formula for integrals in polar coordinates |
| CompareExp.lean | Growth comparison estimates for complex exponentials and powers; asymptotic analysis for z^a * e^(bz) as Re(z) → ∞ |
| ImproperIntegrals.lean | Evaluation of specific improper integrals over ℝ and half-infinite intervals; integrability results for various special functions |
| Choose.lean | Asymptotic behavior of binomial coefficients; proves n.choose k ~ n^k / k! and Θ(n^k) as n → ∞ |
| PolynomialExp.lean | Polynomials multiplied by exponentials; asymptotic and analytical properties |
| SmoothTransition.lean | Smooth transition functions (bump functions) for analysis; infinitely differentiable cutoff functions |
| NonIntegrable.lean | Examples and counterexamples for non-integrable functions; pathological cases in integration theory |
| OrdinaryHypergeometric.lean | Ordinary hypergeometric functions; series definitions and convergence properties |
| MulExpNegMulSq.lean | Functions of the form x ↦ x^n * exp(-a*x²); used in Gaussian integrals and probability |
| MulExpNegMulSqIntegral.lean | Integrals of x^n * exp(-a*x²); evaluations and recurrence relations |

## Subdirectories

- [x] `Complex/` - Complex-valued special functions (complete)
- [x] `ContinuousFunctionalCalculus/` - Continuous functional calculus for special functions (complete)
- [x] `Elliptic/` - Elliptic functions and elliptic integrals (complete)
- [x] `Gamma/` - Gamma function, beta function, and related special functions (complete)
- [x] `Gaussian/` - Gaussian integrals and Gaussian functions (complete)
- [x] `Integrability/` - Integrability results for special functions (complete)
- [x] `Integrals/` - Evaluations of integrals involving special functions (complete)
- [x] `Log/` - Logarithm function and its properties (complete)
- [x] `Pow/` - Power functions (x^y for real/complex x,y) and their properties (complete)
- [ ] `Trigonometric/` - Trigonometric and hyperbolic functions (sin, cos, tan, sinh, cosh, tanh, etc.) (pending)

## Search Tags

special-functions exponential logarithm trigonometric hyperbolic gamma elliptic hypergeometric sqrt power bernstein-polynomials weierstrass-approximation sigmoid entropy japanese-bracket stirling-formula pochhammer polar-coordinates binomial-coefficients factorial asymptotic-analysis gaussian-integrals smooth-transitions bump-functions improper-integrals integrability derivatives analyticity continuity complex-analysis real-analysis
