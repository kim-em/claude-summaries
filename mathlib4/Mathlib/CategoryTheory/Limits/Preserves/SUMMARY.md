---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Preserves
generated: 2025-12-07T12:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 12
subdirs_count: 2
---

# Preserves

## Overview

The `Preserves/` directory provides the comprehensive theory of limit and colimit preservation by functors, formalizing when functors send limit cones to limit cones and colimit cocones to colimit cocones. At its core, the directory defines the fundamental typeclasses (`PreservesLimit`, `PreservesColimit`, `PreservesLimitsOfShape`, `PreservesLimitsOfSize`) and establishes key isomorphisms (`preservesLimitIso`, `preservesColimitIso`) that enable practical verification of preservation via comparison maps. Beyond the general theory, it covers three major aspects: (1) preservation properties of specific functor constructions including opposite functors, functor categories, bifunctors, Grothendieck constructions, and the Yoneda embedding; (2) preservation of limit classes characterized by size or filtering properties (finite limits via `Finite.lean`, filtered colimits via `Filtered.lean`, cofiltered limits via `Over.lean`); and (3) specialized theories for concrete shapes and limit creation. The `Shapes/` subdirectory establishes that preservation of specific diagram shapes (products, pullbacks, equalizers, kernels, biproducts, etc.) is equivalent to comparison maps being isomorphisms, providing practical tools for verifying preservation in concrete cases. The `Creates/` subdirectory extends preservation to limit creation, showing how functors can lift limit structures from the target category back to the source category, with particular emphasis on finite limits and composition properties. Together, these components provide the essential infrastructure for characterizing functors by their interaction with limit constructions—a central organizing principle in category theory that distinguishes left/right exact functors, flat functors, and other important functor classes.

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

- [x] `Creates/` - Limit creation by functors: typeclasses for creating finite (co)limits and specific shapes, with composition/transfer properties and automatic preservation
- [x] `Shapes/` - Shape-specific preservation: equivalences between preserving concrete limit shapes and comparison maps being isomorphisms for products, pullbacks, equalizers, kernels, biproducts, images, and more

## Search Tags

preserves-limits preserves-colimits limit-preservation colimit-preservation preserves-limits-of-shape preserves-finite-limits preserves-filtered-colimits left-exact flat-functor opposite-functors functor-categories grothendieck-construction yoneda-embedding presheaf bifunctor ulift over-categories creates-limits
