---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Polynomial
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# Polynomial

## Overview

The `Polynomial/` directory contains analytical results about polynomials over normed fields, including asymptotic behavior, bounds on roots, factorization properties over specific fields, and Mahler measure theory. It bridges algebraic polynomial theory with analysis through limits, norms, and integration on the complex unit circle.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Limits and asymptotic behavior of polynomial and rational functions; proves polynomials are asymptotically equivalent to their leading term at infinity, with applications to determining when polynomial quotients tend to zero, infinity, or constants |
| CauchyBound.lean | Cauchy's bound on polynomial roots (`1 + max (‖aᵢ‖ / ‖aₙ‖)`); proves that all roots of a polynomial lie within this bound from the origin |
| Factorization.lean | Factorization properties of monic polynomials of given degree over algebraically closed fields and ℝ; shows monic polynomials can be factored into linear factors (over algebraically closed fields) or degree-1/2 factors (over ℝ) |
| MahlerMeasure.lean | Mahler measure of complex polynomials, defined as the exponential of the circle average of `log ‖p(e^(ix))‖`; proves the measure equals the leading coefficient times the product of root norms outside the unit disk, with multiplicativity and coefficient bounds |

## Subdirectories

(none)

## Search Tags

polynomial analysis asymptotic-behavior limits rational-functions leading-coefficient cauchy-bound root-bounds factorization monic-polynomials algebraically-closed real-closed mahler-measure circle-integration complex-polynomials norm-estimates coefficient-bounds
