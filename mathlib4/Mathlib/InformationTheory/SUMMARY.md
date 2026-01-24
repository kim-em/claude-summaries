---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/InformationTheory
generated: 2026-01-24T22:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 1
subdirs_count: 1
---

# InformationTheory

## Overview

The `InformationTheory/` directory contains formalized information theory concepts fundamental to coding theory and information measurement. It includes the Hamming distance/norm metric (counting differing positions in Pi types, used for defining minimum code distance), the Kullback-Leibler (KL) divergence (measuring difference between probability measures), and supporting f-divergence infrastructure. The Hamming implementation provides a type synonym with normed group structure using the Hamming metric instead of sup norm, while KL divergence is defined on finite measures with Gibbs' inequality (nonnegativity) and converse Gibbs' inequality (zero iff measures equal).

## Key Files

| File | Purpose |
|------|---------|
| Hamming.lean | Hamming distance/norm on finite Pi types: defines `hammingDist` (counts positions where values differ), `hammingNorm` (counts non-zero entries), `Hamming β` type synonym equipped with metric/normed group instances using Hamming metric, proves metric space axioms (triangle inequality, symmetry, positivity), and establishes relationship to coding theory minimum distance |

## Subdirectories

- [ ] `KullbackLeibler/` - Kullback-Leibler divergence theory: defines KL divergence `klDiv μ ν` as f-divergence using `klFun x = x * log x + 1 - x`, proves Gibbs' inequality (KL divergence is nonnegative) and converse (zero iff measures equal), establishes equivalence between integrability of log-likelihood ratio and integrability of KL function composed with Radon-Nikodym derivative, with alternative formulas as integral and Lebesgue integral of klFun

## Search Tags

information-theory hamming-distance hamming-norm kullback-leibler kl-divergence f-divergence coding-theory metric-space normed-group gibbs-inequality log-likelihood-ratio radon-nikodym measure-theory mathlib4
