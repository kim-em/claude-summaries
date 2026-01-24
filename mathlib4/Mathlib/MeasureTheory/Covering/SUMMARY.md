---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Covering
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# Covering

## Overview

The `Covering/` directory contains the formalization of covering theorems in measure theory, including the Besicovitch and Vitali covering theorems, and their applications to differentiation of measures. These theorems enable extraction of disjoint subfamilies from collections of sets that cover a space almost everywhere, which is fundamental for proving the Radon-Nikodym theorem, Lebesgue density theorem, and Lebesgue differentiation theorem. The directory establishes the abstract notion of Vitali families and provides concrete implementations via both the Besicovitch covering theorem (for finite-dimensional spaces) and the Vitali covering theorem (for doubling measures).

## Key Files

| File | Purpose |
|------|---------|
| VitaliFamily.lean | Abstract Vitali family structure: defines the general framework where for each point one has a family of measurable sets with nonempty interiors from which disjoint almost-everywhere coverings can be extracted, serves as the foundation for measure differentiation theorems |
| Vitali.lean | Classical Vitali covering theorem: proves that from any family of sets with bounded size function, one can extract a disjoint subfamily whose enlargements cover all original sets; constructs a concrete Vitali family for doubling measures using sets that cover a fixed proportion of balls around them |
| Besicovitch.lean | Topological and measurable Besicovitch covering theorems: defines satellite configurations (technical obstructions to covering), proves that in spaces without satellite configurations one can extract N disjoint families covering all centers, and deduces the measurable version for almost-everywhere covering by disjoint balls |
| BesicovitchVectorSpace.lean | Besicovitch theorem specialization to vector spaces: proves the Füredi-Loeb result that the optimal number of covering families equals the multiplicity (maximum number of 1-separated points in the ball of radius 2), shows multiplicity ≤ 5^dim, establishes HasBesicovitchCovering for finite-dimensional real vector spaces |
| Differentiation.lean | Main differentiation theorem: proves VitaliFamily.ae_tendsto_rnDeriv showing that for a Vitali family, the ratio ρ(a)/μ(a) converges almost everywhere to the Radon-Nikodym derivative as sets shrink to a point, includes Lebesgue density theorem (ae_tendsto_measure_inter_div) and Lebesgue differentiation theorem (ae_tendsto_average_norm_sub) |
| DensityTheorem.lean | Lebesgue density theorem for uniformly locally doubling measures: constructs a Vitali family for such measures, proves that μ(S ∩ Bⱼ)/μ(Bⱼ) → 1 for almost all x ∈ S as balls Bⱼ shrink to x even when centers vary, provides versions for measure convergence and function averaging |
| LiminfLimsup.lean | Liminf/limsup results for uniformly locally doubling measures: proves Cassels' lemma that the limsup of thickenings of a sequence of sets is unchanged almost everywhere when distance sequences are scaled by positive factors, applies Lebesgue density theory to thickening operations |
| OneDim.lean | One-dimensional API extension: shows that closed intervals belong to the Vitali family for Lebesgue measure on ℝ, proves convergence of intervals to points along the Vitali family filter, enables application of general covering theorems to interval-based arguments in real analysis |

## Subdirectories

None.

## Search Tags

covering-theorem vitali-family vitali-covering besicovitch-covering satellite-configuration differentiation-of-measures radon-nikodym-derivative lebesgue-density-theorem lebesgue-differentiation-theorem doubling-measure uniformly-locally-doubling fine-subfamily disjoint-covering almost-everywhere-covering measure-differentiation furedi-loeb multiplicity liminf-limsup cassels-lemma
