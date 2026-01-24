---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Function
generated: 2026-01-25T23:55:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 25
subdirs_count: 7
---

# Function

## Overview

The `Function/` directory contains a comprehensive theory of measurable functions and their properties in measure theory. At its foundation are strongly measurable functions (approximable by simple functions) and their almost everywhere variants, which enable Bochner integration. The directory develops the complete theory of Lp spaces for 1 ≤ p ≤ ∞, including the Lp seminorm hierarchy with triangle inequalities and comparison theorems, completeness of Lp metric spaces, and embeddings of continuous functions. L¹ functions (integrable functions) receive special treatment as both a fundamental Lp space and a foundation for more general integration theory. The L⁰ space of almost everywhere equal functions provides the quotient structure underlying all Lp spaces, with support for group actions via measure-preserving domain transformations. Conditional expectation is developed through a four-stage construction (L² projection, indicators, L¹ extension, general integrability) with uniqueness theorems and connections to Radon-Nikodym derivatives. Advanced topics include simple function density theorems, essential supremum/infimum for L∞ norms, multiple convergence modes (in measure, in distribution, almost everywhere), Egorov's theorem on uniform convergence, locally integrable functions, uniform integrability with the Vitali convergence theorem, change of variables formulas using Jacobians (both one-dimensional and higher-dimensional), Hölder's inequality for bilinear maps on Lp spaces, and measurability theory for special functions (exponential, logarithmic, trigonometric, inner products).

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

- [x] `AEEqFun/` - Group actions on almost everywhere equal functions via measure-preserving domain transformations (DomMulAct, DomAddAct)
- [x] `ConditionalExpectation/` - Conditional expectation operator constructed via L² projection, then extended to indicators, L¹, and general integrable functions; includes uniqueness theorems, pull-out properties, and Radon-Nikodym connections
- [x] `L1Space/` - Integrable functions and L¹ space: HasFiniteIntegral predicate, Integrable predicate (AE strongly measurable + finite integral), API between integrable functions and L¹ elements, dominated convergence
- [x] `LpSeminorm/` - Foundational Lp seminorm theory: eLpNorm definitions for 0 < p < ∞ and p = ∞, triangle inequalities with optimal constants, comparison inequalities between exponents, Chebyshev-Markov inequality, behavior under product measures and trimming
- [x] `LpSpace/` - Lp spaces as equivalence classes with finite eLpNorm: completeness for 1 ≤ p, embeddings of bounded continuous functions, composition with measure-preserving maps, indicator functions, domain group actions
- [x] `SpecialFunctions/` - Measurability and integrability of standard mathematical functions: exponential, logarithm, trigonometric, hyperbolic, power functions, arctan, inner products, RCLike operations, sinc function
- [x] `StronglyMeasurable/` - Foundation for Bochner integration: strongly measurable functions (approximable by simple functions), finitely strongly measurable (with finite support measure), almost everywhere variants, connections to Lp spaces and sigma-finite sets

## Search Tags

measurable-function ae-equal l0-space simple-function lp-space lp-seminorm elpnorm essential-supremum convergence-in-measure convergence-in-distribution egorov-theorem locally-integrable conditional-expectation uniform-integrability vitali-convergence jacobian change-of-variables holder-inequality ae-measurable strongly-measurable finitely-strongly-measurable density-theorem bochner-integral l1-space l2-space integrable has-finite-integral dominated-convergence triangle-inequality chebyshev-markov memlp complete-metric-space orthogonal-projection sub-sigma-algebra indicator-function pull-out-property radon-nikodym-derivative domain-action measure-preserving special-functions exponential logarithm trigonometric inner-product sigma-finite ae-strongly-measurable simple-function-approximation lpMeas trim-measure product-measure comparison-inequality
