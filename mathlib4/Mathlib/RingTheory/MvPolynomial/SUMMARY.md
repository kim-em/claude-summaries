---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/MvPolynomial
generated: 2026-02-01T22:00:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 12
subdirs_count: 2
---

# MvPolynomial

## Overview

This directory contains ring-theoretic results about multivariate polynomials that go beyond the basic algebra in `Mathlib.Algebra.MvPolynomial`. The core topics are: homogeneous polynomials (both uniform total degree and weighted variants) with Euler's identity and component decomposition; monomial orders with associated division algorithms for Gröbner basis computations; and symmetric polynomials including the fundamental theorem and Newton's identities.

Additional topics include: characteristic propagation and basis structures; Frobenius expansion maps; free commutative ring constructions for model theory; irreducibility criteria for linear and quadratic polynomials; localization of polynomial rings; and algebra tower structures.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Foundational ring theory: characteristic propagation (CharP, CharZero, ExpChar), monomial basis construction, submodules of restricted total/individual degree, freeness of polynomial modules |
| EulerIdentity.lean | Euler's homogeneous function identity: for homogeneous polynomials, sum of X_i * (partial derivative w.r.t. X_i) equals degree times the polynomial; weighted version included |
| Expand.lean | Interaction of `MvPolynomial.expand` (substitution X_i -> X_i^p) with Frobenius map: `(expand p f).map frobenius = f^p`; iteration to arbitrary powers |
| FreeCommRing.lean | Tools for constructing ring terms from MvPolynomials via FreeCommRing; `genericPolyMap` for model-theoretic formula construction |
| Groebner.lean | Division algorithm for monomial orders: given polynomials with invertible leading coefficients, computes quotients and remainder with degree bounds; `reduce`, `subLTerm` helper operations |
| Homogeneous.lean | Homogeneous polynomials (monomials of uniform total degree): `IsHomogeneous` predicate, `homogeneousSubmodule`, `homogeneousComponent` projection, decomposition of polynomials into homogeneous parts |
| Ideal.lean | Monomial ideal theory: characterization of membership in span of monomials via support domination; S-polynomial membership in ideals; span of leading terms |
| IrreducibleQuadratic.lean | Irreducibility criteria: linear polynomials of degree 1 with coprime coefficients; linear `sumSMulX`; quadratic `sumSMulXSMulY` with disjoint support; `irreducible_mul_X_add` helper |
| Localization.lean | Localization of MvPolynomial rings: `MvPolynomial σ S` is localization of `MvPolynomial σ R` at image of submonoid; quotient presentation of localization away from element |
| MonomialOrder.lean | Monomial order theory: `degree`, `leadingCoeff`, `Monic`, `leadingTerm`, `sPolynomial`; degree bounds for arithmetic operations; leading coefficient behavior under products and powers |
| Tower.lean | Algebra tower results: `aeval` commutes with `map algebraMap`; behavior of evaluation through algebra maps; subalgebra evaluation lemmas |
| WeightedHomogeneous.lean | Weighted homogeneous polynomials: `weightedTotalDegree'` (WithBot M), `weightedTotalDegree` (M with bot), `IsWeightedHomogeneous`, `weightedHomogeneousSubmodule`, decomposition into weighted components |

## Subdirectories

- [x] `MonomialOrder/` - Degree-lexicographic order: connects `degLex` ordering to total degree, proves `degree_degLexDegree` and monotonicity
- [x] `Symmetric/` - Symmetric polynomials: elementary/complete homogeneous/power sum/monomial symmetric bases; fundamental theorem (subalgebra isomorphism via esymm); Newton's identities via Zeilberger's involution

## Search Tags

multivariate-polynomial ring-theory homogeneous weighted-homogeneous monomial-order Groebner-basis leading-coefficient leading-term S-polynomial division-algorithm irreducibility localization algebra-tower characteristic Euler-identity expansion Frobenius free-commutative-ring monomial-ideal symmetric-polynomial elementary-symmetric Newton-identities degLex
