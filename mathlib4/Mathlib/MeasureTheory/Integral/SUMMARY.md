---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Integral
generated: 2026-01-25T23:59:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 27
subdirs_count: 5
---

# Integral

## Overview

The `Integral/` directory contains the comprehensive formalization of integration theory in mathlib4, providing two foundational integral theories: the Lebesgue integral (`∫⁻`) for extended non-negative real-valued functions (serving as the computational foundation) and the Bochner integral (`∫`) for Banach space-valued functions (constructed via extension from simple functions through L¹ space). The directory establishes fundamental convergence theorems (monotone convergence, dominated convergence for both integral types), measure-theoretic properties (Fubini's theorem for product measures, behavior under measure-preserving maps), and the crucial connection between these two integral theories.

Beyond the core integration machinery, the directory contains specialized integration contexts: interval integration on ℝ with the fundamental theorems of calculus (FTC-1 for derivatives of integrals, FTC-2 for integrals of derivatives), integration techniques (by parts, change of variables), curve integrals for 1-forms with Poincaré's lemma, circle and torus integrals for complex analysis, and improper integration theory linking proper integrals to limits over unbounded domains. Advanced topics include the layer cake formula (Cavalieri's principle), integration against approximations of identity (peak functions), mean inequalities (Hölder, Minkowski), the divergence theorem on boxes, the Vitali-Carathéodory approximation theorem, and the Riesz-Markov-Kakutani representation theorem connecting positive linear functionals on compactly supported continuous functions to regular measures.

## Key Files

| File | Purpose |
|------|---------|
| SetToL1.lean | Extension of linear functions from set indicators to L1 spaces: constructs continuous linear map `(α →₁[μ] E) →L[ℝ] F` from `DominatedFinMeasAdditive` operators, used to define both Bochner integral and conditional expectation, with linearity and order-preservation properties |
| FinMeasAdditive.lean | Additivity on measurable sets with finite measure: defines `FinMeasAdditive` (additivity property for disjoint measurable sets) and `DominatedFinMeasAdditive` (with norm bound by measure), the foundational property needed to extend set functions to L1 |
| DominatedConvergence.lean | Lebesgue dominated convergence theorem for Bochner integrals: proves that almost everywhere convergence of sequence `Fₙ → f` with integrable dominating function implies `∫ Fₙ → ∫ f`, with variants for filters and series (including `hasSum_integral_of_dominated_convergence` and `integral_tsum`) |
| IntegralEqImproper.lean | Links between proper and improper integrals: defines `AECover` (technical condition for approximating integrals over unbounded sets by bounded ones), proves convergence theorems relating `∫ x, f x ∂μ` to limits of `∫ x in φ n, f x ∂μ`, includes FTC-2 on `(a, +∞)` and change of variables on semi-infinite intervals |
| IntegrableOn.lean | Integrability on sets and at filters: defines `IntegrableOn f s μ := Integrable f (μ.restrict s)` and `IntegrableAtFilter` (integrable on some set in the filter), proves union/intersection decomposition theorems and boundedness criteria |
| Prod.lean | Integration on product measures (Fubini's theorem): proves `∫ z, f z ∂(μ.prod ν) = ∫ x, ∫ y, f (x, y) ∂ν ∂μ` for integrable functions on product spaces, includes characterization `integrable_prod_iff` and non-σ-finite version for compactly supported continuous functions |
| Layercake.lean | Layer cake formula / Cavalieri's principle: proves `∫ (G ∘ f) ∂μ = ∫ g(t) * μ{ω | f(ω) ≥ t} dt` for non-negative functions, where `G' = g`, includes standard form `∫ f ∂μ = ∫ μ{f ≥ t} dt` and variants with strict inequality |
| Average.lean | Integral averages of functions: defines `⨍ x, f x ∂μ` (average value) as `∫ x, f x ∂((μ univ)⁻¹ • μ)`, both Bochner and Lebesgue versions, proves first moment method (integrable function is below/above average on positive measure set) |
| CircleIntegral.lean | Complex circle integrals: defines `∮ z in C(c, R), f z` as integral around circle `{z | |z - c| = |R|}`, proves formulas for `∮ (z - w)^n` (zero unless n = -1 with w inside, then 2πi), defines Cauchy power series with convergence on open disc |
| TorusIntegral.lean | Multidimensional torus integrals in ℂⁿ: defines `torusMap c R θ` (maps ℝⁿ to ℂⁿ via `zₖ = cₖ + Rₖ e^{θₖ i}`) and `∯ z in T(c, R), f z` for integration over generalized torus, with dimension-specific reduction formulas |
| CircleAverage.lean | Averages over circles in metric spaces: defines average value of function over sphere `{y | dist x y = R}`, proves continuity and differentiability properties, applications to harmonic functions |
| CircleTransform.lean | Circle transform operations: transformations and manipulations related to circle integrals and circular averaging |
| MeanInequalities.lean | Hölder and Minkowski inequalities for integrals: proves `∫ (f * g) ∂μ ≤ (∫ f^p)^(1/p) * (∫ g^q)^(1/q)` for conjugate exponents, both for ENNReal and NNReal functions, generalizations to finite products with weighted exponents |
| PeakFunction.lean | Integration against approximations of identity: proves that `∫ φₙ • g` tends to `g(x₀)` when `φₙ` are peak functions concentrating at `x₀` (with average one), includes power concentration `(c^n) / ∫ c^n` and rescaling `c^d * φ(c • x)` versions |
| Gamma.lean | Integrals involving the Gamma function: evaluates `∫ x^q * exp(-x^p) dx` and variants in terms of `Real.Gamma`, applications to special function theory |
| DivergenceTheorem.lean | Divergence theorem for Bochner integral on boxes in ℝⁿ⁺¹: proves integral of divergence over box `[a, b]` equals sum of boundary integrals, allows countably many non-differentiability points, includes versions for ℝ → E and (ℝ × ℝ) → E |
| Indicator.lean | Integration of indicator functions: properties and theorems for integrals of characteristic functions of sets, fundamental building blocks for simple functions |
| Marginal.lean | Marginal distributions and integrals: integration over marginal measures in product spaces, relationship to conditional integration |
| MeanValue.lean | Mean value theorems for integrals: integral versions of classical mean value theorems from calculus |
| IntervalAverage.lean | Average values over intervals: specialization of average to interval integrals, `⨍ x in a..b, f x` notation and properties |
| Pi.lean | Integration for Pi types: integration of functions valued in product spaces `Π i, E i`, component-wise integration theorems |
| Regular.lean | Regular measures and integration: properties of integrals with respect to regular measures (inner/outer regular) |
| Asymptotics.lean | Asymptotic behavior of integrals: big-O and little-o estimates for integrals as parameters vary |
| ExpDecay.lean | Integrals with exponential decay: integrability and estimates for functions with exponential decay at infinity |
| BoundedContinuousFunction.lean | Integration of bounded continuous functions: properties specific to integrating functions from the bounded continuous function space |
| CompactlySupported.lean | Integration of compactly supported functions: specialized theorems for functions with compact support |
| LebesgueNormedSpace.lean | Lebesgue integration in normed spaces: connections between Lebesgue integral theory and normed space structure |

## Subdirectories

- [x] `Bochner/` - Bochner integral for Banach space-valued functions, constructed via four-step extension process (set indicators → simple functions → L¹ simple functions → all L¹ functions), including integration on sets (`∫ x in s, f x`), composition with continuous linear maps, FTC for set integrals, and Vitali-Carathéodory approximation by semicontinuous functions
- [x] `Lebesgue/` - Lebesgue integral (`∫⁻`) for extended non-negative real-valued functions, defined as supremum over simple functions, including monotone convergence (Beppo Levi), dominated convergence, additivity/subtraction, behavior under maps and equivalences, Markov's inequality, and specializations to finite/countable types and measures
- [x] `IntervalIntegral/` - Interval integration on ℝ with notation `∫ x in a..b, f x`, establishing both fundamental theorems of calculus (FTC-1 for derivatives of integrals with respect to endpoints, FTC-2 for integrals of derivatives), integration techniques (by parts, change of variables), specialized results (trapezoidal rule, Lebesgue differentiation, mean value theorems, periodic functions), and derivative integrability for monotone and bounded variation functions
- [~] `RieszMarkovKakutani/` - Riesz-Markov-Kakutani representation theorem establishing bijective correspondence between positive linear functionals on compactly supported continuous functions and regular measures on locally compact T2 spaces, proven for both ℝ≥0-linear functionals (with both Bochner and Lebesgue integral formulations) and ℝ-linear functionals, including uniqueness and regularity properties
- [x] `CurveIntegral/` - Curve integrals (line integrals) for 1-forms along paths in normed spaces with notation `∫ᶜ x in γ, ω x`, establishing fundamental properties (additivity, reversal, composition under path operations), derivative formulas for segment integrals, and Poincaré's lemma for convex sets showing closed 1-forms admit primitives via homotopy invariance

## Search Tags

integration bochner-integral lebesgue-integral dominated-convergence fubini-theorem circle-integral torus-integral interval-integral improper-integral layer-cake-formula cavalieri gamma-function holder-inequality minkowski-inequality peak-function approximation-of-identity divergence-theorem mean-value-theorem riesz-markov-kakutani ftc fundamental-theorem-calculus integration-by-parts change-of-variables integrable-on average curve-integral line-integral
