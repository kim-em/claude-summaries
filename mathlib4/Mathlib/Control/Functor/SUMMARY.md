---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Control/Functor
generated: 2025-12-08T16:15:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 1
subdirs_count: 0
---

# Functor

## Overview

The `Functor/` directory contains theory for multivariate functors, which generalize ordinary functors from types to type vectors. It defines the `MvFunctor` typeclass for functors between the category of type vectors (`TypeVec n → Type`) and the category of types, along with lawful instances, predicate/relation lifting, support sets, and equivalence-based functor construction.

## Key Files

| File | Purpose |
|------|---------|
| Multivariate.lean | Defines MvFunctor typeclass with map operation (`<$$>` notation); LawfulMvFunctor class with identity and composition laws; predicate lifting (LiftP/LiftP') and relational lifting (LiftR/LiftR') for type vectors; support sets (supp) for extracting values from projections; specialized lifting theorems for PredLast/RelLast on extended type vectors; ofEquiv for constructing functors from equivalences |

## Subdirectories

None.

## Search Tags

multivariate-functors type-vectors functor-laws predicate-lifting relation-lifting support-sets lawful-functors functor-composition category-theory MvFunctor TypeVec
