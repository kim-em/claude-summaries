---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/MvPolynomial/MonomialOrder
generated: 2026-02-01T21:45:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 1
subdirs_count: 0
---

# MonomialOrder

## Overview

This directory contains lemmas about the degree lexicographic (degLex) monomial order on multivariate polynomials. It connects the degLex ordering on Finsupp (from `Mathlib.Data.Finsupp.MonomialOrder.DegLex`) to MvPolynomial properties, particularly relating the degree of the leading monomial under degLex order to the total degree of the polynomial.

## Key Files

| File | Purpose |
|------|---------|
| DegLex.lean | Lemmas connecting degLex monomial order to MvPolynomial total degree: `degree_degLexDegree` (leading monomial's degree equals polynomial's total degree), `degLex_totalDegree_monotone` (degLex ordering implies total degree ordering) |

## Subdirectories

(none)

## Search Tags

monomial-order degLex degree-lexicographic total-degree leading-monomial multivariate-polynomial MvPolynomial Finsupp linear-order well-founded
