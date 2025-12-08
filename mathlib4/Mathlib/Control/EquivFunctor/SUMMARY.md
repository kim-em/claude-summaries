---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Control/EquivFunctor
generated: 2025-12-08T15:45:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 1
subdirs_count: 0
---

# EquivFunctor

## Overview

The `EquivFunctor/` subdirectory provides concrete instances of the `EquivFunctor` typeclass, which represents endofunctors of the "core" of the category `Type` that map equivalences to equivalences coherently. This folder contains implementations for standard type constructors including `Unique`, `Perm`, `Finset`, and `Fintype`, enabling the `equiv_rw` tactic to rewrite under these functions.

## Key Files

| File | Purpose |
|------|---------|
| Instances.lean | Defines `EquivFunctor` instances for `Unique`, `Perm`, `Finset`, and `Fintype`; each instance provides the `map` function and proves the required functor laws (identity and composition preservation) |

## Subdirectories

*(None)*

## Search Tags

equiv-functor equivalence-functor type-equivalences functor-instances unique perm finset fintype equivalence-rewriting categorical-functors endofunctors lawful-functors
