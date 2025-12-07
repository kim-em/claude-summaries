---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Types
generated: 2025-12-07T20:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Types

## Overview

The `Types/` directory establishes the category of types (`Type u`) as a Cartesian monoidal category, demonstrating that the tensor product is the ordinary product type `×` and the monoidal unit is `PUnit`. It provides computational simp lemmas for all monoidal structure components (tensor, associator, unitors, braiding) and proves that the coyoneda functor from the monoidal unit (`𝟙_ C ⟶ -`) has a lax monoidal structure. This connects categorical monoidal structure to the familiar type-level operations and enables reasoning about monoidal functors to/from `Type`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Monoidal category instance for `Type u` via CartesianMonoidalCategory, braiding from Cartesian structure, and simp lemmas for tensor products, unitors, associators, and braiding on types |
| Coyoneda.lean | Lax monoidal functor instance for coyoneda from the monoidal unit with tensor and unit morphisms |

## Subdirectories

*(No subdirectories)*

## Search Tags

type-category monoidal-types cartesian-monoidal product-types monoidal-unit braiding-types coyoneda lax-monoidal-functor tensor-simp unitor-simp associator-simp
