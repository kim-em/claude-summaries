---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/ChosenFiniteProducts
generated: 2025-12-07T09:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# ChosenFiniteProducts

## Overview

This folder contains deprecated module redirects for the chosen finite products infrastructure, which was reorganized into `Mathlib.CategoryTheory.Monoidal.Cartesian.*` on 2025-05-15. All files in this directory are compatibility shims that re-export the new module locations. The original functionality provided instances and constructions for categories with chosen finite products (terminal objects and binary products), including instances for Cat (category of categories), functor categories, inf-semilattices, and over categories.

## Key Files

| File | Purpose |
|------|---------|
| Cat.lean | Deprecated redirect to `Mathlib.CategoryTheory.Monoidal.Cartesian.Cat` for chosen finite products in Cat |
| FunctorCategory.lean | Deprecated redirect to `Mathlib.CategoryTheory.Monoidal.Cartesian.FunctorCategory` for chosen finite products in functor categories |
| InfSemilattice.lean | Deprecated redirect to `Mathlib.CategoryTheory.Monoidal.Cartesian.InfSemilattice` for chosen finite products in inf-semilattices |
| Over.lean | Deprecated redirect to `Mathlib.CategoryTheory.Monoidal.Cartesian.Over` for chosen finite products in over categories |

## Subdirectories

None.

## Search Tags

category-theory chosen-finite-products deprecated module-redirects cartesian-monoidal terminal-object binary-products functor-category over-category inf-semilattice compatibility-shims
