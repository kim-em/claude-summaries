---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Group
generated: 2026-01-25T22:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 17
subdirs_count: 0
---

# Group

## Overview

The `Group/` directory contains the complete formalization of measure theory on groups and group actions in mathlib4. It provides the theory of invariant measures (measures invariant under left/right multiplication or group actions), Haar measure fundamentals, fundamental domains for group actions, convolution of measures, integration on groups (both Bochner and Lebesgue), and specialized topics including the modular character, Følner filters for amenable groups, geometry of numbers (Blichfeldt and Minkowski theorems), and measure-theoretic properties of the additive circle. The root file `Defs.lean` defines core typeclasses for invariant measures, while other files develop integration theory, product measures on groups, and applications.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core typeclass definitions for invariant measures: defines `SMulInvariantMeasure` (measures invariant under scalar multiplication), `VAddInvariantMeasure` (additive version), `IsMulLeftInvariant`/`IsMulRightInvariant` (measures invariant under left/right group multiplication), and their additive versions `IsAddLeftInvariant`/`IsAddRightInvariant` |
| Measure.lean | Properties of left/right invariant measures on groups: proves measure-preserving properties of translations, develops the inverse measure `μ.inv` (mapping `A ↦ μ(A⁻¹)`), defines the `IsHaarMeasure` typeclass (left-invariant measures that are finite on compact sets and positive on open sets), and proves uniqueness theorems for Haar measures up to scalar multiplication |
| Action.lean | Measures invariant under group actions: proves that scalar multiplication is measure-preserving, develops the almost-everywhere filter for invariant measures, defines minimality and ergodicity for group actions, and proves that `μ((c • ·)⁻¹' s) = μ(s)` for invariant measures and measurable sets |
| FundamentalDomain.lean | Fundamental domains for group actions: defines `IsFundamentalDomain` (sets whose translates cover the space and are pairwise a.e. disjoint), proves that any two fundamental domains have the same measure, shows integrals over fundamental domains are equal, defines `fundamentalInterior` and `fundamentalFrontier`, introduces the `HasFundamentalDomain` typeclass for defining covolume, and the `QuotientMeasureEqMeasurePreimage` typeclass for computing quotient measures |
| Arithmetic.lean | Measurability typeclasses for group operations: defines `MeasurableMul`, `MeasurableAdd`, `MeasurableMul₂`, `MeasurableAdd₂` (typeclasses for measurability of multiplication/addition), `MeasurableDiv`, `MeasurableSub`, `MeasurableInv`, `MeasurableNeg`, and provides dot-style lemmas (`Measurable.mul`, `AEMeasurable.add`, etc.) for composing measurable functions with group operations |
| Convolution.lean | Multiplicative and additive convolution of measures: defines `mconv` (multiplicative convolution, the map of `*` under product measure) with notation `μ ∗ₘ ν`, defines `conv` (additive convolution, the map of `+` under product measure) with notation `μ ∗ ν`, proves Lebesgue integral formulas for convolutions, and establishes that `dirac` is the identity for convolution |
| Integral.lean | Bochner integration on groups: proves integrability is preserved under group translations and inversion (`Integrable.comp_mul_left`, `Integrable.comp_inv`), shows that translating functions doesn't change integrals for invariant measures (`∫ x, f(gx) ∂μ = ∫ x, f(x) ∂μ` for left-invariant `μ`), proves integrals vanish when functions are negated by translations, and handles integration over intervals and inverse sets |
| IntegralConvolution.lean | Bochner integrals of convolutions: proves `integrable_conv_iff` (a function is integrable w.r.t. `μ ∗ ν` iff `y ↦ f(x+y)` is integrable w.r.t. `ν` for `μ`-a.e. `x` and `x ↦ ∫ y, ‖f(x+y)‖ ∂ν` is integrable w.r.t. `μ`), and proves `integral_conv` (the formula `∫ x, f x ∂(μ ∗ ν) = ∫ x, ∫ y, f(x+y) ∂ν ∂μ`) |
| LIntegral.lean | Lebesgue integration on groups: proves `lintegral_inv_eq_self` (Lebesgue integrals are invariant under `x ↦ x⁻¹` for inverse-invariant measures), proves `lintegral_mul_left_eq_self` and `lintegral_mul_right_eq_self` (translation invariance for left/right invariant measures), and shows that for nonzero regular left-invariant measures, the integral of a continuous nonnegative function is zero iff the function is zero |
| FoelnerFilter.lean | Følner sequences and filters for amenable groups: defines `IsFoelner G μ l F` (a sequence of sets is Følner if sets have finite nonzero measure and `μ((g • F i) ∆ F i) / μ(F i) → 0` for all `g`), defines `maxFoelner G μ` (the maximal Følner filter), proves `IsFoelner.amenable` (existence of Følner filters implies existence of `G`-invariant finitely additive probability measures), and characterizes Følner sequences via convergence to the maximal Følner filter |
| ModularCharacter.lean | Modular character of locally compact groups: defines `modularCharacterFun g = μ(· * g⁻¹) / μ` for Haar measure `μ`, proves independence from the choice of Haar measure, and defines `modularCharacter : G →* ℝ≥0` as a group homomorphism (unimodular groups are those where the modular character is trivial) |
| AEStabilizer.lean | Almost-everywhere stabilizer of sets under group actions: defines `MulAction.aestabilizer G μ s` (the subgroup of elements `g` such that `g • s =ᵐ[μ] s`), proves it's a subgroup containing the point stabilizer, shows it equals `⊤` for null or conull sets, and provides `aestabilizer_congr` (stabilizer is invariant under a.e. equivalence of sets) |
| AddCircle.lean | Measure theory on the additive circle: proves `closedBall_ae_eq_ball` (open and closed balls are almost equal in the additive circle), proves `isAddFundamentalDomain_of_ae_ball` (balls are fundamental domains for rational angle rotation), and provides `volume_of_add_preimage_eq` (formula for volumes of rotation-invariant sets in terms of their intersection with a fundamental domain) |
| GeometryOfNumbers.lean | Blichfeldt's theorem and Minkowski's convex body theorem: proves `exists_pair_mem_lattice_not_disjoint_vadd` (Blichfeldt: if covolume of a lattice is less than volume of a set, two distinct lattice translates of the set must overlap), proves `exists_ne_zero_mem_lattice_of_measure_mul_two_pow_lt_measure` (Minkowski: convex symmetric domain of large enough volume contains a nonzero lattice point), and provides the compact version with non-strict inequality |
| MeasurableEquiv.lean | Group operations as measurable equivalences: defines `MeasurableEquiv.smul c` (scalar multiplication as measurable automorphism), `MeasurableEquiv.mulLeft g` and `MeasurableEquiv.mulRight g` (left/right multiplication as measurable automorphisms), `MeasurableEquiv.inv` (inversion as measurable automorphism), and proves corresponding measurable embedding lemmas |
| Pointwise.lean | Pointwise set operations preserve measurability: proves `MeasurableSet.const_smul` (if `s` is measurable then `a • s` is measurable), `MeasurableSet.const_smul_of_ne_zero` (for groups with zero), and `MeasurableSet.const_smul₀` (for mul-actions with zero, handling the zero case via `MeasurableSingletonClass`) |
| Prod.lean | Measure theory on products of groups: defines measurable equivalences `MeasurableEquiv.shearMulRight` (the map `(x,y) ↦ (x,xy)`) and `MeasurableEquiv.shearDivRight` (the map `(x,y) ↦ (x,y/x)`), proves `measurePreserving_prod_mul` (the shear map preserves `μ × ν` when `ν` is left-invariant), proves uniqueness of left-invariant measures up to scaling using iterated integrals, and follows Halmos's proof that for left-invariant `μ` and `ν`, the ratio `μ(t)/μ(s)` equals `ν(t)/ν(s)` |

## Subdirectories

None

## Search Tags

measure-theory groups haar-measure invariant-measure left-invariant right-invariant group-action fundamental-domain convolution integration bochner-integral lebesgue-integral modular-character foelner-filter amenable-group additive-circle geometry-of-numbers blichfeldt-theorem minkowski-theorem measurable-group measurable-multiplication product-measure aestabilizer smul-invariant
