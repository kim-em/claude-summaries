---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/CStarAlgebra/ContinuousFunctionalCalculus
generated: 2025-12-04T15:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 15
subdirs_count: 0
---

# ContinuousFunctionalCalculus

## Overview

This directory contains the implementation and theory of the continuous functional calculus for C⋆-algebras. The continuous functional calculus allows applying continuous functions to operators, generalizing the polynomial functional calculus. It provides two complementary APIs: a unital version (`cfc`) for unital algebras and a non-unital version (`cfcₙ`) for non-unital algebras, each supporting scalar rings ℂ, ℝ, and ℝ≥0 with appropriate predicates (normal, selfadjoint, nonnegative). The implementation includes the core star algebra homomorphisms, isometric properties, continuity in both variables, integral formulations, spectral mapping theorems, uniqueness results, and applications to product types, commuting elements, and unitary characterizations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Main entry point; constructs the continuous functional calculus `C(spectrum ℂ a, ℂ) ≃⋆ₐ[ℂ] elemental ℂ a` for normal elements via Gelfand transform and `elemental.characterSpaceHomeo`; includes primary instance `IsStarNormal.instContinuousFunctionalCalculus` |
| Unital.lean | Generic API for unital continuous functional calculus; defines `ContinuousFunctionalCalculus` class, `cfcHom` (bundled star algebra homomorphism), and `cfc` (unbundled function taking junk values); includes composition property and spectral mapping theorem |
| NonUnital.lean | Generic API for non-unital continuous functional calculus; defines `NonUnitalContinuousFunctionalCalculus` class, `cfcₙHom`, and `cfcₙ` operating on functions vanishing at zero on quasispectrum; mirrors unital design for non-unital algebras |
| Instances.lean | Constructs instances: `IsSelfAdjoint.instContinuousFunctionalCalculus` (ℝ-calculus for selfadjoint elements from ℂ-calculus for normal elements) and `Nonneg.instContinuousFunctionalCalculus` (ℝ≥0-calculus from ℝ-calculus); includes `cfcₙAux` for pulling back non-unital instances from unitization |
| Isometric.lean | Defines `IsometricContinuousFunctionalCalculus` and `IsometricNonUnitalContinuousFunctionalCalculus` classes extending base classes with isometry requirement; proves `norm_cfcHom`, `nnnorm_cfcHom`, and norm characterization via spectral supremum |
| Continuity.lean | Proves continuity of `cfc` and `cfcₙ` in both variables: `tendsto_cfc_fun` (continuity in function variable with uniform convergence), `Filter.Tendsto.cfc` (continuity in element variable), `lipschitzOnWith_cfc_fun` (Lipschitz constant 1 in function), `continuousOn_cfc`, and joint continuity `continuousOn_cfc_setProd` |
| Order.lean | Order-theoretic results depending on continuous functional calculus in star-ordered rings; proves bounds `IsSelfAdjoint.le_algebraMap_norm_self`, `mul_star_le_algebraMap_norm_sq`, `CStarAlgebra.norm_le_norm_of_nonneg_of_le`, conjugate inequalities, and `cfc_tsub`/`cfcₙ_tsub` for nonnegative functions |
| Integral.lean | Integration and continuous functional calculus commutation; proves `cfc_setIntegral`, `cfc_integral`, `cfcₙ_setIntegral`, `cfcₙ_integral` showing `cfc (∫ x, f x) a = ∫ x, cfc (f x) a` under continuity conditions; includes integrability results for `cfc`/`cfcₙ` applications |
| Unique.lean | Uniqueness of continuous functional calculus via Stone-Weierstrass; proves `ContinuousMap.UniqueHom` instances for ℝ, ℂ, and ℝ≥0 showing star algebra homomorphisms from `C(s, R)` are uniquely determined by their value on the identity function |
| Restrict.lean | Restriction of continuous functional calculus to scalar subrings; defines `SpectrumRestricts.homeomorph`, `SpectrumRestricts.starAlgHom`, and `SpectrumRestricts.cfc` for deriving ℝ-calculus for selfadjoint elements from ℂ-calculus for normal elements via spectrum restriction |
| Commute.lean | Commutation with continuous functional calculus applications; proves `Commute.cfcHom` and `Commute.cfcₙ` showing elements commuting with both `a` and `star a` also commute with `cfc f a`; includes specialized versions for selfadjoint elements and ℝ/ℝ≥0 scalars |
| Range.lean | Range characterization of continuous functional calculus; proves `range_cfcHom` and `range_cfcₙHom` showing range equals elemental subalgebra for RCLike scalars; proves `range_cfc_nnreal` and `range_cfcₙ_nnreal` characterizing nonnegative range for ℝ≥0 |
| Pi.lean | Continuous functional calculus on product types; proves `cfc_map_pi` and `cfcₙ_map_pi` showing `cfc f a = fun i => cfc f (a i)` for indexed products; includes `cfc_map_prod` and `cfcₙ_map_prod` for binary products |
| Unitary.lean | Unitary characterization via continuous functional calculus; proves `cfc_unitary_iff` and `unitary_iff_isStarNormal_and_spectrum_subset_unitary` showing element is unitary iff star-normal with spectrum on unit circle; includes `mem_unitary_of_spectrum_subset_unitary` |
| Note.lean | Library note documentation (`library_note2 «continuous functional calculus»`) explaining design philosophy, class hierarchy diagram (12 classes from 3 scalar rings × unital/non-unital × isometric/non-isometric), and organizational structure within Mathlib |

## Subdirectories

(none)

## Search Tags

continuous-functional-calculus cstar-algebras functional-analysis operator-algebras spectral-theory normal-elements selfadjoint-elements nonnegative-elements unitary-elements gelfand-transform elemental-subalgebra stone-weierstrass spectrum quasispectrum star-homomorphisms isometric-calculus composition-property spectral-mapping-theorem unital-algebras non-unital-algebras unitization rclike complex real nonnegative-reals continuity-theorems integration-commutation order-theory product-types commutation unique-homomorphism restrictions
