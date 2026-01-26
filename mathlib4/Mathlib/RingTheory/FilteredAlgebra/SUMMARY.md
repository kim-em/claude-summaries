---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/FilteredAlgebra
generated: 2026-01-26T19:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# FilteredAlgebra

## Overview

The `FilteredAlgebra/` directory contains the foundational theory of filtrations on algebraic structures. It defines increasingly general notions: filtrations on abelian groups (monotone series with controlled suprema), ring filtrations (compatible with multiplication), and module filtrations (compatible with scalar multiplication). The definitions use a `F_lt` parameter to encode "strict predecessors" without requiring complete lattice structures on the ambient type, providing better definitional control especially for integer-indexed filtrations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `IsFiltration`, `IsRingFiltration`, and `IsModuleFiltration` type classes; provides convenience constructors for integer-indexed filtrations |

## Subdirectories

(none)

## Search Tags

filtered-algebra filtration ring-filtration module-filtration graded-monoid graded-smul monotone-series integer-indexed SetLike abelian-group semiring
