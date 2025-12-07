---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/ObjectProperty/FunctorCategory
generated: 2025-12-07T10:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# FunctorCategory

## Overview

The `FunctorCategory/` directory specializes the ObjectProperty framework to functors viewed as objects in functor categories. It defines limit-preservation properties (`preservesLimitsOfShape K`, `preservesFiniteLimits`) as object properties in the functor category `J ⥤ C`, and proves that these properties are stable under colimits when the colimits commute with the corresponding limits (exactness conditions). This connects typeclass-based limit preservation with the object property machinery, enabling formal reasoning about collections of functors that preserve certain limits.

## Key Files

| File | Purpose |
|------|---------|
| PreservesLimits.lean | Defines `preservesLimitsOfShape K` and `preservesFiniteLimits` as object properties in functor categories, proves closure under colimits when they commute with limits (using exact colimits for finite limits) |

## Subdirectories

(None)

## Search Tags

functor-category object-property limit-preservation preserves-limits preserves-finite-limits colimit-closure exact-colimits evaluation-functor natural-isomorphism grothendieck-axioms
