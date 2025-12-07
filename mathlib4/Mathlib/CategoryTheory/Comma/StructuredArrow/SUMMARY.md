---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Comma/StructuredArrow
generated: 2025-12-07T08:48:42Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 5
subdirs_count: 0
---

# StructuredArrow

## Overview

The `StructuredArrow/` directory provides the theory of structured arrow categories and their dual, costructured arrow categories. A structured arrow `StructuredArrow S T` for `S : D` and functor `T : C ⥤ D` has objects that are morphisms `S ⟶ T.obj Y` for some `Y : C`, with morphisms given by commutative triangles. The dual notion `CostructuredArrow S T` for `S : C ⥤ D` and `T : D` consists of morphisms `S.obj Y ⟶ T`. The directory establishes these categories as specializations of comma categories, proves functoriality, establishes equivalences with Grothendieck constructions, proves finality results for costructured arrow categories, and provides smallness/local smallness instances.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `StructuredArrow S T` as `Comma (fromPUnit S) T` and `CostructuredArrow S T` as `Comma T (fromPUnit T)`, with constructors (`mk`, `homMk`, `isoMk`), projection functors, extensionality lemmas, mapping functors, and universal arrow characterizations |
| CommaMap.lean | Equivalence between structured arrow categories on `Comma.map α β` and comma categories on instances of `StructuredArrow.map₂`, establishing `commaMapEquivalence` when `β` is a natural isomorphism |
| Final.lean | Finality theorem for costructured arrow categories: a functor `L : A ⥤ T` is final if there exists a final functor `R : B ⥤ T` such that for all `b : B`, the canonical functor `CostructuredArrow L (R.obj b) ⥤ Over (R.obj b)` is final |
| Functor.lean | Functoriality of structured/costructured arrow construction: `StructuredArrow.functor : Dᵒᵖ ⥤ Cat` and `CostructuredArrow.functor : D ⥤ Cat`, plus equivalence between Grothendieck construction `Grothendieck (R ⋙ functor L)` and comma category `Comma L R` |
| Small.lean | Smallness instances for structured and costructured arrow categories when the underlying category is small and locally small, used in the proof of the Special Adjoint Functor Theorem |

## Subdirectories

(none)

## Search Tags

structured-arrow costructured-arrow comma-category universal-arrow grothendieck-construction final-functor cat-valued-functor small-category locally-small adjoint-functor-theorem categorical-construction
