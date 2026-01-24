---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/VectorMeasure
generated: 2026-01-25T22:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 2
subdirs_count: 1
---

# VectorMeasure

## Overview

The `VectorMeasure/` directory provides the formalization of vector-valued measures and signed measures. Vector measures are σ-additive functions from measurable sets to an additive monoid (such as ℝ, ℂ, or general Banach spaces) that map the empty set and non-measurable sets to zero. This generalizes classical measure theory to allow measures with positive and negative parts. The directory includes fundamental operations (pushforward, restriction, scalar multiplication), order structures, absolute continuity, mutual singularity, and the construction of vector measures via integration (with-density construction for Radon-Nikodym applications).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of vector measures and signed measures: defines `VectorMeasure α M` as a σ-additive function to an additive monoid `M` with topological space structure, provides `SignedMeasure α` as an abbreviation for `VectorMeasure α ℝ`, proves extensionality and summability properties, defines operations (addition, negation, scalar multiplication, pushforward `map`, restriction `restrict`), establishes partial order structure, defines absolute continuity (`≪ᵥ`) and mutual singularity (`⟂ᵥ`) for vector measures, and proves `trim` operation for restricting to sub-σ-algebras |
| WithDensity.lean | Vector measure defined by integration: defines `Measure.withDensityᵥ μ f` as the vector measure sending measurable set `s` to `∫ x in s, f x ∂μ`, proves linearity properties (addition, scalar multiplication, negation), establishes absolute continuity `μ.withDensityᵥ f ≪ᵥ μ.toENNRealVectorMeasure`, proves that integrable functions with equal `withDensityᵥ` are almost everywhere equal, connects `withDensityᵥ` to signed measures via positive/negative parts decomposition, key tool for Radon-Nikodym theorem stating vector measures absolutely continuous with respect to a measure have a density |

## Subdirectories

- [ ] `Decomposition/` - Decomposition theorems for signed and vector measures (Hahn, Jordan, Lebesgue, Radon-Nikodym)

## Search Tags

vector-measure signed-measure sigma-additive absolute-continuity mutual-singularity radon-nikodym with-density integration measure-theory restriction pushforward
