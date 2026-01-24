---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Measure/Lebesgue
generated: 2026-01-25T08:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Lebesgue

## Overview

The `Lebesgue/` directory contains the formalization of Lebesgue measure on ℝ, ℝⁿ, and ℂ as a special case of additive Haar measure on inner product spaces. It establishes that the volume measure on the real line coincides with the Stieltjes measure for the identity function, and extends this to product spaces and finite-dimensional real vector spaces. The directory provides key properties including: volume formulas for intervals and balls, transformation behavior under linear maps (rescaling by the determinant), measure-theoretic properties of the region between two functions, integration substitutions, and explicit computations of volumes for balls in Euclidean spaces, complex spaces, and Lᵖ spaces. The equivalence between Haar measure and Lebesgue measure enables powerful results about linear transformations, density points, and regularity.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Foundational definitions establishing that Lebesgue measure on ℝ equals the Stieltjes measure for the identity function; provides volume formulas for all interval types (Icc, Ico, Ioc, Ioo), balls, and boxes in ℝⁿ; proves transformation formulas for linear maps on ℝⁿ (volume rescales by determinant), transvection preservation, and diagonal matrix scaling; defines the `regionBetween` construction for sets between two functions with measurability and volume results |
| Complex.lean | Defines measurable equivalences between ℂ and ℝ² (both as Fin 2 → ℝ and ℝ × ℝ) and proves these equivalences are volume-preserving, establishing that the inner product space volume on ℂ equals the product Lebesgue measure on ℝ² |
| EqHaar.lean | Proves that Haar measure equals Lebesgue measure on ℝ and ℝⁿ (`addHaarMeasure_eq_volume`); extends transformation properties to arbitrary finite-dimensional real vector spaces (linear maps rescale measure by absolute determinant via `map_linearMap_addHaar_eq_smul_addHaar`); establishes that strict subspaces have zero measure, spheres have zero measure, and balls have volume `rᵈ · μ(ball 0 1)` where d is dimension; proves density point theorems showing that Lebesgue density points have density one for rescaled copies of any measurable set; defines the measure associated to an alternating map |
| Integral.lean | Integration properties with respect to Lebesgue measure: proves that the volume of the region between two integrable functions equals the integral of their difference (`volume_regionBetween_eq_integral`); provides integrability criteria for functions on ℝ via summable norms on unit intervals; establishes substitution formulas for integration with `-x` transformation |
| VolumeOfBalls.lean | Computes explicit volumes of unit balls in various spaces: provides general formula `μ(ball 0 1) = ∫exp(-‖x‖ᵖ)dμ / Γ(dim/p + 1)` for any p > 0; calculates volumes for Lᵖ balls over ℝⁿ and ℂⁿ in terms of Gamma functions; gives concrete formulas for Euclidean spaces (involving √π and Gamma functions), including special cases for ℝ² (πr²), ℝ³ (4πr³/3), and ℂ (πr²); supports both open and closed balls with formulas distinguishing even and odd dimensions |

## Subdirectories

_(No subdirectories)_

## Search Tags

lebesgue-measure haar-measure volume stieltjes-measure real-line euclidean-space finite-dimensional determinant linear-map transformation measure-preserving balls intervals region-between integration density-point complex-plane product-measure gamma-function lp-space inner-product-space
