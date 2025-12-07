---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Internal/Types
generated: 2025-12-07T11:04:54Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# Types

## Overview

The `Types/` directory establishes fundamental equivalences between internal algebraic objects defined in the category `Type u` and their corresponding native bundled categorical structures. It proves that monoid objects, group objects, and commutative variants in `Type` are naturally equivalent to the standard bundled categories `MonCat`, `GrpCat`, `CommMonCat`, and `CommGrpCat`. These equivalences are compatible with forgetful functors, demonstrating that the internal categorical perspective coincides with classical algebraic structures.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Establishes `Mon (Type u) ≌ MonCat.{u}` and `CommMon (Type u) ≌ CommMonCat.{u}`, showing internal (commutative) monoid objects in Type are equivalent to bundled (commutative) monoids, with forgetful functor compatibility |
| Grp_.lean | Proves `Grp (Type u) ≌ GrpCat.{u}`, demonstrating internal group objects in Type correspond to bundled groups, building on the monoid equivalence by adding inversion structure |
| CommGrp_.lean | Establishes `CommGrp (Type u) ≌ CommGrpCat.{u}`, showing internal commutative group objects in Type are equivalent to bundled commutative groups, with compatibility to both group and commutative monoid forgetful functors |

## Subdirectories

None.

## Search Tags

internal-objects type-category category-equivalences monoid-objects group-objects commutative-groups bundled-structures forgetful-functors monoidal-categories concrete-categories categorical-algebra
