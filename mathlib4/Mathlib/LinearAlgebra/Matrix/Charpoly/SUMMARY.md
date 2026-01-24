---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Matrix/Charpoly
generated: 2026-01-25T10:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# Charpoly

## Overview

The `Charpoly/` subdirectory contains mathlib4's comprehensive formalization of characteristic polynomials for matrices, including the Cayley-Hamilton theorem over arbitrary commutative rings. The directory establishes fundamental definitions (characteristic matrix `charmatrix`, characteristic polynomial `charpoly`), proves key structural results (degree formulas, coefficient characterizations connecting trace and determinant), and develops specialized theory for eigenvalues, minimal polynomials, finite fields, and generalized module endomorphisms. Notable highlights include the proof that eigenvalues are precisely the roots of the characteristic polynomial, the universal characteristic polynomial with multivariate polynomial coefficients, and extensions of Cayley-Hamilton to finitely generated modules.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and Cayley-Hamilton theorem: `charmatrix` (matrix `XI - C(M)`), `charpoly` (determinant of charmatrix), proof of `aeval M M.charpoly = 0` via elegant argument from Dror Bar-Natan, simp lemmas for charmatrix of special matrices |
| Coeff.lean | Coefficient analysis of characteristic polynomials: `charpoly_degree_eq_dim` (degree equals matrix dimension), `det_eq_sign_charpoly_coeff` (determinant as constant term up to sign), `trace_eq_neg_charpoly_coeff` (trace as negative of second-highest coefficient), `charpolyRev` (reverse polynomial), coefficient comparison with diagonal product |
| Eigs.lean | Eigenvalue-characteristic polynomial connection: `mem_spectrum_iff_isRoot_charpoly` (eigenvalues are exactly the charpoly roots in fields), `det_eq_prod_roots_charpoly` and `trace_eq_sum_roots_charpoly` in algebraically closed fields, splitting versions for general fields, expresses trace/det as sum/product of eigenvalues |
| Disc.lean | Matrix discriminant: `Matrix.discr` defined as discriminant of characteristic polynomial, specialized formula for 2×2 matrices (`discr = trace² - 4·det`), deprecation of old `disc` naming |
| FiniteField.lean | Characteristic polynomials over finite fields: `charpoly_pow_card` (characteristic polynomial of `M^q` equals that of `M` for field of size `q`), `trace_pow_card` identity using Frobenius, specialized versions for `ZMod p` |
| LinearMap.lean | Cayley-Hamilton for finitely generated modules: matrix representation of endomorphisms via spanning sets (`Matrix.Represents`), existence of matrix representations with entries in ideals when range is bounded, proves Cayley-Hamilton for f.g. modules over arbitrary rings by reducing to matrix case |
| Minpoly.lean | Minimal polynomial relations: `minpoly_dvd_charpoly` (minimal polynomial divides characteristic polynomial over fields), compatibility of minpoly under matrix-linear map correspondences (`minpoly_toLin`, `minpoly_toMatrix`), `charpoly_leftMulMatrix` (charpoly of left multiplication is minpoly for power basis) |
| Univ.lean | Universal characteristic polynomial: `Matrix.charpoly.univ` (charpoly of matrix with symbolic entries `Xᵢⱼ` as multivariate polynomials), homogeneity of coefficients (`univ_coeff_isHomogeneous`: i-th coefficient is homogeneous of degree n-i), evaluation at concrete matrix entries recovers ordinary charpoly |

## Subdirectories

*(none)*

## Search Tags

characteristic-polynomial charpoly cayley-hamilton charmatrix eigenvalues spectrum minimal-polynomial trace determinant coefficients finite-fields frobenius discriminant finitely-generated-modules matrix-representation universal-polynomial homogeneous-polynomials multivariate-polynomials algebraically-closed splitting-field roots power-basis
