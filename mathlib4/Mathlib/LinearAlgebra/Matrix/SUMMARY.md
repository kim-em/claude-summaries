---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Matrix
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 53
subdirs_count: 4
---

# Matrix

## Overview

The `Matrix/` directory contains mathlib4's comprehensive formalization of matrix theory, bridging concrete matrix computations with abstract linear algebra. It defines matrices as functions `m → n → α` with extensive support for matrix operations (multiplication, transpose, conjugate transpose), structural properties (rank, trace, determinant), and equivalences between matrices and linear maps. The directory covers both computational aspects (Cramer's rule, matrix inversion via adjugate, Kronecker products) and theoretical foundations (basis conversions, positive definiteness, special matrix groups), with specialized support for notation (`!![a, b; c, d]` syntax) and connections to quadratic/bilinear/sesquilinear forms.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core matrix definitions: `Matrix m n α` as `m → n → α`, transpose, map, submatrix, module structure, and extensionality |
| ToLin.lean | Matrix-linear map correspondence: `Matrix.toLin` and `LinearMap.toMatrix` as equivalences between matrices and linear maps with respect to bases, bilinear versions for matrix-vector products |
| Notation.lean | Matrix notation system: `!![a, b; c, d]` syntax for constructing matrices via `Matrix.of`, parser for empty matrices, and simp lemmas for operations on notation-built matrices |
| Basis.lean | Basis-matrix conversions: `Basis.toMatrix` sends families of vectors to coordinate matrices, equivalences between basis changes and matrix multiplication |
| NonsingularInverse.lean | Matrix inversion: invertibility via determinant (adjugate/det formula), equivalence between matrix invertibility and determinant invertibility, Cramer's rule for solving linear systems |
| Adjugate.lean | Adjugate matrices and Cramer's rule: `Matrix.cramer` for column replacement determinants, `Matrix.adjugate` as transpose of cofactor matrix, properties `adjugate * A = det A • I` |
| Trace.lean | Matrix trace: sum of diagonal entries with additive/linear structure, trace of products and transposes, connection to endomorphism trace |
| Rank.lean | Matrix rank: `Matrix.rank` as dimension of column space, cardinal rank `cRank`, extended rank `eRank`, rank inequalities for submatrices and products |
| Block.lean | Block matrix operations: construction from blocks, extraction of submatrices, block diagonal matrices, and lemmas for operations on block matrices |
| BilinearForm.lean | Matrices of bilinear forms: conversion between bilinear forms and matrices via bases, matrix representations of form composition and base change |
| SesquilinearForm.lean | Matrices of sesquilinear forms: conversion between sesquilinear forms and matrices (including conjugate-linear structure), form-matrix correspondence, hermitian forms |
| DotProduct.lean | Dot products and matrix-vector multiplication: `dotProduct`, `mulVec` (matrix-vector product), `vecMul` (vector-matrix product), and their bilinear properties |
| Diagonal.lean | Diagonal matrices: `Matrix.diagonal` constructs diagonal matrices from functions, properties of diagonal operations, scalar matrix construction |
| PosDef.lean | Positive definite matrices: `Matrix.PosDef` (xᴴMx > 0 for nonzero x) and `Matrix.PosSemidef` (xᴴMx ≥ 0), connection to quadratic forms, Schur complement criteria |
| Hermitian.lean | Hermitian matrices: `Matrix.IsHermitian` (Aᴴ = A), properties under operations, eigenvalue characterization, star-ordered ring structure |
| ConjTranspose.lean | Conjugate transpose: `Matrix.conjTranspose` (notation `ᴴ`), interaction with operations, involutive properties, relationship to transpose and star |
| Kronecker.lean | Kronecker products: `Matrix.kroneckerMap` for generalized tensor products, specialized to `⊗ₖ` (scalar multiplication) and `⊗ₖₜ` (tensor product), bilinearity and trace properties |
| Transvection.lean | Transvection matrices: elementary row/column operations (adding scalar multiple of one row to another), generation of SL(n), Gaussian elimination, LU decomposition foundations |
| SpecialLinearGroup.lean | Special linear group: `Matrix.SpecialLinearGroup n R` as matrices with determinant 1, group structure, equivalence with `SL(n, R)` for modules |
| GeneralLinearGroup.lean | Import aggregator: delegates general linear group theory to `GeneralLinearGroup/` subdirectory |
| SchurComplement.lean | Schur complements: `M.schurComplement A` for block matrices, determinant formula via Schur complements, invertibility criteria for block matrices |
| Reindex.lean | Matrix reindexing: `Matrix.reindex` for changing index types via equivalences, preservation of operations under reindexing |
| RowCol.lean | Row and column operations: extracting/updating rows and columns, `Matrix.row`, `Matrix.col`, row/column equivalence to vectors |
| Permutation.lean | Permutation matrices: matrices corresponding to permutations of rows/columns, relationship to determinant sign |
| Swap.lean | Row and column swaps: elementary permutation operations, effect on determinant |
| Polynomial.lean | Polynomial matrices: matrices with polynomial entries, evaluation maps, and connections to characteristic polynomials |
| Module.lean | Module structure on matrices: explicit module instances, compatibility with matrix operations |
| ToLinearEquiv.lean | Linear equivalences from invertible matrices: `Matrix.toLinearEquiv` when matrix is invertible, group structure on `GLₙ(R)` |
| StdBasis.lean | Standard basis matrices: matrices with single 1 entry and 0s elsewhere, coordinate projection properties |
| InvariantBasisNumber.lean | Invariant basis number for matrices: matrices over rings with invariant basis number preserve dimension |
| Circulant.lean | Circulant matrices: matrices constant on diagonals, construction from first row, eigenvalue properties |
| FixedDetMatrices.lean | Matrices with fixed determinant: subsets of matrices with specified determinant value, algebraic structure |
| Gershgorin.lean | Gershgorin circle theorem: bounds on eigenvalues via row sums, localization of spectrum |
| Hadamard.lean | Hadamard product: entrywise matrix multiplication (Schur product), bilinearity, and trace properties |
| Ideal.lean | Matrix ideals: ideals generated by matrix entries, properties for matrices over commutative rings |
| IsDiag.lean | Diagonal matrix predicate: `Matrix.IsDiag` for matrices with off-diagonal zeros, characterization lemmas |
| MvPolynomial.lean | Multivariate polynomial matrices: matrices with polynomial entries, evaluation and algebraic properties |
| Nondegenerate.lean | Nondegenerate matrices: matrices with trivial kernel/cokernel, full rank characterization |
| Orthogonal.lean | Import aggregator for orthogonal matrices (some content may be in other files or subdirectories) |
| Permanent.lean | Matrix permanent: permanent of a matrix (like determinant but all positive signs), combinatorial properties |
| ProjectiveSpecialLinearGroup.lean | Projective special linear group: PSL(n) as quotient of SL(n) by scalar matrices |
| SemiringInverse.lean | Inverses in semiring context: matrix inversion when only semiring structure available, relationship to units |
| Symmetric.lean | Symmetric matrices: `Matrix.IsSymm` (Aᵀ = A), properties under operations, relationship to bilinear forms |
| Unique.lean | Uniqueness properties for special matrices |
| Vec.lean | Vector operations: viewing vectors as single-column or single-row matrices, conversion lemmas |
| ZPow.lean | Integer powers of matrices: `A ^ n` for integer n (including negative powers when invertible) |
| AbsoluteValue.lean | Absolute value on matrices: extending absolute values from scalars to matrices |
| BaseChange.lean | Base change for matrices: scalar extension, behavior under ring homomorphisms |
| CharP.lean | Characteristic p properties for matrices over rings of characteristic p |
| Dual.lean | Dual space constructions for matrices: relationship between matrix spaces and their duals |
| FiniteDimensional.lean | Finite-dimensionality for matrix spaces: dimension formulas, basis constructions |
| HermitianFunctionalCalculus.lean | Import aggregator for functional calculus on hermitian matrices |
| Integer.lean | Integer matrices: properties specific to matrices over ℤ, divisibility, and determinant bounds |
| LDL.lean | LDL decomposition: factorization of matrices as LDLᵀ for symmetric/hermitian matrices |
| Charpoly | Characteristic polynomial subdirectory (detailed in child SUMMARY.md) |
| Determinant | Determinant theory subdirectory (detailed in child SUMMARY.md) |
| GeneralLinearGroup | General linear group subdirectory (detailed in child SUMMARY.md) |
| Irreducible | Irreducible matrices subdirectory (detailed in child SUMMARY.md) |

## Subdirectories

- [x] `Charpoly/` - Characteristic polynomials of matrices
- [x] `Determinant/` - Determinant theory and computation
- [ ] `GeneralLinearGroup/` - General linear group GL(n) theory
- [ ] `Irreducible/` - Irreducible matrices and primitivity

## Search Tags

matrix matrices linear-algebra matrix-multiplication transpose conjugate-transpose trace determinant rank adjugate inverse cramer-rule basis-change matrix-notation kronecker-product block-matrices bilinear-forms sesquilinear-forms dot-product diagonal hermitian positive-definite special-linear-group general-linear-group transvection schur-complement reindex permutation-matrix polynomial-matrix circulant gershgorin hadamard-product permanent symmetric-matrix orthogonal characteristic-polynomial finite-dimensional
