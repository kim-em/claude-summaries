---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Eigenspace
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# Eigenspace

## Overview

The `Eigenspace/` directory contains mathlib4's formalization of eigenvalue theory for linear endomorphisms. Following Axler's basis-independent approach, it defines eigenspaces as kernels of `(f - μ • id)`, eigenvectors as nonzero elements of eigenspaces, and eigenvalues as scalars with nontrivial eigenspaces. The directory extends to generalized eigenspaces (kernels of `(f - μ • id) ^ k`), proves eigenvalues are roots of both minimal and characteristic polynomials, establishes the existence of eigenvalues over algebraically closed fields with spanning generalized eigenspaces (triangularizability), and covers special cases including diagonal matrices, semisimple endomorphisms, simultaneous eigenvalues for compatible families of endomorphisms, and the zero eigenvalue with connections to nilpotency.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core eigenspace theory: generalized eigenspaces `genEigenspace f μ k` as kernels of `(f - μ • id) ^ k`, eigenvector/eigenvalue predicates (`HasUnifEigenvector`, `HasUnifEigenvalue`, `UnifEigenvalues`), membership characterizations, monotonicity in exponents, maximal eigenspace index for Noetherian modules, relationship to spectrum, and eigenrange definitions |
| Charpoly.lean | Characteristic polynomial connection: eigenvalues are exactly the roots of the characteristic polynomial (`hasEigenvalue_iff_isRoot_charpoly`, `mem_spectrum_iff_isRoot_charpoly`), requires integral domain to avoid counterexamples |
| Minpoly.lean | Minimal polynomial connection: eigenvalues are roots of the minimal polynomial (`hasEigenvalue_iff_isRoot`), eigenvector evaluation formula `aeval f p x = p.eval μ • x`, finiteness of eigenvalues for finite-dimensional spaces, and Fintype instance for eigenvalue type |
| Matrix.lean | Matrix-specific eigenvalue theory: basis vectors as eigenvectors of diagonal operators (`hasEigenvector_toLin_diagonal`), eigenvalues of diagonal matrices are exactly diagonal entries (`hasEigenvalue_toLin_diagonal_iff`), supremum of diagonal eigenspaces equals top, and standard basis specializations |
| Pi.lean | Simultaneous eigenvalues for families of endomorphisms: compatibility condition (maximal generalized eigenspaces invariant under all family members), simultaneous generalized eigenspaces as intersections, independence of simultaneous eigenspaces, and spanning theorems when eigenspaces of individual maps span (generalizes commuting endomorphisms to compatible families from nilpotent Lie algebras) |
| Semisimple.lean | Eigenspaces of semisimple endomorphisms: for semisimple `f`, generalized eigenspaces equal ordinary eigenspaces (`IsFinitelySemisimple.genEigenspace_eq_eigenspace`), maximal generalized eigenspace equals eigenspace, proven via nilpotency of `f - μ • id` on eigenspace |
| Triangularizable.lean | Triangularizability over algebraically closed fields: existence of eigenvalue for finite-dimensional nontrivial spaces (`exists_eigenvalue`), generalized eigenspaces span the whole space (`iSup_maxGenEigenspace_eq_top`), restriction to invariant submodules preserves spanning, and inhabited instance for eigenvalue type |
| Zero.lean | Zero eigenvalue characterizations: nilpotency equivalent to characteristic polynomial `X ^ finrank` (`isNilpotent_iff_charpoly`), TFAE lists for nilpotent endomorphisms, eigenvalue 0 equivalences (nontrivial kernel, zero determinant, not injective), dimension of maximal generalized 0-eigenspace equals trailing degree of characteristic polynomial, and connections to Artinian modules |

## Subdirectories

(No subdirectories)

## Search Tags

eigenspace eigenvector eigenvalue generalized-eigenspace minimal-polynomial characteristic-polynomial spectrum triangularizable semisimple nilpotent diagonal-matrix simultaneous-eigenvalues compatible-families basis-independent axler algebraically-closed maximal-eigenspace zero-eigenvalue determinant kernel noetherian finite-dimensional
