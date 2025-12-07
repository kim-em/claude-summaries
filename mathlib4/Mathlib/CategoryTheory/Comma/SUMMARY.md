---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Comma
generated: 2025-12-07T08:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 5
subdirs_count: 3
---

# Comma

## Overview

The `Comma/` directory implements comma categories and their specializations. A comma category `Comma L R` for functors `L : A ⥤ T` and `R : B ⥤ T` has objects consisting of morphisms `L.obj left ⟶ R.obj right` and morphisms given by commutative squares. This construction generalizes several important categorical concepts: the arrow category (where both functors are identity), over/under categories (slice and coslice categories), and structured arrow categories. The directory also includes properties of comma categories such as finality of projections, local smallness conditions, and cardinality results.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of comma categories `Comma L R` with objects as triples `(left, right, hom)` where `hom : L.obj left ⟶ R.obj right`, plus morphisms as commutative squares |
| Arrow.lean | Arrow category `Arrow T` as specialization of `Comma (𝟭 T) (𝟭 T)` with morphisms in `T` as objects and commutative squares as morphisms |
| CardinalArrow.lean | Cardinality results for arrow categories: finiteness equivalence with `FinCategory`, equivalence with opposite arrow category, and smallness properties |
| Final.lean | Finality results for comma category projections: `fst L R` is final if `R` is final, `snd L R` is initial if `L` is initial, plus filteredness and connectivity results |
| LocallySmall.lean | Local smallness instances for comma categories and specializations (structured arrows, over/under categories) when underlying categories are locally small |

## Subdirectories

- [~] `Over/` - Over and under categories (slice and coslice categories) (preliminary)
- [ ] `Presheaf/` - Comma categories related to presheaves (pending)
- [ ] `StructuredArrow/` - Structured arrow categories and costructured arrow categories (pending)

## Search Tags

comma-category slice-category coslice-category arrow-category over-category under-category structured-arrow final-functor locally-small commutative-square
