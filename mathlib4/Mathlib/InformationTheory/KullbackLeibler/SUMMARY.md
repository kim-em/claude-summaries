---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/InformationTheory/KullbackLeibler
generated: 2026-01-24T22:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# KullbackLeibler

## Overview

The `KullbackLeibler/` directory provides the formal definition and theory of the Kullback-Leibler (KL) divergence, a fundamental measure of difference between probability distributions used in information theory and statistics. The implementation defines KL divergence as an f-divergence using the function `klFun x = x * log x + 1 - x`, extends it to finite measures via a correction term `ν.real univ - μ.real univ`, and establishes key results including Gibbs' inequality (nonnegativity) and the converse Gibbs' inequality (zero iff measures equal).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Main KL divergence definition and theory: defines `klDiv μ ν` taking value in `ℝ≥0∞` (infinity if not absolutely continuous or not integrable, otherwise `ENNReal.ofReal (∫ x, llr μ ν x ∂μ + ν.real univ - μ.real univ)`), provides alternative formulas as integral/Lebesgue integral of `klFun` composed with Radon-Nikodym derivative, proves Gibbs' inequality (`integral_llr_add_sub_measure_univ_nonneg`), proves converse Gibbs' inequality (`klDiv_eq_zero_iff`: KL divergence zero iff measures equal), establishes various inequalities including `mul_log_le_toReal_klDiv` |
| KLFun.lean | The f-divergence function for KL divergence: defines `klFun x = x * log x + 1 - x` (continuous, nonnegative, strictly convex on [0,∞) with minimum 0 at 1), proves derivative properties (`deriv klFun = log`, `rightDeriv_klFun_one = 0`), establishes integrability equivalence (`integrable_klFun_rnDeriv_iff`: `klFun ∘ rnDeriv` integrable iff log-likelihood ratio integrable), proves integral formula `integral_klFun_rnDeriv` relating integrals over different measures, chosen to satisfy `klFun 1 = 0` and `deriv klFun 1 = 0` ensuring desirable KL divergence properties extend to finite measures |

## Subdirectories

None

## Search Tags

kullback-leibler kl-divergence f-divergence information-theory measure-theory gibbs-inequality log-likelihood-ratio radon-nikodym-derivative absolute-continuity finite-measures probability-theory convex-analysis integrability mathlib4
