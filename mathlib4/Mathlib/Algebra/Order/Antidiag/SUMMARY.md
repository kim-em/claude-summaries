---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Antidiag
generated: 2025-12-01T19:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# Antidiag

## Overview

The `Antidiag/` folder provides infrastructure for working with "antidiagonals" in ordered algebraic contexts—finsets of tuples whose components sum (or multiply) to a fixed value. The core abstraction is the `HasAntidiagonal` typeclass defining `antidiagonal : A → Finset (A × A)` for pairs summing to a value. This generalizes to functions (`piAntidiag`), finitely supported functions (`finsuppAntidiag`), and specialized natural number multiplicative antidiagonals (`finMulAntidiag`), with applications to combinatorial counting problems like counting ways to factor squarefree integers.

## Key Files

| File | Purpose |
|------|---------|
| Prod.lean | Defines `HasAntidiagonal` typeclass for additive monoids with `antidiagonal : A → Finset (A × A)` where pairs sum to a value; provides `antidiagonalOfLocallyFinite` for canonically ordered monoids with locally finite order |
| Pi.lean | Antidiagonals in function spaces: defines `piAntidiag s n` (finset of functions `ι → μ` with support in `s` summing to `n`) and `finAntidiagonal d n` (efficient version for `Fin d → μ`); includes insertion/cons operations and natural number scalar multiplication results |
| Finsupp.lean | Antidiagonals for finitely supported functions: defines `finsuppAntidiag s n` (finset of `f : ι →₀ μ` with support in `s` and sum `n`) by mapping from `piAntidiag`; provides insertion decomposition and additive equivalence preservation |
| Nat.lean | Natural number multiplicative antidiagonals: defines `finMulAntidiag d n` (d-tuples of naturals with product n), proves `#(finMulAntidiag d n) = d^(ω n)` for squarefree n, and shows `#{(a,b) : lcm a b = n} = 3^(ω n)` for squarefree n using divisor-based constructions |

## Subdirectories

*(none)*

## Search Tags

antidiagonal finset tuples-summing-to-value ordered-monoid pi-antidiag finsupp-antidiag multiplicative-antidiagonal divisors squarefree-counting omega-function combinatorial-counting lcm-pairs fintype-pi canonical-order locally-finite
