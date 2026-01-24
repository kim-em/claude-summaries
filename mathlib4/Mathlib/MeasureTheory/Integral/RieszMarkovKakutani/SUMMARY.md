---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Integral/RieszMarkovKakutani
generated: 2026-01-25T08:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 3
subdirs_count: 0
---

# RieszMarkovKakutani

## Overview

This directory contains the formalization of the Riesz-Markov-Kakutani representation theorem, which establishes the fundamental correspondence between positive linear functionals on spaces of compactly supported continuous functions and regular measures on locally compact T2 spaces. The theorem is proven for both ℝ≥0-linear and ℝ-linear functionals, with the ℝ version providing the core proof and the ℝ≥0 version building on it.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Technical foundations for the Riesz-Markov-Kakutani theorem: defines Riesz content via `rieszContentAux` (infimum of `Λf` over test functions dominating compact sets), proves monotonicity, finite subadditivity, and exact additivity on disjoint compacts, constructs partition-of-unity machinery for ℝ≥0-valued functions on disjoint compact sets, and establishes content regularity |
| Real.lean | Riesz-Markov-Kakutani representation theorem for ℝ-linear positive functionals: proves `∫ x, f x ∂(rieszMeasure Λ) = Λ f` via constructing the measure through `rieszContent` on the ℝ≥0-linearization, establishes bijectivity between positive linear functionals on `C_c(X, ℝ)` and regular measures, includes uniqueness theorem `Measure.ext_of_integral_eq_on_compactlySupported` and special cases for compact spaces |
| NNReal.lean | Riesz-Markov-Kakutani representation theorem for ℝ≥0-linear functionals: proves both Bochner integral version `∫ (x : X), (f x : ℝ) ∂(rieszMeasure Λ) = Λ f` and Lebesgue integral version `∫⁻ (x : X), f x ∂(rieszMeasure Λ) = Λ f`, establishes bijectivity between linear functionals on `C_c(X, ℝ≥0)` and regular measures via `integralLinearMap`, reduces to ℝ-version using `toRealPositiveLinear` conversion |

## Subdirectories

## Search Tags

riesz-markov-kakutani representation-theorem positive-linear-functional measure-theory regular-measure content riesz-content locally-compact hausdorff compactly-supported bochner-integral lebesgue-integral integral-representation partition-of-unity test-function nnreal real continuous-function measure-uniqueness
