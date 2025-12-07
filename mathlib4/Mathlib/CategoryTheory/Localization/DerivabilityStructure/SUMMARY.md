---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Localization/DerivabilityStructure
generated: 2025-12-07T09:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 5
subdirs_count: 0
---

# DerivabilityStructure

## Overview

The `DerivabilityStructure/` directory formalizes the Kahn-Maltsiniotis framework of derivability structures for category localization. A localizer morphism `Φ : LocalizerMorphism W₁ W₂` is a right (resp. left) derivability structure when it has right (resp. left) resolutions and satisfies a Guitart exactness condition on the commutative square of localization functors. This machinery provides systematic conditions under which derived functors can be constructed, avoiding the need to verify pointwise conditions for each functor individually. The framework generalizes classical constructions such as injective/projective derivability structures in abelian categories with enough injectives/projectives.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of right and left derivability structures (`IsRightDerivabilityStructure`, `IsLeftDerivabilityStructure`) as typeclasses on localizer morphisms, requiring right/left resolutions and Guitart exactness of the localization square, duality between left and right structures via opposite categories |
| Constructor.lean | Constructor `IsRightDerivabilityStructure.mk'` showing a localized equivalence is a right derivability structure if resolution categories are connected and arrows have resolutions (essentially Kahn-Maltsiniotis Lemme 6.5) |
| OfFunctorialResolutions.lean | Constructor showing functorial resolutions (functor `ρ : C₂ ⥤ C₁` with natural transformation from identity) give derivability structures when the morphism property is induced and multiplicative with two-out-of-three |
| PointwiseRightDerived.lean | Connection to pointwise derived functors showing `F : C₂ ⥤ H` has pointwise right derived functor w.r.t. `W₂` iff `Φ.functor ⋙ F` has one w.r.t. `W₁` (Kahn-Maltsiniotis Proposition 5.5), comparison natural transformation between derived functors |
| Derives.lean | Abbreviation `Φ.Derives F` for when `W₁` is inverted by `Φ.functor ⋙ F`, showing this condition ensures existence of right derived functor for `F` w.r.t. `W₂`, characterization of when natural transformation is a right derived functor via isomorphism on images of `C₁` objects |

## Subdirectories

(none)

## Search Tags

derivability-structure kahn-maltsiniotis category-localization localizer-morphism guitart-exact right-derived-functor left-derived-functor resolution-category functorial-resolutions pointwise-derived-functor localized-equivalence abelian-category derived-categories homotopy-theory
