---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry/EllipticCurve/DivisionPolynomial
generated: 2025-12-04T18:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# DivisionPolynomial

## Overview

The `DivisionPolynomial/` directory provides a formalization of division polynomials for Weierstrass elliptic curves. Division polynomials are polynomials whose roots correspond to the x-coordinates of n-torsion points on an elliptic curve. The directory defines both univariate and bivariate forms of these polynomials (`preΨₙ`, `ΨSqₙ`, `Ψₙ`, `Φₙ`, `ψₙ`, `φₙ`) and establishes their fundamental properties including recursive definitions via elliptic divisibility sequences, their degrees, and leading coefficients.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines division polynomials for Weierstrass curves as normalized elliptic divisibility sequences (EDS): the bivariate n-division polynomials `ψₙ ∈ R[X, Y]`, the univariate auxiliary polynomials `preΨₙ ∈ R[X]` (avoiding division in the ring), the bivariate polynomials `Ψₙ` congruent to `ψₙ` in the coordinate ring, the univariate polynomials `ΨSqₙ` and `Φₙ` congruent to `ψₙ²` and `φₙ`, and the associated polynomials `φₙ ∈ R[X][Y]`; includes recursive formulas for even and odd indices, congruence relations in the coordinate ring, and mapping properties across ring homomorphisms and base changes |
| Degree.lean | Computes leading terms and degrees of division polynomials: proves that `preΨₙ` has degree `(n² - 4)/2` with leading coefficient `n/2` when n is even, degree `(n² - 1)/2` with leading coefficient `n` when n is odd; proves `ΨSqₙ` has degree `n² - 1` with leading coefficient `n²`; proves `Φₙ` has degree `n²` with leading coefficient `1`; establishes these results over integral domains of characteristic not dividing n using strong induction on the recursive EDS formulas |

## Subdirectories

(none)

## Search Tags

elliptic-curves division-polynomials torsion-points weierstrass-equations elliptic-divisibility-sequences polynomial-degree leading-coefficients univariate-polynomials bivariate-polynomials coordinate-ring algebraic-geometry number-theory
