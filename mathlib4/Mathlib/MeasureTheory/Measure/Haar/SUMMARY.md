---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Measure/Haar
generated: 2026-01-25T20:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 9
subdirs_count: 0
---

# Haar

## Overview

The `Haar/` directory contains the formalization of Haar measure theory for locally compact topological groups and vector spaces. It establishes the existence and uniqueness (up to scaling) of left-invariant measures on groups, develops special cases for normed spaces and inner product spaces, and provides tools for measure disintegration and quotient measures. Key results include the construction of Haar measure on compact sets via covering numbers, uniqueness theorems under various regularity conditions, Lebesgue measure as the canonical Haar measure on vector spaces, and the distributive and multiplicative characters that measure how group actions scale Haar measures.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core construction of Haar measure for locally compact Hausdorff groups via covering numbers (index function), content `chaar`, and Tychonoff's theorem; proves existence of left-invariant regular measure `haarMeasure` normalized to give measure 1 to a chosen compact set, includes basic uniqueness theorem for σ-finite measures on second-countable groups |
| Unique.lean | Comprehensive uniqueness results for Haar measures beyond second-countable case: proves two left-invariant measures coincide up to scalar factor under various regularity conditions (inner regular, regular, completion-regular); includes integral equality `integral_isMulLeftInvariant_eq_smul_of_hasCompactSupport`, measure equality on compact sets and open sets, uniqueness for probability Haar measures, following McQuillan's approach for completion-regularity |
| OfBasis.lean | Construction of additive Haar measure (Lebesgue measure) from a basis of a finite-dimensional real vector space; defines parallelepiped spanned by basis vectors, `Basis.addHaar` giving measure 1 to the basis parallelepiped, establishes `MeasureSpace` instance for finite-dimensional inner product spaces using orthonormal bases |
| Quotient.lean | Haar measure theory on quotient spaces `G ⧸ Γ` for subgroup `Γ` acting on group `G`; proves quotient measures satisfying `QuotientMeasureEqMeasurePreimage` are invariant under `G`-action, develops left-invariant measures on quotients of unimodular groups (both left and right invariant), includes fundamental domain relationships and converse results relating quotient measure properties to covolume finiteness |
| InnerProductSpace.lean | Canonical volume forms and measures on finite-dimensional inner product spaces: proves orientation-induced volume form gives measure 1 to parallelepipeds spanned by orthonormal bases (`Orientation.measure_orthonormalBasis`), establishes `Orientation.measure_eq_volume` showing canonical volume form coincides with the `MeasureSpace` volume, includes `LinearIsometryEquiv.toMeasurableEquiv` for isometry-induced measurable equivalences |
| NormedSpace.lean | Basic Haar measure properties for real normed vector spaces; proves additive Haar measures on nontrivial finite-dimensional spaces have no atoms, establishes `MapLinearEquiv.isAddHaarMeasure` for linear equivalences preserving Haar property, includes continuity result `AddMonoidHom.continuous_of_measurable` showing Borel-measurable group homomorphisms from locally compact normed groups are continuous |
| Disintegration.lean | Disintegration of Haar measure along linear maps: main theorem `LinearMap.exists_map_addHaar_eq_smul_addHaar` proving pushforward of Haar measure under surjective linear map is proportional to target Haar measure (with proportionality factor related to kernel measure), establishes `ae_mem_of_ae_add_linearMap_mem` showing almost-everywhere properties can be verified along translates of vector subspaces |
| DistribChar.lean | Distributive Haar character `distribHaarChar : G →* ℝ≥0` for groups `G` acting by additive morphisms on locally compact commutative groups `A`; defines the unique positive real by which group elements scale Haar measures under the action (`μ (g • s) = distribHaarChar(g) * μ s`), proves character is independent of chosen Haar measure and forms a group homomorphism, includes scalar factor relationships `addHaarScalarFactor_smul_eq_distribHaarChar` |
| MulEquivHaarChar.lean | Multiplicative Haar character `mulEquivHaarChar : (G ≃ₜ* G) → ℝ≥0` measuring how continuous group automorphisms scale Haar measures; defines the positive real factor satisfying `mulEquivHaarChar φ • map φ μ = μ` for regular Haar measure `μ`, establishes independence from choice of Haar measure via `mulEquivHaarChar_eq`, includes additive version `addEquivAddHaarChar` for topological group isomorphisms |

## Subdirectories

## Search Tags

haar-measure left-invariant-measure locally-compact-group topological-group existence-uniqueness regular-measure inner-regular covering-number chaar index parallelepiped basis-measure lebesgue-measure orthonormal-basis volume-form inner-product-space quotient-measure fundamental-domain unimodular-group disintegration linear-map pushforward scalar-factor distributive-character multiplicative-character group-action measure-scaling normed-space finite-dimensional no-atoms borel-measurable
