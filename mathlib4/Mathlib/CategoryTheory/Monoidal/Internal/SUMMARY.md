---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Internal
generated: 2025-12-07T10:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 3
subdirs_count: 1
---

# Internal

## Overview

The `Internal/` directory contains equivalences between internal algebraic objects in monoidal categories and their corresponding bundled categorical constructions. It demonstrates that monoid objects, comonoid objects, and commutative monoid objects in functor categories `C ⥤ D` are equivalent to functors into the categories of such objects in `D`. Additionally, it shows that monoid objects in `ModuleCat R` correspond to R-algebras, and establishes limits for categories of monoid objects.

## Key Files

| File | Purpose |
|------|---------|
| FunctorCategory.lean | Equivalences `Mon (C ⥤ D) ≌ C ⥤ Mon D`, `Comon (C ⥤ D) ≌ C ⥤ Comon D`, and `CommMon (C ⥤ D) ≌ C ⥤ CommMon D` showing internal objects in functor categories correspond to functors into categories of internal objects |
| Limits.lean | Construction of limits for `Mon C` when `C` has limits, showing the forgetful functor preserves limits by interpreting monoid objects as functors and using the lax monoidal limit functor |
| Module.lean | Equivalence `Mon (ModuleCat R) ≌ AlgCat R` demonstrating that monoid objects in the category of R-modules are naturally equivalent to R-algebras, with compatibility of forgetful functors |

## Subdirectories

- [ ] `Types/` - Equivalences between internal algebraic objects in Type and bundled concrete categories (pending)

## Search Tags

internal-objects monoidal-categories functor-categories monoid-objects comonoid-objects commutative-monoid-objects category-equivalences module-algebras limits-preservation lax-monoidal-functors categorical-algebra
