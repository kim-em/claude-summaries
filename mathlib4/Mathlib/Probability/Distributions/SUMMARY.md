---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Distributions
generated: 2026-01-26T20:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 9
subdirs_count: 1
---

# Distributions

## Overview

The `Distributions/` directory provides formalized implementations of concrete probability distributions over various spaces. It includes continuous distributions (beta, exponential, gamma, Pareto) with probability density functions (PDFs) over the reals, discrete distributions (geometric, Poisson) with probability mass functions (PMFs) over the naturals, and specialized distributions (uniform over sets and fintypes, set-Bernoulli for random sets). The directory also contains Fernique's theorem proving exponential integrability for rotation-invariant Gaussian measures. Each distribution file defines the PDF/PMF, proves it integrates/sums to 1, constructs the corresponding probability measure, and for continuous distributions often includes the cumulative distribution function (CDF).

## Key Files

| File | Purpose |
|------|---------|
| Beta.lean | Beta distribution over ℝ with shape parameters α and β, defined via `betaPDFReal α β x = (1 / beta α β) * x ^ (α - 1) * (1 - x) ^ (β - 1)` for x in (0,1), includes beta function normalization via gamma functions |
| Exponential.lean | Exponential distribution over ℝ with rate parameter r, defined as special case of gamma distribution (shape=1), includes CDF proof `1 - exp(-(r*x))` and integration formulas |
| Gamma.lean | Gamma distribution over ℝ with shape a and rate r, PDF `r^a / Gamma(a) * x^(a-1) * exp(-(r*x))` for x≥0, proves PDF integrates to 1 using integral of rpow times exponential |
| Pareto.lean | Pareto distribution over ℝ with scale t and shape r, PDF `r * t^r * x^(-(r+1))` for x≥t, also called power-law distribution |
| Geometric.lean | Geometric distribution over ℕ with success probability p, PMF `(1-p)^n * p`, models number of failures before first success |
| Poisson.lean | Poisson distribution over ℕ with rate λ, PMF `exp(-λ) * λ^n / n!`, proves sum equals 1 using exponential series |
| Uniform.lean | Two related notions: (1) uniform distribution on measurable sets via `IsUniform` predicate and `uniformPDF`, (2) uniform PMFs via `uniformOfFinset`, `uniformOfFintype`, and `ofMultiset` for finite/countable structures |
| SetBernoulli.lean | Product of Bernoulli distributions on a set - for set u and probability p, each element i∈u belongs to random set with probability p, notation `setBer(u, p)` |
| Fernique.lean | Fernique's theorem: for finite measure μ on normed space where μ.prod μ is invariant under rotation by -π/4, there exists C>0 such that `exp(C*‖x‖²)` is integrable, includes detailed proof via annuli decomposition and geometric threshold sequence |

## Subdirectories

- [ ] `Gaussian/` - Gaussian (normal) distributions

## Search Tags

probability-distributions beta-distribution exponential-distribution gamma-distribution pareto-distribution geometric-distribution poisson-distribution uniform-distribution gaussian-distribution normal-distribution pdf cdf pmf probability-density-function cumulative-distribution-function probability-mass-function bernoulli fernique rotation-invariant continuous-distributions discrete-distributions measure-theory
