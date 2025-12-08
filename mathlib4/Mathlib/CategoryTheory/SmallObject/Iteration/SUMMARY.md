---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/SmallObject/Iteration
generated: 2025-12-08T15:45:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 4
subdirs_count: 0
---

# Iteration

## Overview

This subdirectory contains the detailed implementation machinery for transfinite iteration of successor structures (`SuccStruct`), which is a key component of the small object argument. The core concept is to iterate a successor structure `Φ` along a well-ordered type `J`, building functors `Set.Iic j ⥤ C` that encode the iteration values for all indices up to `j`. The implementation uses transfinite induction with careful handling of three cases: bottom elements, successor elements, and limit elements.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions for `SuccStruct` and `Φ.Iteration j`, including the structure of iteration data, restriction operations, and proof that `Φ.Iteration j` is a subsingleton (uniqueness via extensive well-founded induction) |
| ExtendToSucc.lean | Provides `extendToSucc` to extend a functor `F : Set.Iic j ⥤ C` to `Set.Iic (Order.succ j) ⥤ C` by specifying the image of the new successor element and the transition morphism |
| FunctorOfCocone.lean | Defines `ofCocone` which extends a functor `F : Set.Iio j ⥤ C` and a cocone to a functor `Set.Iic j ⥤ C` by mapping the top element `j` to the cocone point (used for limit stages) |
| Nonempty.lean | Proves existence of `Φ.Iteration j` for all `j : J` by transfinite induction, constructing iterations via `mkOfBot`, `mkOfSucc`, and `mkOfLimit` for the three inductive cases |

## Subdirectories

_(none)_

## Search Tags

transfinite-iteration successor-structures well-ordered-types small-object-argument iteration-machinery functorial-factorization-systems category-theory ordinals well-founded-induction subsingletons limit-colimit-constructions cocones functor-extensions
