---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/FinCategory
generated: 2025-12-07T13:25:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# FinCategory

## Overview

The `FinCategory/` directory provides the formalization of finite categories in mathlib4. A finite category is one with finitely many objects and finitely many morphisms between each pair of objects. The directory defines the `FinCategory` typeclass and proves that finite categories can be equivalently represented as categories with objects in `Type 0`, providing a bridge between abstract finite categories and concrete finitary representations using `Fin` types.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `FinCategory` typeclass requiring `Fintype` instances for objects and morphism spaces, with instances for discrete categories, opposite categories, and ULift constructions |
| AsType.lean | Equivalences showing any finite category is equivalent to a category with `Fin n` objects and `Fin m` morphisms, enabling concrete finitary representations |

## Subdirectories

(No subdirectories)

## Search Tags

finite-categories fintype discrete-categories fin-types category-equivalence finitary-representations finite-objects finite-morphisms
