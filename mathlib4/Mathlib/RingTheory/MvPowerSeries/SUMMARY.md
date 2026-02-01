---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/MvPowerSeries
generated: 2026-02-01T09:15:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 11
subdirs_count: 0
---

# MvPowerSeries

## Overview

The `MvPowerSeries/` directory contains the formalization of multivariate formal power series and their properties. Multivariate power series generalize polynomials to infinite sums, defined as `MvPowerSeries σ R := (σ →₀ ℕ) → R` where `σ` indexes the variables and `R` is the coefficient ring. This folder provides the ring structure (semiring, ring, commutative ring), coefficient extraction, monomials, constant terms, multiplicative inverses over fields and local rings, order/weighted order theory, truncation to polynomials, evaluation and substitution of power series, topology (product/Pi topology and linear topology), and the absence of zero divisors when the base ring has none.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `MvPowerSeries σ R`, `coeff`, `monomial`, `C` (constants), `X` (variables), `constantCoeff`; ring structure; multiplication via antidiagonal sums; `map` for coefficient change; coercion from `MvPolynomial` |
| Inverse.lean | Multiplicative inverses: `invOfUnit` for invertible constant coefficient, `inv` over fields; proves power series over local rings form local rings |
| Order.lean | Weighted order and order (degree) of power series; vanishing of low-degree coefficients; homogeneous components; order bounds for sums and products |
| Trunc.lean | Truncation to polynomials: `trunc` (strict inequality) and `trunc'` (inclusive); relationship between truncations and products |
| Evaluation.lean | Evaluation of power series at topologically nilpotent elements; `eval₂`, `eval₂Hom`, `aeval` as ring/algebra morphisms; requires linear topology on target |
| Substitution.lean | Substitution of power series into power series: `subst`, `substAlgHom`; `HasSubst` condition for nilpotent constant coefficients; `rescale` for variable scaling |
| Expand.lean | Expansion: replace `X i` by `X i ^ p`; algebra homomorphism `expand`; interaction with Frobenius in characteristic p |
| LexOrder.lean | Lexicographic order valuation using well-founded recursion on exponents; `lexOrder` as element of `WithTop (Lex (σ →₀ ℕ))` |
| LinearTopology.lean | Linear topology on power series when base ring has linear topology; basis of neighborhoods as two-sided ideals; topological nilpotency characterization |
| NoZeroDivisors.lean | Proves `NoZeroDivisors` instance when base ring has none; non-zero-divisor criteria via constant coefficient; multiplicativity of order |
| PiTopology.lean | Product (Pi) topology on power series; continuity of coefficients and operations; completeness; summability and multipliability of families; geometric series formula |

## Subdirectories

(none)

## Search Tags

power-series formal-power-series multivariate MvPowerSeries coefficient monomial constant-coefficient inverse invOfUnit local-ring order weighted-order truncation evaluation substitution subst rescale expand Frobenius lexicographic-order topology product-topology linear-topology complete no-zero-divisors summable multipliable geometric-series
