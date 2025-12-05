---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Complex/Polynomial
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# Polynomial

## Overview

This folder contains fundamental theorems about complex polynomials, most notably the Fundamental Theorem of Algebra proving that every nonconstant complex polynomial has a root. It establishes that ℂ is algebraically closed and provides Galois-theoretic results about rational polynomials with specified numbers of non-real roots. Additional results include the Gauss-Lucas theorem on the location of polynomial derivative roots and irreducibility criteria for unit trinomials.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Fundamental Theorem of Algebra proving every nonconstant complex polynomial has a root, establishing ℂ as algebraically closed; algebraic extensions of ℝ are isomorphic to ℝ or ℂ; Galois group results for ℚ-polynomials with specific counts of non-real roots; irreducibility criteria for real polynomials (degree ≤ 2) |
| GaussLucas.lean | Gauss-Lucas Theorem: roots of polynomial derivatives lie in the convex hull of the original polynomial's roots; provides explicit convex combination weights via `derivRootWeight` |
| UnitTrinomial.lean | Irreducibility criterion for unit trinomials (polynomials with three terms, all coefficients ±1) based on having no common complex roots with their mirror polynomial |

## Subdirectories

(none)

## Search Tags

fundamental-theorem-of-algebra algebraically-closed complex-polynomial polynomial-roots gauss-lucas-theorem derivative-roots convex-hull liouville-theorem galois-group rational-polynomial irreducible-polynomial unit-trinomial real-polynomial quadratic-polynomial polynomial-degree polynomial-splitting-field algebraic-extension isalg-closed
