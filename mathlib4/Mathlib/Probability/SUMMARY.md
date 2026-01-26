---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability
generated: 2026-01-26T19:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 15
subdirs_count: 8
---

# Probability

## Overview

The `Probability/` directory provides comprehensive formalization of probability theory built on measure theory foundations. It defines core probability concepts including probability density functions (PDFs), conditional probability and expectation, random variables with laws, probability mass functions, cumulative distribution functions (CDFs), and identically distributed random variables. The directory includes major theorems such as the Borel-Cantelli lemmas and the strong law of large numbers (Etemadi's version requiring only pairwise independence). It also contains specialized subdirectories for probability kernels, martingales, stochastic processes, moments (variance, MGFs), independence theory, concrete distributions, and decision theory.

## Key Files

| File | Purpose |
|------|---------|
| Notation.lean | Defines standard probability notation: `P[X]` (expectation under measure P), `𝔼[X]` (expectation), `𝔼[X\|m]` (conditional expectation), `P⟦s\|m⟧` (conditional probability), `X =ₐₛ Y` (almost sure equality), `∂P/∂Q` (Radon-Nikodym derivative), `ℙ` (volume measure) |
| Integration.lean | Deprecated module (since 2025-07-30) that previously provided integration utilities |
| HasLaw.lean | Defines the `HasLaw X μ P` predicate stating random variable X has law μ under measure P (i.e., `P.map X = μ`), with theorems on composition, products of independent variables, and integration formulas (law of unconscious statistician) |
| HasLawExists.lean | Brief extension providing existence theorems for laws |
| ConditionalProbability.lean | Defines conditional probability measure `cond μ s` (notation `μ[\|s]`) as scaled restriction `(μ s)⁻¹ • μ.restrict s`, proves it's a probability measure, derives axiomatic definition `μ[t \| s] = (μ s)⁻¹ * μ (s ∩ t)`, includes Bayes' theorem and law of total probability |
| ConditionalExpectation.lean | Import wrapper for conditional expectation from measure theory |
| Density.lean | Defines `HasPDF X ℙ μ` (X has probability density function with respect to measures ℙ and μ), defines `pdf X` as Radon-Nikodym derivative, proves law of unconscious statistician for PDFs, includes uniform distribution theory |
| IdentDistrib.lean | Defines identically distributed random variables via `IdentDistrib X Y μ ν` (X under μ has same distribution as Y under ν), with preservation theorems under composition and algebraic operations |
| IdentDistribIndep.lean | Proves independence properties are preserved under identical distribution |
| BorelCantelli.lean | Second Borel-Cantelli lemma: for independent sets with `∑ μ sₙ = ∞`, the limsup has measure 1 (first lemma is in MeasureTheory) |
| StrongLaw.lean | Strong law of large numbers (Etemadi's proof): for pairwise independent identically distributed integrable random variables, `∑ i ∈ range n, X i / n → 𝔼[X 0]` almost surely; includes both almost-sure and Lᵖ convergence versions |
| CDF.lean | Cumulative distribution function for real-valued random variables |
| CondVar.lean | Conditional variance theory |
| ProductMeasure.lean | Product measure constructions for probability |
| UniformOn.lean | Uniform distribution on sets |

## Subdirectories

- [ ] `Decision/` - Decision theory
- [ ] `Distributions/` - Concrete probability distributions
- [ ] `Independence/` - Independence theory for random variables and events
- [ ] `Kernel/` - Probability kernels (Markov kernels)
- [ ] `Martingale/` - Martingale theory
- [ ] `Moments/` - Moments of random variables (variance, MGFs)
- [ ] `ProbabilityMassFunction/` - Discrete probability distributions
- [ ] `Process/` - Stochastic processes

## Search Tags

probability probability-theory random-variables pdf cdf expectation conditional-expectation conditional-probability bayes-theorem measure-theory law-of-large-numbers strong-law borel-cantelli radon-nikodym density-function uniform-distribution identically-distributed independence martingales stochastic-processes moments variance pmf kernels markov
