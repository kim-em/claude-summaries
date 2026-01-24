---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Integral/Bochner
generated: 2026-01-25T08:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# Bochner

## Overview

The `Bochner/` directory contains the foundational theory of the Bochner integral, which extends Lebesgue integration to functions valued in Banach spaces (complete normed vector spaces). It constructs the integral via a four-step process: defining integrals on set indicators via weighted scalar multiplication, extending to simple functions, transferring to L¹ simple functions with continuity, and finally extending to all L¹ functions via density and continuous extension. The directory includes core linearity and order properties, the fundamental theorem of calculus for set integrals, composition with continuous linear maps, set integration theory (with the `∫ x in s, f x ∂μ` notation), and the Vitali-Carathéodory approximation theorem (approximating integrable functions by semicontinuous functions with controlled integral error).

## Key Files

| File | Purpose |
|------|---------|
| L1.lean | L¹ space construction of Bochner integral: defines `weightedSMul` (set indicator integral `μ.real s • x`), extends through simple functions to L¹ functions via `ContinuousLinearMap.extend`, proves `DominatedFinMeasAdditive` property needed for extension via `setToL1`, notation `α →₁ₛ[μ] E` for simple functions in L¹ |
| Basic.lean | Main Bochner integral API and properties: defines `∫ a, f a ∂μ` as Bochner integral (evaluates to integral of L¹ equivalence class, or 0 if not integrable), proves linearity (`integral_add`, `integral_smul`), order properties (`integral_mono_ae`), connection to Lebesgue integral (`integral_eq_lintegral_pos_part_sub_lintegral_neg_part`), norm inequality (`norm_integral_le_integral_norm`), with induction principles for proving properties via simple function approximation |
| Set.lean | Set integration theory and theorems: properties of `∫ x in s, f x ∂μ` notation (defined as `∫ x, f x ∂(μ.restrict s)`), proves equivalence `integral_indicator` (set integral equals indicator integral for measurable sets), decomposition theorems (`setIntegral_union`, `setIntegral_empty`, `setIntegral_univ`), `IntegrableOn f s μ` predicate, congruence and manipulation lemmas for integrals over sets |
| ContinuousLinearMap.lean | Integration commutes with continuous linear maps: proves `L.integral_comp_comm` stating `∫ x, L(φ x) ∂μ = L(∫ x, φ x ∂μ)` for continuous linear map `L : E →L[𝕜] F` and integrable `φ`, uses `compLp` construction for composition on L¹ classes, includes `integral_apply` for applying pointwise to continuous linear map-valued integrals, proved via induction on simple functions with continuity closure |
| FundThmCalculus.lean | Fundamental theorem of calculus for set integrals: proves `integral_sub_linear_isLittleO_ae` showing `∫ x in s, f x ∂μ = μ.real s • c + o(μ.real s)` when `f → c` at measurably generated filter `l`, versions for `nhdsWithin` (`ContinuousWithinAt.integral_sub_linear_isLittleO_ae`) and continuity at points, asymptotic formula relating set integrals to limits for locally finite measures |
| VitaliCaratheodory.lean | Vitali-Carathéodory approximation theorem: for integrable `f : α → ℝ` on regular σ-finite measure space, proves existence of semicontinuous approximations with strict inequalities (`exists_lt_lower_semicontinuous_integral_lt` for `f < g` lower semicontinuous, `exists_upper_semicontinuous_lt_integral_gt` for upper semicontinuous `g < f`) and integrals arbitrarily close to `∫ f`, proved via series of simple functions with open/closed set approximations by regularity |

## Subdirectories

*(No subdirectories)*

## Search Tags

bochner-integral banach-space-valued l1-space simple-functions weighted-smul dominated-fin-meas-additive set-integral integrable-on continuous-linear-map integral-commutes fundamental-theorem-calculus vitali-caratheodory semicontinuous-approximation regular-measure linearity monotonicity lintegral measure-theory integration
