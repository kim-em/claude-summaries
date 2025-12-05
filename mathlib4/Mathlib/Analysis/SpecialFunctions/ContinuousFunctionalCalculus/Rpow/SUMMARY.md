---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/ContinuousFunctionalCalculus/Rpow
generated: 2025-12-05T08:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# Rpow

## Overview

The `Rpow/` directory defines real powers and square roots via the continuous functional calculus (CFC) for C⋆-algebras and star-ordered rings. It provides both unital (`CFC.rpow`, implementing `a ^ y` for `y : ℝ`) and non-unital (`CFC.nnrpow`, implementing `a ^ y` for `y : ℝ≥0`) versions of real powers, as well as `CFC.sqrt` for square roots. The implementation includes comprehensive API for algebraic properties (composition, multiplication), norm characterizations for isometric CFC, integral representations of rpow for exponents in (0,1), and order-theoretic properties (operator monotonicity for exponents in [0,1]).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `CFC.nnrpow`, `CFC.sqrt`, and `CFC.rpow` via continuous functional calculus; includes algebraic properties (composition, inversion, multiplication rules), power notation instances, characterizations of nonnegative and strictly positive elements in C⋆-algebras via square root decomposition, and product/pi type compatibility |
| IntegralRepresentation.lean | Integral representation of `x ^ p` for `p ∈ (0,1)` as `∫ t, rpowIntegrand₀₁ p t x ∂μ` where `rpowIntegrand₀₁ p t x := t ^ p * (t⁻¹ - (t + x)⁻¹)`; proves existence of measure, integrability conditions, and lifts this representation to CFC with `exists_measure_nnrpow_eq_integral_cfcₙ_rpowIntegrand₀₁`; foundation for operator monotonicity and concavity results |
| Isometric.lean | Norm characterizations for rpow and sqrt over algebras with isometric CFC; proves `‖a ^ r‖ = ‖a‖ ^ r` for positive exponents and `‖sqrt a‖ = √‖a‖`, with both nnnorm and norm versions for unital and non-unital cases |
| Order.lean | Order-theoretic properties of rpow and sqrt in C⋆-algebras; proves operator monotonicity of `a ↦ a ^ p` for `p ∈ [0,1]` (both `monotone_nnrpow` and `monotone_rpow`) and `monotone_sqrt`; uses integral representation from IntegralRepresentation.lean to establish these properties |

## Subdirectories

*(None)*

## Search Tags

continuous-functional-calculus cfc real-powers rpow sqrt square-root cstar-algebra star-ordered-ring unital non-unital nnrpow operator-monotonicity integral-representation spectral-theory nonnegative-spectrum isometric-cfc norm-preserving algebraic-properties order-properties functional-analysis
