---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/ProbabilityMassFunction
generated: 2026-01-26T19:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# ProbabilityMassFunction

## Overview

The `ProbabilityMassFunction/` directory provides a complete formalization of probability mass functions (PMFs), which are discrete probability measures defined as functions `α → ℝ≥0∞` with values summing to 1. This includes the core `PMF` type definition with conversions to and from measure theory (`toMeasure`, `toPMF`), monadic operations (`pure`, `bind`, `bindOnSupport`) giving PMF a monad structure, functorial operations (`map`, `seq`), construction utilities (`ofFinset`, `ofFintype`, `normalize`, `filter`), concrete distributions (Bernoulli, binomial), and integration theory connecting PMFs with expected values through weighted sums.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core PMF type definition as `{f : α → ℝ≥0∞ // HasSum f 1}` with support theory, conversions between PMF and measure theory (`toOuterMeasure`, `toMeasure`, `Measure.toPMF`), probability measure instance, and fundamental theorems on singleton measures and support properties |
| Monad.lean | Monadic operations: `pure a` (distribution concentrated at single point), `bind` (sampling composition: sample from first PMF then from dependent second PMF), `bindOnSupport` (generalized bind for partial functions defined only on support), with Monad and LawfulMonad instances |
| Constructions.lean | PMF construction utilities: `map` and `seq` (functorial/applicative operations), `ofFinset`/`ofFintype` (construct from finite sums), `normalize` (normalize arbitrary function by its sum), `filter` (filter support and renormalize), `bernoulli` (Bernoulli distribution on Bool with parameter `p : ℝ≥0`), LawfulFunctor instance, and ULiftable instance for universe polymorphism |
| Binomial.lean | Binomial distribution `binomial p h n : PMF (Fin (n+1))` representing probability of observing exactly `i` successes in `n` independent trials with success probability `p`, using formula `p^i * (1-p)^(n-i) * choose(n,i)`, with theorem `binomial_one_eq_bernoulli` showing equivalence to Bernoulli for `n=1` |
| Integrals.lean | Integration theory for PMFs: main theorem `integral_eq_tsum` showing integral with respect to `p.toMeasure` equals `∑' a, (p a).toReal • f a`, finite version `integral_eq_sum` for `Fintype`, and specific expected value calculation `bernoulli_expectation` showing `𝔼[b] = p.toReal` for Bernoulli distribution |

## Subdirectories

(none)

## Search Tags

probability-mass-function pmf discrete-probability monad bind pure map measure-theory integration expected-value bernoulli binomial summation tsum normalized-function support countable-measure probability-measure dirac fintype
