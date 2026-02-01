---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Polynomial/Cyclotomic
generated: 2026-02-01T00:00:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 5
subdirs_count: 0
---

# Cyclotomic

## Overview

The `Cyclotomic/` directory contains a comprehensive theory of cyclotomic polynomials, including both a modified version `cyclotomic'` (defined as the product over primitive roots in any integral domain) and the standard cyclotomic polynomial `cyclotomic` (with integer coefficients mapped to any ring). The directory establishes fundamental properties (degree equals Euler's totient φ(n), irreducibility over ℤ, identification as minimal polynomial of primitive roots), evaluations at special points (eval at 1 equals p for prime powers), behavior under polynomial expansion operations, factorization over finite fields, and characterizations of roots (primitive n-th roots of unity).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and properties: `cyclotomic'` (modified version as product over primitive roots), `cyclotomic` (standard version via integer coefficients), degree formulas (natDegree = totient n), monicity, product formula X^n - 1 = ∏ cyclotomic(d) over divisors, Möbius inversion, integer coefficient lifting, and irreducibility over ℤ via minimal polynomial identification |
| Roots.lean | Root characterization theorems: primitive n-th roots are exactly the roots of cyclotomic n (when NeZero n), cyclotomic n ℤ equals the minimal polynomial of any primitive root, irreducibility of cyclotomic over ℤ and ℚ, injectivity of n ↦ cyclotomic n, coprimality of distinct cyclotomic polynomials |
| Eval.lean | Evaluation results: eval 1 (cyclotomic p^k) = p for prime powers, eval 1 (cyclotomic n) = 1 otherwise, positivity theorem cyclotomic_pos for n > 2 over ordered rings, special evaluation at -1 |
| Expand.lean | Expand operation relationships: cyclotomic_expand theorems relating expand p (cyclotomic n) to cyclotomic (n*p) depending on divisibility, behavior in characteristic p (power formulas), explicit formula for cyclotomic 6 = X^2 - X + 1, irreducibility inheritance for prime powers |
| Factorization.lean | Factorization over finite fields: for finite field K of cardinality p^f with p coprime to n, irreducible factors of cyclotomic n have degree equal to the multiplicative order of p^f mod n, computation of the number of distinct irreducible factors as φ(n) / order(p^f mod n) |

## Subdirectories

(none)

## Search Tags

cyclotomic polynomial primitive-root roots-of-unity totient Euler-phi degree irreducible minimal-polynomial integer-coefficients Gauss Mobius-inversion evaluation expand characteristic-p finite-field factorization multiplicative-order primitive-root-of-unity X^n-1 divisor product Vieta complex algebraic-number-theory ring-theory field-theory Galois-theory
