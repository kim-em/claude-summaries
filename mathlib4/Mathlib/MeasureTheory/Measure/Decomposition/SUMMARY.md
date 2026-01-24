---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Measure/Decomposition
generated: 2026-01-24T19:20:33Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Decomposition

## Overview

The `Decomposition/` directory contains fundamental measure decomposition theorems in mathlib4. It formalizes the Lebesgue decomposition theorem (decomposing a measure into mutually singular and absolutely continuous parts), the Radon-Nikodym theorem (characterizing absolute continuity via density functions), the unsigned Hahn decomposition theorem (partitioning a space where one measure dominates the other), and the method of exhaustion (finding sigma-finite sets for measures). These theorems are central to measure theory and provide the foundation for integration theory, probability theory, and the Radon-Nikodym derivative.

## Key Files

| File | Purpose |
|------|---------|
| Lebesgue.lean | Lebesgue decomposition theorem: for σ-finite measures μ and ν, decomposes μ as `μ = μ.singularPart ν + ν.withDensity (μ.rnDeriv ν)` where singularPart is mutually singular with ν; defines `HaveLebesgueDecomposition` typeclass, `singularPart`, and `rnDeriv` with uniqueness results |
| RadonNikodym.lean | Radon-Nikodym theorem: proves `μ ≪ ν ↔ ν.withDensity (μ.rnDeriv ν) = μ` when HaveLebesgueDecomposition holds; includes properties of rnDeriv such as `rnDeriv_withDensity_left`, `rnDeriv_withDensity_right`, `inv_rnDeriv`, and integral formulas `setLIntegral_rnDeriv` for both Lebesgue and Bochner integrals |
| Hahn.lean | Unsigned Hahn decomposition theorem: for finite measures μ and ν, constructs measurable partition where `ν ≤ μ` on one part and `μ ≤ ν` on the complement; defines `IsHahnDecomposition` predicate characterizing such partitions using measure restriction |
| Exhaustion.lean | Method of exhaustion for measures: for μ and s-finite ν, constructs `μ.sigmaFiniteSetWRT ν` where μ is sigma-finite on this set, and for all subsets of the complement either `ν t = 0` or `μ t = ∞`; includes `sigmaFiniteSet` for a measure relative to itself; foundational for handling non-sigma-finite measures |
| IntegralRNDeriv.lean | Integral inequalities for Radon-Nikodym derivatives: proves Jensen's inequality type results for convex continuous functions of rnDeriv, notably `mul_le_integral_rnDeriv_of_ac` showing `ν.real univ * f (μ.real univ / ν.real univ) ≤ ∫ x, f (μ.rnDeriv ν x).toReal ∂ν` when μ ≪ ν |

## Subdirectories

(none)

## Search Tags

lebesgue-decomposition radon-nikodym hahn-decomposition measure-decomposition singular-part rnDeriv absolute-continuity mutual-singularity withDensity exhaustion sigma-finite s-finite density-function jensen-inequality convex-function integral-inequality
