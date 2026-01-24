---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Charpoly
generated: 2026-01-25T09:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Charpoly

## Overview

The `Charpoly/` directory contains the formalization of characteristic polynomials for linear endomorphisms on finite free modules. It defines `LinearMap.charpoly f` as the characteristic polynomial of `f : M →ₗ[R] M`, proves the Cayley-Hamilton theorem (the characteristic polynomial annihilates the endomorphism), establishes basis-independence of the construction, and provides base change compatibility showing how characteristic polynomials behave under scalar extension. The implementation reduces to matrix characteristic polynomials via the chosen basis, with proofs that the result is independent of the choice of basis.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `LinearMap.charpoly` as the characteristic polynomial of the matrix representation in any chosen basis, basic properties (evaluation, monicity, degree), Cayley-Hamilton theorem (`aeval_self_charpoly`), integrality of endomorphisms, minimal polynomial divisibility, and reduction of polynomial evaluation modulo the characteristic polynomial |
| ToMatrix.lean | Basis-independence: proof that `charpoly f` equals the characteristic polynomial of the matrix of `f` in any basis (`charpoly_toMatrix`), product map compatibility (`charpoly_prodMap`), conjugation invariance (`LinearEquiv.charpoly_conj`), and reverse direction showing matrix characteristic polynomials agree with linear map characteristic polynomials |
| BaseChange.lean | Base change properties: characteristic polynomial commutes with scalar extension (`charpoly_baseChange`), determinant formula as signed coefficient (`det_eq_sign_charpoly_coeff`), and determinant base change compatibility |

## Subdirectories

(none)

## Search Tags

characteristic-polynomial cayley-hamilton linear-endomorphisms finite-free-modules basis-independence minimal-polynomial integrality determinant base-change matrix-polynomial polynomial-evaluation monic-polynomials
