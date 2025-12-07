---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Internal
generated: 2025-12-07T11:10:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 1
---

# Internal

## Overview

The `Internal/` directory establishes the deep connection between internal algebraic objects defined categorically in monoidal categories and their corresponding bundled algebraic structures. At the core are equivalences showing that internal objects (monoids, comonoids, commutative monoids, groups) in functor categories `C ⥤ D` correspond precisely to functors into the categories of such objects in `D`. This principle specializes beautifully: monoid objects in `ModuleCat R` are equivalent to R-algebras, and internal algebraic objects in `Type` recover the classical bundled structures (`MonCat`, `GrpCat`, `CommMonCat`, `CommGrpCat`). The directory also demonstrates that limits of internal monoid objects can be constructed when the ambient category has limits, with preservation properties via lax monoidal functors.

## Key Files

| File | Purpose |
|------|---------|
| FunctorCategory.lean | Equivalences `Mon (C ⥤ D) ≌ C ⥤ Mon D`, `Comon (C ⥤ D) ≌ C ⥤ Comon D`, and `CommMon (C ⥤ D) ≌ C ⥤ CommMon D` showing internal objects in functor categories correspond to functors into categories of internal objects |
| Limits.lean | Construction of limits for `Mon C` when `C` has limits, showing the forgetful functor preserves limits by interpreting monoid objects as functors and using the lax monoidal limit functor |
| Module.lean | Equivalence `Mon (ModuleCat R) ≌ AlgCat R` demonstrating that monoid objects in the category of R-modules are naturally equivalent to R-algebras, with compatibility of forgetful functors |

## Subdirectories

- [x] `Types/` - Fundamental equivalences between internal algebraic objects in `Type u` (monoids, groups, and commutative variants) and their bundled categorical counterparts (`MonCat`, `GrpCat`, `CommMonCat`, `CommGrpCat`), demonstrating that categorical and classical algebraic perspectives coincide

## Search Tags

internal-objects monoidal-categories functor-categories monoid-objects comonoid-objects commutative-monoid-objects category-equivalences module-algebras limits-preservation lax-monoidal-functors categorical-algebra
