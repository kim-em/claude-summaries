---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Preserves
generated: 2025-12-07T10:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 12
subdirs_count: 2
---

# Preserves

## Overview

The `Preserves/` directory provides the comprehensive theory of limit and colimit preservation by functors, formalizing when functors send limit cones to limit cones and colimit cocones to colimit cocones. It defines core typeclasses (`PreservesLimit`, `PreservesColimit`, `PreservesLimitsOfShape`) and establishes preservation properties for specific functor constructions (opposite functors, functor categories, Grothendieck constructions, Yoneda embedding), for specific limit shapes (`Shapes/` subdirectory with products, pullbacks, equalizers, etc.), and for specific size classes (finite limits, filtered colimits, cofiltered limits). The directory also covers creation of limits by functors (`Creates/` subdirectory) and provides isomorphisms relating preservation to natural transformations, enabling reasoning about when functors commute with limit constructions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core typeclasses: `PreservesLimit`, `PreservesColimit`, `PreservesLimitsOfShape`, `PreservesLimitsOfSize` with foundational definitions |
| Limits.lean | Isomorphisms for preserved limits: `preservesLimitIso`, `preservesColimitIso`, and commutation lemmas for `lift`/`desc` with functor mapping |
| Bifunctor.lean | Preservation for bifunctors: `PreservesLimit₂`, `PreservesColimit₂` classes for functors `G : C₁ ⥤ C₂ ⥤ C` with mapped cones/cocones |
| Opposites.lean | Preservation properties of `F.op`, `F.unop`, `F.leftOp`, `F.rightOp` relating limit preservation to colimit preservation via opposite categories |
| Finite.lean | Finite limit preservation: `PreservesFiniteLimits` typeclass for functors preserving limits over finite categories (left exact functors) |
| Filtered.lean | Filtered colimit preservation: `PreservesFilteredColimitsOfSize`, `PreservesFilteredColimits` for colimits over filtered diagrams (important for algebraic categories) |
| FunctorCategory.lean | Preservation in functor categories: product functors preserve colimits pointwise, composition functors preserve limits |
| Presheaf.lean | Finite-limit-preserving presheaves: equivalence between `CostructuredArrow yoneda A` being filtered and `A` preserving finite limits (Kashiwara-Schapira 3.3.13) |
| Yoneda.lean | Yoneda preservation: natural isomorphism `yoneda.op ⋙ yoneda.obj (colimit F) ≅ yoneda.op ⋙ colimit (F ⋙ yoneda)` |
| Ulift.lean | ULift preserves all limits and colimits (including large ones), and creates small limits and colimits via fully faithfulness |
| Grothendieck.lean | Preservation for Grothendieck constructions: colimits on fibers preserve limits implies colimits on total category preserve limits |
| Over.lean | Over/Under category preservation: `Over.forget X` preserves cofiltered limits, `Under.forget X` preserves filtered colimits |

## Subdirectories

- [x] `Creates/` - Functors that create limits: classes for finite (co)limits, products, coproducts, with composition and transfer properties (complete)
- [x] `Shapes/` - Preservation of specific limit shapes: products, pullbacks, equalizers, kernels, terminal objects, biproducts, and their duals (complete)

## Search Tags

preserves-limits preserves-colimits limit-preservation colimit-preservation preserves-limits-of-shape preserves-finite-limits preserves-filtered-colimits left-exact flat-functor opposite-functors functor-categories grothendieck-construction yoneda-embedding presheaf bifunctor ulift over-categories creates-limits
