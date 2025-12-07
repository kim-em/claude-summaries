---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Localization
generated: 2025-12-07T08:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 27
subdirs_count: 3
---

# Localization

## Overview

The `Localization/` directory formalizes the localization of categories with respect to morphism properties, a fundamental construction in category theory that formally inverts a specified class of morphisms. It provides the universal construction `W.Localization` obtained by taking quotients of path categories (following Gabriel-Zisman), the predicate `L.IsLocalization W` characterizing when a functor identifies its target with the localized category, calculus of fractions for computing morphisms in localized categories, and specialized localization functors such as Bousfield localization. This machinery is essential for homotopy theory, derived categories, and any context where one needs to "invert" certain morphisms to create new categories.

## Key Files

| File | Purpose |
|------|---------|
| Construction.lean | Core construction of localized category `W.Localization` via quotient of path category over quiver with formal inverses |
| Predicate.lean | Predicate `L.IsLocalization W` expressing when functor identifies target with localized category, includes universal property and lifting theorems |
| HasLocalization.lean | Typeclass `HasLocalization.{w} W` allowing users to specify localized category with custom universe parameters |
| CalculusOfFractions.lean | Left and right calculus of fractions (Gabriel-Zisman), showing morphisms in localized categories can be represented as fractions |
| Equivalence.lean | Preservation of localization through equivalences of categories, showing localization predicate stable under source/target equivalences |
| Bousfield.lean | Bousfield localization defining `P.isLocal` morphisms that induce bijections on hom-sets to local objects |
| BousfieldTransfiniteComposition.lean | Transfinite composition techniques for Bousfield localization |
| Adjunction.lean | Localization of adjunctions showing adjoint functors induce adjunctions on localized categories |
| Composition.lean | Composition of localization functors and morphism properties |
| LocalizerMorphism.lean | Morphisms between localizers (functors preserving the classes of morphisms to be inverted) |
| Resolution.lean | Right and left resolutions for morphism of localizers, fundamental for derivability structures |
| HomEquiv.lean | Equivalences between hom-sets induced by localization |
| Opposite.lean | Localization in opposite categories |
| Quotient.lean | Quotient functors and their localization properties |
| FiniteProducts.lean | Preservation of finite products under localization |
| Linear.lean | Localization of linear categories |
| Preadditive.lean | Localization of preadditive categories |
| LocallySmall.lean | Conditions for localized categories to be locally small |
| SmallHom.lean | Small hom-sets in localized categories |
| SmallShiftedHom.lean | Small shifted hom-sets for triangulated localization |
| Pi.lean | Localization of product categories |
| Prod.lean | Localization of binary products |
| Bifunctor.lean | Localization of bifunctors |
| Trifunctor.lean | Localization of trifunctors |
| StructuredArrow.lean | Localization of structured arrow categories |
| Triangulated.lean | Localization of triangulated categories |
| Monoidal.lean | Entry point for monoidal localization (subdirectory) |

## Subdirectories

- [x] `CalculusOfFractions/` - Additional calculus of fractions constructions (complete)
- [x] `DerivabilityStructure/` - Derivability structures for localization (Kahn-Maltsiniotis framework) (complete)
- [ ] `Monoidal/` - Localization of monoidal categories (pending)

## Search Tags

localization category-theory morphism-property universal-property calculus-of-fractions gabriel-zisman bousfield-localization derived-categories homotopy-theory quotient-category formal-inverses resolution derivability-structure localizer-morphism triangulated-categories
