---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/InformationTheory
generated: 2026-01-24T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 1
---

# InformationTheory

## Overview

The `InformationTheory/` directory provides foundational information-theoretic measures with applications to coding theory and statistics. It formalizes two key concepts: the Hamming distance/norm (discrete metric counting differing positions in finite Pi types, yielding a normed group structure essential for error-correcting codes) and the Kullback-Leibler divergence (a measure of difference between probability distributions implemented as an f-divergence). The Hamming theory establishes metric space axioms and connections to minimum code distance. The KL divergence implementation is comprehensive, defining `klDiv μ ν` on finite measures using the f-divergence function `klFun x = x * log x + 1 - x`, providing alternative formulas via log-likelihood ratio integrals, proving Gibbs' inequality (nonnegativity) and its converse (zero iff measures equal), and establishing integrability equivalences between the KL function and log-likelihood ratios.

## Key Files

| File | Purpose |
|------|---------|
| Hamming.lean | Hamming distance/norm on finite Pi types: defines `hammingDist` (counts positions where values differ), `hammingNorm` (counts non-zero entries), `Hamming β` type synonym equipped with metric/normed group instances using Hamming metric, proves metric space axioms (triangle inequality, symmetry, positivity), and establishes relationship to coding theory minimum distance |

## Subdirectories

- [x] `KullbackLeibler/` - Kullback-Leibler divergence theory: defines KL divergence `klDiv μ ν` as f-divergence using `klFun x = x * log x + 1 - x` (continuous, nonnegative, strictly convex with minimum at 1), extends to finite measures via correction term, proves Gibbs' inequality (nonnegativity via `integral_llr_add_sub_measure_univ_nonnegative`), proves converse (`klDiv_eq_zero_iff`: zero iff measures equal), establishes integrability equivalence between `klFun ∘ rnDeriv` and log-likelihood ratio, provides integral formulas and inequalities including `mul_log_le_toReal_klDiv`

## Search Tags

information-theory hamming-distance hamming-norm kullback-leibler kl-divergence f-divergence coding-theory metric-space normed-group gibbs-inequality log-likelihood-ratio radon-nikodym measure-theory mathlib4
