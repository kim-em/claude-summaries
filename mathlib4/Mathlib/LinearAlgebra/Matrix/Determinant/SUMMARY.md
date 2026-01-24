---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Matrix/Determinant
generated: 2026-01-25T23:47:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Determinant

## Overview

The `Determinant/` subdirectory provides a comprehensive formalization of determinant theory for matrices. `Basic.lean` defines the determinant via the Leibniz formula (sum over permutations) and establishes its fundamental properties: multiplicativity (`det(AB) = det(A)det(B)`), behavior under transpose, permutation, and reindexing, interaction with row/column operations, and conditions for zero determinants (repeated rows, linear dependence). `Misc.lean` contains specialized determinant formulas for matrices with constrained row/column sums. `TotallyUnimodular.lean` formalizes totally unimodular matrices (all square submatrix determinants in {-1, 0, 1}) with closure properties and characterization theorems.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core determinant theory: `Matrix.det` defined via Leibniz formula, `detRowAlternating` as alternating multilinear map, fundamental properties (det_mul, det_transpose, det_diagonal, det_one), row/column operation effects, determinant computation for block diagonal and block triangular matrices, relationship to linear independence |
| Misc.lean | Specialized determinant formulas: submatrix determinant relations for matrices with zero row/column sums, cofactor expansion variants for constrained matrices |
| TotallyUnimodular.lean | Totally unimodular matrices: `Matrix.IsTotallyUnimodular` predicate (all square submatrices have determinant in {-1, 0, 1}), closure under transpose/submatrix/reindex, characterizations involving row/column augmentation with unit vectors |

## Subdirectories

## Search Tags

determinant matrix-determinant leibniz-formula permutation det-mul det-transpose multilinear-map alternating-map row-operations column-operations block-diagonal det-zero linear-independence cofactor-expansion totally-unimodular unimodular-matrix submatrix det-one det-diagonal sign-permutation
