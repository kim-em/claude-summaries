---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Independence
generated: 2026-01-26T20:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 10
subdirs_count: 1
---

# Independence

## Overview

The `Independence/` directory provides a comprehensive formalization of independence theory in probability, built on a kernel-based framework that unifies unconditional and conditional independence. The directory defines four flavors of independence (sets of sets, σ-algebras, sets/events, and functions/random variables), both for families (`iIndep*`) and pairs (`Indep*`), with notation `X ⟂ᵢ[μ] Y` for unconditional independence and `X ⟂ᵢ[Z, hZ; μ] Y` for conditional independence. The `Kernel/` subdirectory provides the foundational kernel-based definitions that work with respect to a kernel `κ : Kernel α Ω` and measure `μ`, generalizing both conditional independence (using `condExpKernel`) and unconditional independence (using `Kernel.const Unit μ`). The main directory builds on this foundation to provide user-facing independence concepts, multiple characterizations (via bounded continuous functions, characteristic functions), integration results (multiplicativity of expectation for independent variables), infinite product measures for arbitrary families, stochastic process independence, and Kolmogorov's 0-1 law for tail σ-algebras. The fundamental π-system lemma shows that independent π-systems generate independent σ-algebras.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of independence: `iIndepSets` (families of π-systems), `iIndep` (families of σ-algebras), `iIndepSet` (families of sets), `iIndepFun` (families of random variables), with pairwise versions; fundamental theorem that independent π-systems generate independent σ-algebras; notation `X ⟂ᵢ[μ] Y` |
| Conditional.lean | Conditional independence given a σ-algebra: `iCondIndepSets`, `iCondIndep`, `iCondIndepSet`, `iCondIndepFun` with kernel-based definitions using `condExpKernel`; theorem that conditionally independent π-systems generate conditionally independent σ-algebras; notation `X ⟂ᵢ[Z, hZ; μ] Y` |
| BoundedContinuousFunction.lean | Characterization of independence via bounded continuous functions: random variables X and Y are independent iff `∫ f(X)g(Y) = ∫ f(X) · ∫ g(Y)` for all bounded continuous f, g; extends to stochastic processes and events; handles products without second countability assumption |
| CharacteristicFunction.lean | Independence characterization via characteristic functions: random variables are independent iff their joint characteristic function equals the product of individual characteristic functions; versions for Hilbert spaces (`charFun`) and Banach spaces (`charFunDual`); extends to finite families |
| Integration.lean | Integration results for independent random variables: `E[X * Y] = E[X] * E[Y]` for independent random variables over ℝ≥0∞ and similar results for integrable functions |
| Integrable.lean | Proves that if a nonzero function belongs to Lᵖ (in particular is integrable) and is independent of another function, then the measure is a probability measure |
| InfinitePi.lean | Independence of arbitrary (possibly uncountable) families of random variables via infinite product measures: random variables are independent iff their joint distribution equals the infinite product measure |
| Process.lean | Independence of stochastic processes: a process (Xₛ)ₛ is independent from Y iff all finite subfamilies are independent from Y; two processes are independent iff all finite subfamilies are pairwise independent |
| ZeroOne.lean | Kolmogorov's 0-1 law: any set measurable with respect to the tail σ-algebra `limsup s atTop` of an independent sequence of σ-algebras has probability 0 or 1 |
| Kernel.lean | Deprecated module (since 2025-12-01) that re-exports `Kernel.IndepFun` |

## Subdirectories

- [x] `Kernel/` - Kernel-based independence framework: `iIndepSets`/`iIndep`/`iIndepSet`/`iIndepFun` definitions with respect to a kernel and measure; generalizes both unconditional and conditional independence; π-system lemma; independence preserved under composition, arithmetic operations, and suprema of directed families; conditional probability factorization

## Search Tags

independence conditional-independence random-variables stochastic-processes characteristic-function bounded-continuous-function integration expectation multiplicativity kolmogorov-zero-one-law tail-sigma-algebra infinite-product pi-system kernel markov-kernel indepfun indepset probability-measure integrable conditional-expectation
