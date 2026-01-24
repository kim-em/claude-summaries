---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Integral/Lebesgue
generated: 2026-01-25T08:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# Lebesgue

## Overview

The `Lebesgue/` directory contains the foundational theory of the Lebesgue integral for extended non-negative real-valued functions (`ℝ≥0∞`), also known as the lower Lebesgue integral (denoted `∫⁻`). This includes the basic definition as a supremum over simple functions, monotone convergence theorem (Beppo Levi lemma), dominated convergence theorem for sequences and filters, additivity and subtraction properties, behavior under measure-preserving maps and equivalences, Markov's inequality and its applications, and specialized results for finite/countable types and measures (including Dirac measures and counting measure). This forms the computational foundation upon which the Bochner integral (for Banach space-valued functions) is built.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of the lower Lebesgue integral `∫⁻ x, f x ∂μ` as supremum over simple functions, monotonicity properties, relationship between `lintegral` and simple function integrals, and fundamental inequalities |
| Add.lean | Monotone convergence theorem (Beppo Levi lemma) proving `∫⁻ ⨆ n, f n = ⨆ n, ∫⁻ f n` for monotone sequences, with applications to additivity `∫⁻ (f + g) = ∫⁻ f + ∫⁻ g` and scalar multiplication of the Lebesgue integral |
| Sub.lean | Subtraction of Lebesgue integrals: proves `∫⁻ (f - g) = ∫⁻ f - ∫⁻ g` when `g ≤ f` almost everywhere and `∫⁻ g ≠ ∞`, includes monotone convergence for decreasing sequences (`lintegral_iInf_ae`) |
| Map.lean | Behavior under maps: proves `∫⁻ a, f a ∂(μ.map g) = ∫⁻ a, f (g a) ∂μ` for measurable `f` and `g`, includes variants for measure-preserving maps, measurable embeddings, equivalences, and subtype coercion |
| Markov.lean | Markov's inequality (Chebyshev's first inequality): `ε * μ{x \| ε ≤ f x} ≤ ∫⁻ f`, with applications including characterization of almost everywhere equality via integral comparison and strict monotonicity of integral |
| DominatedConvergence.lean | Dominated convergence theorem for `ℝ≥0∞`-valued functions: if `Fₙ → f` pointwise a.e. and `Fₙ ≤ bound` with `∫⁻ bound ≠ ∞`, then `∫⁻ Fₙ → ∫⁻ f`, includes variants for filters and converse results (integral convergence implies pointwise convergence for monotone/antitone sequences) |
| Countable.lean | Specializations to finite and countable contexts: integrals over finite measures with bounded functions are finite, integral equals constant for probability measures, Dirac measure integrals `∫⁻ a, f a ∂(dirac a) = f a`, counting measure results |
| Norm.lean | Interactions with norms: relates `∫⁻ ‖f x‖ₑ` (integral of extended norm) to `∫⁻ ENNReal.ofReal (f x)` for real-valued functions, particularly when `f` is non-negative |

## Subdirectories

None

## Search Tags

lebesgue-integral lintegral lower-lebesgue-integral ennreal extended-nonnegative-reals simple-functions monotone-convergence beppo-levi dominated-convergence markov-inequality chebyshev-inequality measure-preserving map-measure dirac-measure counting-measure finite-measure probability-measure additivity subtraction norm convergence-theorems
