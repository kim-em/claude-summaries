---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Matrix
generated: 2025-12-09T00:00:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 15
subdirs_count: 0
---

# Matrix

## Overview

The `Matrix/` directory contains the core definition and operations on matrices in mathlib4. Matrices are defined as `m → n → α` (functions from row indices to column indices to values), with this file collection providing basic matrix algebra including addition, scalar multiplication, matrix multiplication, transpose, diagonal matrices, block matrices, and invertibility. The files establish matrices as rings (when square), modules, and algebras, along with bundled morphisms and specialized operations for working with concrete finite matrices, partial equivalences, and dual numbers.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core matrix theory: bundled versions of operators (linear equivalences, additive/linear homomorphisms for diagonal matrices); decidable equality and fintype instances; sum operations on matrices |
| Mul.lean | Matrix multiplication operations: defines dot product (`⬝ᵥ`), matrix multiplication, `mulVec` (`*ᵥ`), `vecMul` (`ᵥ*`), `vecMulVec`; establishes ring structure on square matrices |
| Diagonal.lean | Diagonal matrices and related structures: `Matrix.diagonal d` creates diagonal matrix from vector `d`; `Matrix.diag M` extracts diagonal; `AddCommMonoidWithOne` instance for matrices |
| Block.lean | Block matrix operations: `fromBlocks` constructs matrix from 4 blocks, `toBlocks₁₁/₁₂/₂₁/₂₂` extract blocks; `blockDiagonal` for equally-sized blocks with ring homomorphism; `blockDiagonal'` for unequally-sized blocks |
| Basis.lean | Matrices with single non-zero element: `Matrix.single i j a` has `a` at position `(i,j)` and zeros elsewhere; previously called `stdBasisMatrix`; includes transpose and smul lemmas |
| Invertible.lean | Invertibility theory for matrices: lemmas about invertible matrices, cancellation properties for rectangular matrix multiplication; `invertibleConjTranspose`, `invertibleTranspose`, and unit characterizations |
| ColumnRowPartitioned.lean | Row and column concatenation: `fromRows` concatenates matrices vertically (same columns), `fromCols` horizontally (same rows); extraction functions `toRows₁/₂` and `toCols₁/₂`; products with block matrices |
| Composition.lean | Matrix composition equivalences: `Matrix.comp` shows `Mₙ(Mₘ(R)) ≃ Mₙₘ(R)` via Cartesian product of indices; `Matrix.swap` for index reordering; preserves algebraic structures (AddCommMonoid, Semiring, Algebra) |
| Bilinear.lean | Bundled bilinear forms of matrix multiplication: `mulLeftLinearMap` and `mulRightLinearMap` for heterogeneous matrix multiplication; coincides with `LinearMap.mulLeft/mulRight` on square matrices |
| PEquiv.lean | Partial equivalence representation: `PEquiv.toMatrix` converts partial equivalences to 0-1 matrices where `f.toMatrix i j = 1 ↔ f i = some j`; composition corresponds to matrix multiplication; represents projection maps |
| Action.lean | Module structures via matrix-vector multiplication: left-module structure via `*ᵥ` (mulVec) and right-module structure via `ᵥ*` (vecMul) on opposite algebra; scalar tower and commutativity instances |
| DMatrix.lean | Dependent-typed matrices: `DMatrix m n α` where `α : m → n → Type`; provides map, transpose, row/col constructors; algebraic instances (Add, AddSemigroup, etc.) for dependent matrices |
| Reflection.lean | Definitional lemmas for concrete finite matrices: alternative definitions that expand definitionally on `!![]` notation; enables proof by reflection via `Matrix.etaExpand`; includes `transposeᵣ`, `dotProductᵣ`, `mulᵣ`, etc. |
| Auto.lean | Placeholder for automatically generated lemmas: infrastructure for "magic" lemmas that auto-generate for concrete matrix sizes; Lean 3 functionality not yet ported (should use simprocs) |
| DualNumber.lean | Isomorphism between matrices of dual numbers and dual numbers of matrices: `Matrix.dualNumberEquiv : Matrix n n (DualNumber R) ≃ₐ[R] DualNumber (Matrix n n R)` |

## Subdirectories

*(no subdirectories)*

## Search Tags

matrices matrix-multiplication linear-algebra dot-product transpose diagonal-matrices block-matrices invertible-matrices partial-equivalences matrix-vector-multiplication dependent-matrices dual-numbers bilinear-forms composition ring-structure module-structure algebra
