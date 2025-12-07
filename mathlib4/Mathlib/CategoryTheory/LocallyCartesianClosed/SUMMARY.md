---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/LocallyCartesianClosed
generated: 2025-12-07T10:35:41Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# LocallyCartesianClosed

## Overview

The `LocallyCartesianClosed/` directory provides formalization of chosen pullbacks along morphisms, which is foundational infrastructure for locally cartesian closed categories. It defines the `ChosenPullbacksAlong` typeclass that provides functorial pullback data as a right adjoint to `Over.map f`, proves closure properties (isomorphisms and compositions have chosen pullbacks), and establishes that chosen pullbacks yield actual pullbacks. For cartesian monoidal categories, it proves that morphisms to the terminal unit and product projections have chosen pullbacks.

## Key Files

| File | Purpose |
|------|---------|
| ChosenPullbacksAlong.lean | Typeclass for functorial choice of pullbacks along a morphism `f : Y ⟶ X` given by functor `Over X ⥤ Over Y` right adjoint to `Over.map f`, with closure properties and compatibility with cartesian monoidal structure |

## Subdirectories

*(none)*

## Search Tags

category-theory locally-cartesian-closed pullbacks chosen-pullbacks over-categories adjunctions slice-categories cartesian-monoidal
