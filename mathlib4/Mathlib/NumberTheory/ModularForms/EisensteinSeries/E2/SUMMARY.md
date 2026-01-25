---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/ModularForms/EisensteinSeries/E2
generated: 2026-01-25T21:40:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# E2

## Overview

The `E2/` directory provides the formalization of the weight-2 Eisenstein series, which requires special treatment due to conditional convergence issues. Unlike the higher weight cases (k ≥ 3) that converge absolutely, the weight-2 series E2 must be defined as a conditional sum over symmetric intervals. The implementation defines both the normalized E2 and the unnormalized G2 forms, establishes their summability via symmetric limits, derives q-expansion formulas relating E2 to divisor sums, and characterizes the defect function D2 that measures how E2 fails to be a true modular form (transforming with an anomalous term under SL(2,ℤ) action).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions for weight-2 Eisenstein series: `e2Summand m z` auxiliary summand, `G2` as conditional sum over symmetric intervals `symmetricIcc ℤ`, normalized `E2 = (1/(2*ζ(2))) • G2`, defect function `D2 γ z` measuring modular form failure, includes parity lemmas, transformation laws `D2_mul` and `D2_inv`, generator evaluations `D2_T = 0` and `D2_S z = 2πi/z` |
| Summable.lean | Summability and convergence proofs: establishes `hasSum_e2Summand_symmetricIcc` and `summable_e2Summand_symmetricIcc` for symmetric interval summation, derives q-expansion `G2 z = 2*ζ(2) - 8π² ∑' n, σ₁(n) qⁿ` via `qExpansion_identity_pnat`, proves `tendsto_e2Summand_atTop_nhds_zero`, includes equivalence between `symmetricIcc` and `symmetricIco` summation |

## Subdirectories

None

## Search Tags

weight-2-eisenstein-series conditional-convergence symmetric-intervals e2 g2 defect-function quasi-modular-form sl2z-transformation q-expansion divisor-sum riemann-zeta summability-symmetric parity-even modular-anomaly slash-action-defect
