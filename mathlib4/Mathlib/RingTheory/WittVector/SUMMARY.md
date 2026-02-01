---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/WittVector
generated: 2026-02-01T23:30:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: complete
files_count: 20
subdirs_count: 0
---

# WittVector

## Overview

The `WittVector/` directory contains a comprehensive formalization of p-typical Witt vectors, fundamental objects in commutative algebra and arithmetic geometry. Witt vectors provide a canonical way to construct rings of characteristic 0 from rings of characteristic p, with the key example being the p-adic integers constructed from ℤ/pℤ. The implementation defines the type `WittVector p R` as infinite sequences `ℕ → R` with non-standard ring operations defined via structure polynomials, and establishes the complete ring structure, functoriality (map operation), ghost component theory, specialized operators (Frobenius, Verschiebung, Teichmüller), truncated variants, and connections to fraction fields and isocrystals.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of `WittVector p R` as structure with `coeff : ℕ → R`; defines ring operations (zero, one, add, mul, neg, sub, nsmul, zsmul, pow) via structure polynomials; proves basic simplifications and coefficient formulas |
| Basic.lean | Verifies ring axioms for Witt vectors; defines `map : (R →+* S) → (𝕎 R →+* 𝕎 S)` for functoriality; introduces `ghostMap : 𝕎 R →+* (ℕ → R)` and proves it's an isomorphism when p is invertible in R; establishes `constantCoeff : 𝕎 R →+* R` |
| StructurePolynomial.lean | Develops the polynomial machinery underlying Witt vector operations; defines Witt polynomials `W_n`, structure polynomials, and `xInTermsOfW` converting between coefficient and ghost component representations |
| WittPolynomial.lean | Defines the Witt polynomials `W_n = X_0^(p^n) + p·X_1^(p^(n-1)) + ... + p^n·X_n` used in ghost component theory |
| Frobenius.lean | Defines Frobenius endomorphism `frobeniusFun : 𝕎 R → 𝕎 R` via polynomials that work for all rings; proves that in characteristic p it equals `map (frobenius R p)`; shows Frobenius is polynomial function |
| FrobeniusFractionField.lean | Lifts Frobenius to fraction field automorphism when R is a domain of characteristic p; proves it's an isomorphism and establishes compatibility with ghost components |
| Verschiebung.lean | Defines Verschiebung operator (shift coefficients up by one, inserting 0); establishes relationship with ghost components: `ghostComponent (n+1) (verschiebung x) = p · ghostComponent n x` |
| Teichmuller.lean | Defines Teichmüller lift `teichmuller : R →* 𝕎 R` embedding r as 0th coefficient with other coefficients 0; proves it's a monoid homomorphism and `ghostComponent n (teichmuller r) = r^(p^n)` |
| TeichmullerSeries.lean | Establishes that Teichmüller map respects addition for perfect rings of characteristic p using the binomial theorem and summation formulas |
| Truncated.lean | Defines truncated Witt vectors `TruncatedWittVector p n R` as first n coefficients; establishes quotient structure with `truncate : 𝕎 R → TruncatedWittVector p n R`; proves Witt vectors are projective limit of truncated versions via `lift` |
| InitTail.lean | Decomposes Witt vectors into initial segment and tail; provides `init` and `tail` operations for working with finite prefixes |
| Compare.lean | Comparison and ordering results for Witt vectors when R is ordered |
| Complete.lean | Establishes completeness properties of Witt vectors with respect to truncation topology |
| Identities.lean | Collection of algebraic identities involving Witt vector operations, ghost components, and structure polynomials |
| MulCoeff.lean | Detailed analysis of multiplication coefficients; proves formulas for computing (x * y).coeff n from x.coeff and y.coeff |
| MulP.lean | Properties of multiplication by p in Witt vectors; short-circuits for characteristic p calculations |
| IsPoly.lean | Framework for polynomial functions on Witt vectors; establishes that various operations (add, mul, Frobenius, Verschiebung) are polynomial in the coefficients |
| Isocrystal.lean | Defines F-isocrystals over perfect fields as vector spaces over K(p,k) with Frobenius-linear automorphisms; proves one-dimensional classification theorem (Dieudonné-Manin) |
| DiscreteValuationRing.lean | Proves that Witt vectors over a perfect field of characteristic p form a discrete valuation ring |
| Domain.lean | Establishes that WittVector p k is an integral domain when k is |

## Subdirectories

(none)

## Search Tags

Witt-vectors p-typical p-adic integers characteristic-p characteristic-0 lift structure-polynomial ghost-component Witt-polynomial Frobenius Verschiebung Teichmuller truncated-Witt-vectors projective-limit isocrystal Dieudonne-Manin perfect-field discrete-valuation-ring DVR ghost-map polynomial-function fraction-field perfect-ring binomial commutative-algebra arithmetic-geometry
