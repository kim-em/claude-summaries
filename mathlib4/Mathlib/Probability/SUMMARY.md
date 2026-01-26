---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability
generated: 2026-01-26T23:50:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 15
subdirs_count: 8
---

# Probability

## Overview

The `Probability/` directory provides comprehensive formalization of modern probability theory built on rigorous measure-theoretic foundations. At the top level, it defines core concepts including probability density functions (PDFs) via Radon-Nikodym derivatives, conditional probability measures with Bayes' theorem, random variable laws (distributions), cumulative distribution functions (CDFs), identically distributed random variables, and fundamental limit theorems (Borel-Cantelli lemmas, strong law of large numbers). The directory encompasses eight major subdirectories forming a complete probability library: `Kernel/` provides the Markov kernel infrastructure with composition operations, disintegration theory for product spaces, and Ionescu-Tulcea theorem for infinite products; `Independence/` develops both unconditional and conditional independence via a unified kernel framework with characterizations through bounded continuous functions and characteristic functions, plus Kolmogorov's 0-1 law; `Distributions/` implements concrete continuous distributions (beta, exponential, gamma, Pareto) and discrete distributions (geometric, Poisson, uniform), with sophisticated Gaussian theory extending to infinite-dimensional Banach and Hilbert spaces including Fernique's theorem; `ProbabilityMassFunction/` formalizes discrete distributions as a monad with Bernoulli and binomial constructions; `Martingale/` establishes martingale theory with Doob's decomposition and convergence theorems, optional stopping and sampling theorems, upcrossing estimates, and Lévy's generalized Borel-Cantelli; `Moments/` develops moment-generating functions as analytic functions with derivatives yielding moments, variance and covariance theory, sub-Gaussian variables, and Chernoff/Hoeffding concentration inequalities; `Process/` defines filtrations, adapted and progressively measurable processes, stopping times, hitting times, predictable processes, and finite-dimensional distributions; and `Decision/` formalizes statistical decision theory with risk measures (average, Bayes, minimax) and data-processing inequalities. Together, these components provide the mathematical foundation for rigorous probability theory from elementary concepts through advanced stochastic process analysis and statistical inference.

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

- [x] `Decision/` - Statistical decision theory: framework for analyzing estimators via loss functions and risk measures (average risk, Bayes risk, minimax risk), with fundamental inequalities relating Bayes and minimax risk and data-processing theorems showing information loss increases risk
- [x] `Distributions/` - Concrete probability distributions spanning continuous (beta, exponential, gamma, Pareto with explicit PDFs), discrete (geometric, Poisson with PMFs), uniform distributions, and comprehensive Gaussian theory from real line to infinite-dimensional Banach/Hilbert spaces with characteristic functions, convolution properties, and Fernique's theorem for exponential integrability
- [x] `Independence/` - Comprehensive independence theory with kernel-based framework unifying unconditional and conditional independence: four flavors (sets of sets, σ-algebras, events, random variables) with notation `X ⟂ᵢ[μ] Y`, characterizations via bounded continuous functions and characteristic functions, multiplicativity of expectation, infinite product measures, stochastic process independence, and Kolmogorov's 0-1 law for tail σ-algebras
- [x] `Kernel/` - Markov kernels (measurable maps `α → Measure β`): foundational theory with classifications (Markov, finite, s-finite), basic constructors (deterministic, constant, identity, restriction), composition operations (sequential `∘ₖ`, parallel `∥ₖ`, composition-product `⊗ₖ`, simple product `×ₖ`) with Chapman-Kolmogorov equations, disintegration theory decomposing product measures into marginals and conditional kernels for standard Borel spaces, Ionescu-Tulcea theorem for infinite products from history-dependent kernels, Radon-Nikodym derivatives and Lebesgue decomposition, regular conditional probability distributions, and Bayesian posterior distributions
- [x] `Martingale/` - Discrete-time martingale theory: core definitions (martingales, supermartingales, submartingales) with respect to filtrations, Doob's decomposition into martingale and predictable parts, optional stopping theorem (fair game theorem) with Doob's maximal inequality, Doob's upcrossing estimate, martingale convergence theorems (almost everywhere and L¹), optional sampling theorem, and Lévy's generalized Borel-Cantelli lemma
- [x] `Moments/` - Moment theory centered on moment-generating functions (MGF) and cumulant-generating functions (CGF): analyticity of MGF with derivatives yielding moments, integrability domains as convex intervals, complex MGF extension connecting to characteristic functions with uniqueness results, variance and covariance theory (Chebyshev's inequality, Bhatia-Davis and Popoviciu's inequalities), covariance bilinear forms for Banach and Hilbert spaces, tilted measures relating MGF derivatives to variance, sub-Gaussian random variables, and concentration inequalities (Hoeffding's lemma and inequality, Azuma-Hoeffding for martingales)
- [x] `ProbabilityMassFunction/` - Discrete probability formalization via PMF type (functions `α → ℝ≥0∞` summing to 1) with conversions to/from measure theory, monadic structure (`pure`, `bind`, `bindOnSupport`) making PMF a lawful monad, functorial operations (`map`, `seq`), construction utilities (`ofFinset`, `ofFintype`, `normalize`, `filter`), concrete distributions (Bernoulli, binomial with choose coefficients), and integration theory connecting PMFs to expected values via weighted sums
- [x] `Process/` - Stochastic process foundations: filtrations (monotone sequences of sub-σ-algebras), adapted and progressively measurable processes, stopping times with associated σ-algebras and stopped processes, hitting times as stopping times for discrete processes, predictable σ-algebras and predictable processes, finite-dimensional distributions with projective limit characterization, Kolmogorov-Chentsov conditions for continuous modifications, and partition-based filtrations for constructing measurable functions

## Search Tags

probability probability-theory random-variables pdf cdf expectation conditional-expectation conditional-probability bayes-theorem measure-theory law-of-large-numbers strong-law borel-cantelli radon-nikodym density-function uniform-distribution identically-distributed independence martingales stochastic-processes moments variance pmf kernels markov
