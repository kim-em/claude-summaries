---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/ModularForms/EisensteinSeries
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 1
---

# EisensteinSeries

## Overview

The `EisensteinSeries/` directory provides a comprehensive formalization of Eisenstein series for modular forms across all weights k ≥ 2. For weights k ≥ 3, the implementation establishes that Eisenstein series are genuine modular forms by proving slash-invariance, boundedness at cusps, and holomorphicity via absolutely convergent sums over coprime integer pairs. The theory includes detailed summability results, uniform convergence proofs, and explicit q-expansion formulas relating Eisenstein series to Riemann zeta values, Bernoulli numbers, and divisor sums. The weight-2 case receives specialized treatment in the `E2/` subdirectory, as it requires conditional summation techniques and exhibits quasi-modular behavior (transforming with an anomalous defect function under SL(2,ℤ) action) rather than being a true modular form.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Constructs Eisenstein series as modular forms: `eisensteinSeries_MF` proves E-series of weight k ≥ 3 satisfy slash-invariance, holomorphicity, and cusp boundedness; includes normalized level-1 series `E` |
| Defs.lean | Core definitions: `gammaSet N r a` for coprime integer pairs congruent to `a` mod N with gcd r, `eisSummand k v z` summand function, `eisensteinSeries` as infinite sum, `eisensteinSeries_SIF` as slash-invariant form, includes gamma set equivalences and slash action transformation lemmas |
| IsBoundedAtImInfty.lean | Proves Eisenstein series are bounded at infinity (`isBoundedAtImInfty_eisensteinSeries_SIF`) by showing norm bounds in vertical strips and using vertical strip confinement for Γ(N)-invariance |
| MDifferentiable.lean | Proves holomorphicity of Eisenstein series: `eisensteinSeries_SIF_MDifferentiable` shows E-series are MDifferentiable (holomorphic ℍ → ℂ functions) using uniform convergence and term-by-term differentiation |
| QExpansion.lean | Derives q-expansion formulas for level-1 Eisenstein series: proves `E_k(z) = 1 - (2k/B_k) ∑' n, σ_{k-1}(n) q^n` via cotangent expansion identity and Riemann zeta relation to Bernoulli numbers (even k, k ≥ 3) |
| Summable.lean | Establishes summability of Eisenstein series summands: defines bounding functions `r(z)` and `r1(z)`, proves norm bounds for `eisSummand` terms, includes general p-series summability lemmas for k > 2 |
| UniformConvergence.lean | Proves locally uniform convergence of Eisenstein series on ℍ (`eisensteinSeries_tendstoLocallyUniformly`), essential for differentiability arguments and construction of holomorphic limit |

## Subdirectories

- [x] `E2/` - Weight-2 Eisenstein series requiring conditional summation over symmetric intervals

## Search Tags

eisenstein-series modular-forms q-expansion riemann-zeta bernoulli-numbers summability uniform-convergence holomorphic slash-invariant gamma-set coprime-pairs level-gamma-N boundedness-at-cusps mdifferentiable divisor-sum sigma-function
