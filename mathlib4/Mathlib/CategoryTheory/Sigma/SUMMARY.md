---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Sigma
generated: 2025-12-08T15:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 1
subdirs_count: 0
---

# Sigma

## Overview

The `Sigma/` directory defines the category structure on sigma-types (disjoint unions) of categories. Given an indexed family of categories `C i` for `i : I`, this constructs the coproduct category `Σ i, C i` where objects are pairs `⟨i, X⟩` with `X : C i`, and morphisms exist only between objects in the same component. This construction witnesses that sigma-types provide the categorical coproduct in the category of categories (Cat), with inclusion functors from each component and a universal property for functors out of the coproduct.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Category structure on sigma-types with morphisms `SigmaHom`, inclusion functors `incl i : C i ⥤ Σ i, C i`, universal functor `desc` satisfying `incl i ⋙ desc F ≅ F i`, functoriality of `map` for index functions, and assembly of indexed families of functors/natural transformations |

## Subdirectories

(none)

## Search Tags

sigma-types disjoint-union coproduct-category inclusion-functor universal-property categorical-coproduct indexed-families natural-transformations functor-assembly category-of-categories
