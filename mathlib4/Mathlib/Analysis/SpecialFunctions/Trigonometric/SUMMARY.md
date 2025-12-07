---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/Trigonometric
generated: 2025-12-07T08:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 15
subdirs_count: 0
---

# Trigonometric

## Overview

The `Trigonometric/` directory contains comprehensive formalization of trigonometric and inverse trigonometric functions for both real and complex arguments. It provides core definitions (including π), basic properties, continuity, differentiability results, bounds and inequalities, series representations, product formulas, and specialized applications. The directory covers standard functions (sin, cos, tan, arcsin, arccos, arctan, cot), the Real.Angle quotient type (ℝ/2πℤ), Chebyshev polynomial characterizations of multiple angle formulas, Euler's infinite product for sine, the Mittag-Leffler expansion for cotangent, and the sinc function. Special attention is given to analytical properties: derivatives (strict and ordinary), asymptotic behavior, polynomial bounds, and relationships between real and complex versions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and properties of trigonometric functions; defines π; establishes basic inequalities, continuity, and periodicity for real trig functions |
| Deriv.lean | Differentiability of all standard trigonometric functions (sin, cos, tan, sinh, cosh, tanh); computes derivatives and establishes strict differentiability |
| Complex.lean | Complex trigonometric functions; proves when cos/sin equal zero, periodicity, and relationships between complex and real trig functions |
| ComplexDeriv.lean | Derivatives of complex trigonometric functions; proves tan has derivative 1/cos²x and establishes asymptotic behavior when cos = 0 |
| Angle.lean | Defines Real.Angle as quotient type ℝ/2πℤ; establishes trigonometric functions on angles, circular order, and relationships with ℝ |
| Arctan.lean | Arctan function with addition formulas (arctan_add); tan as OpenPartialHomeomorph between (-π/2, π/2) and ℝ; includes Machin-like formulas for π/4 |
| ArctanDeriv.lean | Derivatives and continuity of tan and arctan functions; establishes when tan is continuous (cos x ≠ 0) and computes derivatives |
| Inverse.lean | Inverse trigonometric functions arcsin, arccos with range specifications; proves basic properties and relationships with forward functions |
| InverseDeriv.lean | Derivatives of arcsin and arccos; computes derivatives (e.g., arcsin' x = 1/√(1-x²)) with appropriate domain restrictions |
| Bounds.lean | Polynomial bounds for trigonometric functions; proves sin x < x for x > 0, x < tan x for 0 < x < π/2, and cos x bounds involving √(x²+1) |
| Chebyshev.lean | Multiple angle formulas for cos and cosh in terms of Chebyshev polynomials; relates trig functions to polynomial evaluations |
| Cotangent.lean | Cotangent function with series expansions; proves geometric series and Mittag-Leffler expansion π·cot(πz) = 1/z + Σ(1/(z-n) + 1/(z+n)) |
| EulerSineProd.lean | Euler's infinite product formula for sine: sin(πz) = πz·∏(1 - z²/n²); proof via integral recursion generalizing Wallis' formula |
| Series.lean | Trigonometric functions as infinite series; proves cos and sin can be expressed as power series with explicit summability results |
| Sinc.lean | Sinc function (sin x / x with sinc 0 = 1); proves continuity and basic properties using differential slope characterization |

## Subdirectories

None.

## Search Tags

trigonometric sine cosine tangent arcsin arccos arctan cotangent hyperbolic sinh cosh tanh angle pi derivatives differentiability continuity complex-trigonometry inverse-trig bounds inequalities polynomial-bounds chebyshev-polynomials euler-product mittag-leffler series-expansion sinc machin-formula wallis-formula real-angle quotient-type periodic-functions multiple-angle-formulas asymptotic-behavior strict-derivatives product-formulas
