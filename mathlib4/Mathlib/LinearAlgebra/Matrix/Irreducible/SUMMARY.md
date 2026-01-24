---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Matrix/Irreducible
generated: 2026-01-25T22:47:30Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Irreducible

## Overview

The `Irreducible/` directory provides a graph-theoretic framework for studying irreducibility and primitivity of nonnegative matrices, establishing the foundation for Perron-Frobenius theory. It associates a directed graph (quiver) with each matrix where edges correspond to positive entries, enabling translation between algebraic properties (matrix powers) and graph-theoretic properties (path existence). The directory proves the equivalence between the graph-theoretic definition of irreducibility (strong connectivity) and the algebraic definition (existence of positive entries in powers), and establishes that primitive matrices (with an all-positive power) are irreducible.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions and theorems for irreducible and primitive matrices: `Matrix.toQuiver` (quiver of positive entries), `Matrix.IsIrreducible` (nonnegative with strongly connected quiver), `Matrix.IsPrimitive` (nonnegative with all-positive power), equivalence `pow_apply_pos_iff_nonempty_path` linking matrix powers to graph paths, and invariance of irreducibility under transposition |

## Subdirectories

*(No subdirectories)*

## Search Tags

matrix irreducible primitive nonnegative graph quiver path strong-connectivity matrix-powers perron-frobenius transpose linear-ordered-ring
