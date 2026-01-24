---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/QuadraticForm/QuadraticModuleCat
generated: 2026-01-25T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# QuadraticModuleCat

## Overview

This subdirectory extends the `QuadraticModuleCat` category (defined in the parent directory) with categorical structures. It equips the category of quadratic modules with a monoidal structure using tensor products of quadratic forms, and proves this monoidal structure is symmetric. The constructions require invertibility of 2 in the base ring and mirror analogous development for algebras in `AlgCat`.

## Key Files

| File | Purpose |
|------|---------|
| Monoidal.lean | Monoidal category structure on `QuadraticModuleCat R`: tensor product of quadratic modules using `QuadraticForm.tmul`, monoidal unit as squared form `sq (R := R)`, associators/unitors via tensor isometries (`tensorAssoc`, `tensorLId`, `tensorRId`), whiskering operations, proof that `forget₂` functor to `ModuleCat` is monoidal, and auxiliary definitions for tensor objects and morphisms |
| Symmetric.lean | Symmetric monoidal structure: braided category instance using tensor commutativity isometry `tensorComm`, proof that `forget₂` functor is braided, and `SymmetricCategory` instance showing the braiding is symmetric (both constructed via faithful functor method from `ModuleCat`) |

## Subdirectories

(none)

## Search Tags

quadratic-modules category-theory monoidal-categories symmetric-monoidal tensor-products braided-categories forgetful-functors monoidal-functors isometries categorical-structures
