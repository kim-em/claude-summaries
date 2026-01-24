---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Function
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 25
subdirs_count: 7
---

# Function

## Overview

The `Function/` directory contains the theory of measurable functions and their properties in measure theory. This includes almost everywhere equality classes (L⁰ space), simple functions and their density properties, Lp spaces and their seminorms, essential supremum and infimum, convergence modes (in measure, in distribution, almost everywhere), locally integrable functions, conditional expectation, uniform integrability and the Vitali convergence theorem, change of variables formulas with Jacobians, and Hölder's inequality for bilinear maps on Lp spaces.

## Key Files

| File | Purpose |
|------|---------|
| AEEqFun.lean | Almost everywhere equal functions (L⁰ space): equivalence classes of almost everywhere strongly measurable functions, with linear and order structure, composition operations |
| AEEqOfIntegral.lean | Almost everywhere equality from integral: conditions under which functions are equal almost everywhere based on integral properties |
| AEEqOfLIntegral.lean | Almost everywhere equality from Lebesgue integral: characterizations of AE equality using the Lebesgue integral |
| AEMeasurableOrder.lean | Almost everywhere measurable functions with order structure: properties of measurability combined with order relations |
| AEMeasurableSequence.lean | Almost everywhere measurable sequences: properties of sequences of measurable functions |
| AbsolutelyContinuous.lean | Absolutely continuous functions: functions whose measures of preimages are absolutely continuous with respect to the base measure |
| ContinuousMapDense.lean | Density of continuous maps: theorems showing continuous functions are dense in various function spaces |
| ConvergenceInDistribution.lean | Convergence in distribution: weak convergence of measures and functions, used in probability theory |
| ConvergenceInMeasure.lean | Convergence in measure: sequences of functions converging in measure, relations with AE convergence and Lp convergence, used in weak law of large numbers |
| Egorov.lean | Egorov's theorem: almost everywhere convergent sequences on finite measure spaces converge uniformly except on arbitrarily small sets |
| EssSup.lean | Essential supremum and infimum: smallest c such that f(x) ≤ c almost everywhere, used to define L∞ norm |
| FactorsThrough.lean | Functions factoring through measurable spaces: characterization of when a function factors through a coarser measurable structure |
| Floor.lean | Floor function measurability: properties of floor and related functions in measure theory |
| Holder.lean | Hölder's inequality for bilinear maps: continuous bilinear maps on Lp spaces with Hölder conjugate exponents, pairing between dual Lp spaces |
| Intersectivity.lean | Intersectivity of set families: properties of collections of sets related to measurability |
| Jacobian.lean | Change of variables in higher-dimensional integrals: Jacobian formula for measure under differentiable injective maps, relates μ(f(s)) to integral of |det(f')|, Sard's lemma |
| JacobianOneDim.lean | Change of variables in one dimension: specialized Jacobian formulas using derivatives instead of Fréchet derivatives, versions for monotone/antitone functions |
| L2Space.lean | L² space: Hilbert space structure on square-integrable functions |
| LocallyIntegrable.lean | Locally integrable functions: functions integrable on neighborhoods of every point, integrability on compact sets |
| LpOrder.lean | Order structure on Lp spaces: lattice properties and order relations for Lp functions |
| SimpleFunc.lean | Simple functions: functions with finite range and measurable fibers, approximation of measurable functions by simple functions, induction principle for ℝ≥0∞-valued measurable functions |
| SimpleFuncDense.lean | Density of simple functions: simple functions are dense in various topologies and function spaces |
| SimpleFuncDenseLp.lean | Density of simple functions in Lp: approximation theorems showing simple functions are dense in Lp spaces |
| UnifTight.lean | Uniform tightness: families of measures that are uniformly concentrated on compact sets, important for weak convergence |
| UniformIntegrable.lean | Uniform integrability and Vitali convergence theorem: uniform integrability in measure theory and probability theory senses, convergence in Lp characterized by uniform integrability and convergence in measure |

## Subdirectories

- [x] `AEEqFun/` - Additional theory for almost everywhere equal functions
- [x] `ConditionalExpectation/` - Conditional expectation with respect to sub-σ-algebras
- [x] `L1Space/` - L¹ space of integrable functions
- [x] `LpSeminorm/` - Seminorms on Lp spaces and their properties
- [x] `LpSpace/` - Lp spaces for 1 ≤ p ≤ ∞
- [x] `SpecialFunctions/` - Measure theory properties of special functions
- [ ] `StronglyMeasurable/` - Strongly measurable functions and related concepts

## Search Tags

measurable-function ae-equal l0-space simple-function lp-space essential-supremum convergence-in-measure convergence-in-distribution egorov-theorem locally-integrable conditional-expectation uniform-integrability vitali-convergence jacobian change-of-variables holder-inequality ae-measurable strongly-measurable density-theorem
