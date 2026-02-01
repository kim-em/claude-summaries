---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/PowerSeries
generated: 2026-02-01T03:12:25Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 20
subdirs_count: 0
---

# PowerSeries

## Overview

This folder develops the theory of univariate formal power series `R⟦X⟧` over a commutative (semi)ring `R`. Power series are defined as the special case of multivariate power series `MvPowerSeries Unit R`. The folder covers foundational operations (coefficients, truncation, order), algebraic structure (ideals, no zero divisors, invertibility), calculus-like operations (derivative, evaluation, substitution), well-known series (exp, sin, cos, binomial, Catalan, Schröder), and advanced topics including the Weierstrass preparation theorem for complete local rings.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `R⟦X⟧` as `MvPowerSeries Unit R`, coefficient extraction, `X`, `C`, monomial, polynomial coercion, rescaling |
| Order.lean | Order of a power series (lowest nonzero coefficient index), properties for multiplication, addition |
| Trunc.lean | Truncation `trunc n φ` to polynomial with same coefficients below `n`, used in many computations |
| Inverse.lean | Multiplicative inverses for series with unit constant coefficient, `invOfUnit`, division |
| Derivative.lean | Formal differentiation as a derivation, Leibniz rule, uniqueness of series by derivative and constant term |
| Evaluation.lean | Evaluation `eval₂ φ a f` at topologically nilpotent elements in complete algebras |
| Substitution.lean | Substitution of power series with nilpotent constant coefficient into another series |
| Expand.lean | Expansion `expand p φ` replacing `X` by `X^p`, useful for studying `p`-adic properties |
| WellKnown.lean | `invUnitsSub u` for `1/(u-X)`, `invOneSubPow d` for `(1-X)^(-d)`, `sin`, `cos` series |
| Exp.lean | Exponential series `exp A = Σ Xⁿ/n!`, differential equation `exp' = exp`, functional equations |
| Binomial.lean | Binomial series `(1+X)^r` for elements in binomial rings, including negative integer exponents |
| Catalan.lean | Catalan generating function satisfying `C = 1 + X·C²` |
| Schroder.lean | Large Schröder numbers power series satisfying `S = 1 + X·S + X·S²` |
| NoZeroDivisors.lean | `R⟦X⟧` is a domain when `R` is, `X` is prime and irreducible |
| Ideal.lean | Prime ideal structure in `R⟦X⟧`, noetherianity when `R` is noetherian, UFD when `R` is a PID |
| GaussNorm.lean | Gauss norm for power series: `sup_i ‖coeff_i f‖ · c^i` |
| Restricted.lean | Restricted power series where `‖coeff_i f‖ · c^i → 0`, closure under operations in ultrametric setting |
| CoeffMulMem.lean | Coefficient ideal membership for products: if coefficients are in ideals `I`, `J`, product coefficients are in `I·J` |
| PiTopology.lean | Product topology on power series (coefficientwise convergence), completeness, topological nilpotence |
| WeierstrassPreparation.lean | Weierstrass division and preparation theorem for complete local rings: factorization into distinguished polynomial times unit |

## Subdirectories

(none)

## Search Tags

power-series formal-power-series univariate-power-series coefficients truncation order derivative evaluation substitution exp exponential sin cos binomial catalan schroder inverse weierstrass-preparation complete-local-ring noetherian UFD ideal prime gauss-norm restricted topology

