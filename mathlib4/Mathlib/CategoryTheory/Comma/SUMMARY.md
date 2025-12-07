---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Comma
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 5
subdirs_count: 3
---

# Comma

## Overview

The `Comma/` directory provides a comprehensive treatment of comma categories and their specializations, serving as a central hub for several fundamental categorical constructions. A comma category `Comma L R` for functors `L : A ⥤ T` and `R : B ⥤ T` has objects consisting of morphisms `L.obj left ⟶ R.obj right` with morphisms given by commutative squares. The core files establish basic definitions, prove finality results, and establish cardinality and local smallness properties.

Three specialized subdirectories develop key instances: `StructuredArrow/` provides the theory of structured and costructured arrow categories (morphisms from/to a functor's image) with connections to Grothendieck constructions and finality theorems; `Over/` implements over and under categories (slice and coslice categories) with a complete framework including typeclass interfaces, adjunctions via pullback/pushout functors, and star/costar functors; and `Presheaf/` establishes the deep connection between comma categories and presheaf categories via the equivalence `Over A ≌ (CostructuredArrow yoneda A)ᵒᵖ ⥤ Type v`, enabling relative versions of the Yoneda lemma. Together, these files provide the essential machinery for working with "morphisms over/under" objects and functorial constructions throughout category theory.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of comma categories `Comma L R` with objects as triples `(left, right, hom)` where `hom : L.obj left ⟶ R.obj right`, plus morphisms as commutative squares |
| Arrow.lean | Arrow category `Arrow T` as specialization of `Comma (𝟭 T) (𝟭 T)` with morphisms in `T` as objects and commutative squares as morphisms |
| CardinalArrow.lean | Cardinality results for arrow categories: finiteness equivalence with `FinCategory`, equivalence with opposite arrow category, and smallness properties |
| Final.lean | Finality results for comma category projections: `fst L R` is final if `R` is final, `snd L R` is initial if `L` is initial, plus filteredness and connectivity results |
| LocallySmall.lean | Local smallness instances for comma categories and specializations (structured arrows, over/under categories) when underlying categories are locally small |

## Subdirectories

- [x] `StructuredArrow/` - Structured and costructured arrow categories with Grothendieck construction equivalences, finality results, and smallness instances (complete)
- [x] `Over/` - Over and under categories with typeclass interfaces, pullback/pushout adjunctions, and star/costar functors connecting to binary products/coproducts (complete)
- [x] `Presheaf/` - Equivalence `Over A ≌ (CostructuredArrow yoneda A)ᵒᵖ ⥤ Type v` relating over categories to presheaves, with relative Yoneda colimit preservation (complete)

## Search Tags

comma-category slice-category coslice-category arrow-category over-category under-category structured-arrow costructured-arrow final-functor locally-small commutative-square pullback-functor pushout-functor adjunction typeclass-interface star-functor costar-functor grothendieck-construction presheaf yoneda-lemma categorical-equivalence colimit-preservation universal-arrow small-category
