---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Filtered
generated: 2025-12-07T08:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 9
subdirs_count: 0
---

# Filtered

## Overview

The `Filtered/` directory provides a comprehensive formalization of filtered and cofiltered categories in mathlib4. Filtered categories are those where every finite diagram admits a cocone, characterized by the existence of objects "to the right" for any pair of objects and morphisms equalizing parallel arrows. This concept is fundamental for colimit theory, as filtered colimits are better behaved than arbitrary colimits (they commute with finite limits and are preserved by many functors). The directory includes the basic definition and characterizations, connections to finality and initiality, preservation through Grothendieck construction and representably flat functors, and constructions for finally small categories.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of filtered/cofiltered categories with `IsFilteredOrEmpty` and `IsFiltered` typeclasses, characterization via cocone conditions, proof that filtered categories admit cocones for finite diagrams, `sup_exists` for constructing common objects receiving morphisms from finite sets, and dual cofiltered API |
| Connected.lean | Proves that filtered categories are connected (there exists a zigzag of morphisms between any two objects) using the left/right-to-max morphisms |
| CostructuredArrow.lean | Transfers filteredness via costructured arrow categories, proving that if `R : B ⥤ T` is final, `B` is filtered, and each `CostructuredArrow L (R.obj b)` is filtered, then domain `A` of `L : A ⥤ T` is filtered (Kashiwara-Schapira Proposition 3.1.8) |
| Final.lean | Characterizes finality for functors with filtered domain/codomain: `F : C ⥤ D` is final iff `StructuredArrow d F` is filtered for all `d : D`, proves under categories and diagonal/projection functors are final when appropriate, shows fully faithful functors satisfying existence conditions preserve filteredness |
| FinallySmall.lean | Constructs final functors from small filtered categories to locally small filtered finally small categories via `FilteredFinalModel` and `fromFilteredFinalModel`, with dual cofiltered construction `CofilteredInitialModel` |
| Flat.lean | Transfers filteredness along representably coflat functors (if `F : C ⥤ D` is representably coflat and `D` is filtered, then `C` is filtered) with dual for cofilteredness and representably flat functors |
| Grothendieck.lean | Proves Grothendieck construction preserves filteredness: if `F : C ⥤ Cat` with `C` filtered and each `F.obj c` filtered, then `Grothendieck F` is filtered |
| OfColimitCommutesFiniteLimit.lean | Converse to colimit-limit commutativity: proves `K` is filtered if colimits of shape `K` commute with finite limits via `isFiltered_of_nonempty_limit_colimit_to_colimit_limit` |
| Small.lean | Constructs filtered closure of a family of objects (minimal filtered subcategory containing the family) and proves it is small (size depends only on index type and morphism types, not object types), enabling factorization through small filtered categories |

## Subdirectories

(none)

## Search Tags

filtered-categories cofiltered-categories filtered-colimits directed-colimits final-functors structured-arrow costructured-arrow grothendieck-construction representably-flat small-categories connected-categories colimit-limit-commutativity
