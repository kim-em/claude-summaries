---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/VectorMeasure/Decomposition
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Decomposition

## Overview

The `Decomposition/` directory formalizes the four fundamental decomposition theorems for signed measures and vector measures: the Hahn decomposition theorem (signed measures can be decomposed into positive and negative parts on complementary sets), the Jordan decomposition theorem (signed measures uniquely decompose into mutually singular positive and negative measures), the Lebesgue decomposition theorem (signed measures decompose into singular and absolutely continuous parts with respect to a measure), and the Radon-Nikodym theorem (absolutely continuous signed measures have a density). These decomposition theorems form the theoretical foundation for measure-theoretic analysis, enabling the representation and manipulation of signed measures in terms of simpler components.

## Key Files

| File | Purpose |
|------|---------|
| Hahn.lean | Hahn decomposition theorem for signed measures: proves that every signed measure `s` admits a measurable partition of the space into complementary sets `i` and `j` where `i` is positive (`0 ≤[i] s`) and `j` is negative (`s ≤[j] 0`), establishes `exists_isCompl_positive_negative` theorem, proves auxiliary result `exists_subset_restrict_nonpos` showing that sets of negative measure contain negative subsets, uses constructive sequence `restrictNonposSeq` to find maximal negative sets, proves uniqueness property `of_symmDiff_compl_positive_negative` stating symmetric difference of two Hahn decompositions has measure zero |
| Jordan.lean | Jordan decomposition theorem for signed measures: defines `JordanDecomposition α` as a pair of mutually singular finite measures (`posPart` and `negPart`), proves existence via `toJordanDecomposition` constructing the Jordan decomposition from any signed measure, proves uniqueness via `toSignedMeasure_injective` showing Jordan decompositions are uniquely determined by their associated signed measure, establishes `toJordanDecompositionEquiv` equivalence between signed measures and Jordan decompositions, defines total variation `totalVariation` as sum of positive and negative parts, provides scalar multiplication and negation operations on Jordan decompositions, proves that Jordan decompositions provide Hahn decompositions via `exists_compl_positive_negative` |
| JordanSub.lean | Jordan decomposition for measure subtraction: proves that for finite measures `μ` and `ν`, the signed measure `μ.toSignedMeasure - ν.toSignedMeasure` has Jordan decomposition `(μ - ν, ν - μ)` via `toJordanDecomposition_toSignedMeasure_sub`, establishes mutual singularity `mutually_singular_measure_sub` of the measures `μ - ν` and `ν - μ`, proves `sub_toSignedMeasure_eq_toSignedMeasure_sub` connecting measure subtraction to signed measure subtraction, uses Hahn decomposition as key tool via `IsHahnDecomposition` to partition space where `μ ≤ ν` and `ν ≤ μ`, provides `jordanDecompositionOfToSignedMeasureSub` constructor for this special Jordan decomposition |
| Lebesgue.lean | Lebesgue decomposition theorem for signed measures: defines `HaveLebesgueDecomposition` typeclass indicating signed measure has Lebesgue decomposition with respect to a measure, defines `singularPart s μ` as the mutually singular component of signed measure `s` with respect to measure `μ`, defines `rnDeriv s μ` as the Radon-Nikodym derivative (density function) of `s` with respect to `μ`, proves main theorem `singularPart_add_withDensity_rnDeriv_eq` establishing `s.singularPart μ + μ.withDensityᵥ (s.rnDeriv μ) = s`, proves uniqueness results `eq_singularPart` and `eq_rnDeriv` showing the decomposition is unique, establishes linearity properties (addition, subtraction, scalar multiplication) of singular part and Radon-Nikodym derivative, extends to complex measures via `ComplexMeasure.HaveLebesgueDecomposition`, `ComplexMeasure.singularPart`, and `ComplexMeasure.rnDeriv` |
| RadonNikodym.lean | Radon-Nikodym theorem for signed measures: proves `withDensityᵥ_rnDeriv_eq` stating that if `s ≪ᵥ μ` (absolute continuity), then `μ.withDensityᵥ (s.rnDeriv μ) = s`, establishes `absolutelyContinuous_iff_withDensityᵥ_rnDeriv_eq` characterizing absolute continuity as equivalence between signed measure and its with-density reconstruction, proves `withDensityᵥ_rnDeriv_smul` for composition of Radon-Nikodym derivatives with scalar multiplication, connects signed measure Radon-Nikodym theory to the underlying measure-theoretic Radon-Nikodym theorem via imports from `Mathlib.MeasureTheory.Measure.Decomposition.RadonNikodym`, requires σ-finiteness for main theorems |

## Subdirectories

(No subdirectories)

## Search Tags

hahn-decomposition jordan-decomposition lebesgue-decomposition radon-nikodym signed-measure vector-measure mutually-singular absolute-continuity singular-part density rn-deriv positive-part negative-part total-variation decomposition-theorems measure-theory
