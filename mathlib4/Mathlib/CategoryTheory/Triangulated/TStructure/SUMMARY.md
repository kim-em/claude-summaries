---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Triangulated/TStructure
generated: 2025-12-08T15:45:30Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 2
subdirs_count: 0
---

# TStructure

## Overview

The `TStructure/` directory contains the formalization of t-structures on triangulated categories, a fundamental concept for working with filtrations and truncations in homological algebra. A t-structure consists of two families of full subcategories indexed by integers (the "less than or equal to n" and "greater than or equal to n" parts) satisfying compatibility axioms with the shift functor and a factorization property. The main file defines the `TStructure` type with type classes `IsLE X n` and `IsGE X n` to express membership in these subcategories, proves monotonicity and shift compatibility, and establishes that morphisms between incompatible objects are zero. The truncation file implements the key truncation functors `truncLT n` and `truncGE n` that project objects to their "less than n" and "greater than or equal to n" parts, along with the natural transformations fitting into distinguished triangles.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `TStructure C` as pairs of object predicates `le n` and `ge n` with closure under isomorphisms and shift; defines type classes `IsLE X n` and `IsGE X n`; proves monotonicity (`le_monotone`, `ge_antitone`), shift compatibility, and orthogonality (`zero`: morphisms X → Y are zero when X ≤ n₀ < n₁ ≤ Y) |
| TruncLTGE.lean | Constructs truncation functors `truncLT n : C ⥤ C` and `truncGE n : C ⥤ C` with natural transformations `truncLTι n : truncLT n ⟶ 𝟭 C`, `truncGEπ n : 𝟭 C ⟶ truncGE n`, and `truncGEδLT n : truncGE n ⟶ truncLT n ⋙ shiftFunctor C 1` forming distinguished triangles; proves uniqueness via `triangle_map_ext` using orthogonality |

## Subdirectories

(No subdirectories)

## Search Tags

t-structures triangulated-categories truncation-functors homological-algebra filtrations hearts derived-categories object-predicates shift-compatibility orthogonality distinguished-triangles perverse-sheaves BBD
