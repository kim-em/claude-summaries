---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Real/Pi
generated: 2025-12-05T08:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 5
subdirs_count: 0
---

# Pi

## Overview

The `Pi/` directory contains theoretical results and computational formulas related to the mathematical constant π (pi). This includes rigorous numerical bounds on π's value, proofs of its irrationality using Cartwright's method via integral sequences, and classical infinite series and product formulas (Leibniz series, Wallis product, Chudnovsky algorithm). The bounds file provides tactics for mechanized proofs of inequalities involving π.

## Key Files

| File | Purpose |
|------|---------|
| Bounds.lean | Establishes numerical bounds on π using series approximations; defines `pi_gt_sqrtTwoAddSeries` and `pi_lt_sqrtTwoAddSeries` relating π to nested square root sequences; provides custom tactics `pi_lower_bound` and `pi_upper_bound` for proving rational bounds; includes witnesses for bounds like `3.14 < π < 3.15` up to 20 decimal places |
| Irrational.lean | Proves `irrational_pi` using Cartwright's proof method; defines integral sequence `I n θ = ∫ x in (-1)..1, (1 - x²)ⁿ * cos(x * θ)`; constructs integer-coefficient polynomials `sinPoly` and `cosPoly` relating integrals to trigonometric values; shows the integral bounds lead to contradiction if π/2 were rational |
| Leibniz.lean | Proves Leibniz's series for π: the alternating sum `Σ (-1)ⁱ / (2i + 1)` converges to π/4 (`tendsto_sum_pi_div_four`); uses Abel's limit theorem to extend the Maclaurin series of arctan to x = 1 |
| Wallis.lean | Establishes the Wallis product formula for π/2 (`tendsto_prod_pi_div_two`); defines `W k` as the product `∏ (2i+2)/(2i+1) * (2i+2)/(2i+3)`; proves convergence by analyzing ratios of integrals `∫ sin x ^ n` and using squeeze theorem |
| Chudnovsky.lean | Defines Chudnovsky's formula for computing π⁻¹ using the infinite sum involving factorials and the constant 640320; includes definitions `chudnovskyTerm`, `chudnovskyNum`, `chudnovskyDenom`, and `chudnovskySum`; contains `proof_wanted chudnovskySum_eq_pi_inv` for future work (proof not yet completed) |

## Subdirectories

*(No subdirectories)*

## Search Tags

pi real-analysis irrational bounds numerical-approximation leibniz-series wallis-product chudnovsky-formula trigonometric-integrals arctan cartwright-proof integral-sequences factorial rational-approximation
