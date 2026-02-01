---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/IntegralClosure
generated: 2026-02-01T00:28:26Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 3
subdirs_count: 3
---

# IntegralClosure

## Overview

The `IntegralClosure/` directory provides a comprehensive formalization of integral closures in ring extensions. An element x of an R-algebra A is integral over R if it is a root of some monic polynomial with coefficients in R. This directory builds the theory in layers: the core predicate `IsIntegral R x` for individual elements (with almost integral elements and complete integral closure), the typeclass `Algebra.IsIntegral R A` for when all elements are integral (with `integralClosure R A` as the subalgebra of integral elements), and the characteristic predicate `IsIntegralClosure A R B` for when A is exactly the integral closure of R in B (with properties like inverse membership in division rings and "integral + finite type = finite"). The top-level files then develop advanced topics: `IsIntegrallyClosed R` for domains containing all their integral elements, the AKLB setup with `galRestrict` (restricting Galois automorphisms to integral closures) and `intTrace`/`intNorm` (trace and norm on integral closures), and the going-down theorem for integrally closed domains.

## Key Files

| File | Purpose |
|------|---------|
| IntegrallyClosed.lean | Defines `IsIntegrallyClosedIn R A` and `IsIntegrallyClosed R` (R contains all integral elements of its fraction field); proves equivalence with being an integral closure, preservation under isomorphisms and localizations, and that fields are integrally closed |
| IntegralRestrict.lean | AKLB setup (A integrally closed, K = Frac(A), L finite extension of K, B = integral closure of A in L); defines `galRestrict` (restriction of Gal(L/K) to Aut(B/A)), `Algebra.intTrace` and `Algebra.intNorm` (trace/norm restricted to integral closures), proves transitivity and localization compatibility |
| GoingDown.lean | Proves the going-down theorem: for integral extensions R ⊆ S where R is integrally closed, the extension satisfies the going-down property for prime ideals (Stacks 00H8) |

## Subdirectories

- [x] `Algebra/` - Integral algebras: the typeclass `Algebra.IsIntegral R A` (all elements integral), `integralClosure R A` as a subalgebra closed under algebraic operations, integrality over ideals (Stacks 00H5), preservation under homomorphisms/products/tensor products
- [x] `IsIntegral/` - Core predicate `IsIntegral R x`: definition via monic polynomials, basic properties (mapping, tower compatibility, adjoin spans finitely generated), almost integral elements and `completeIntegralClosure` (equivalence with integral for Noetherian domains)
- [x] `IsIntegralClosure/` - Characteristic predicate `IsIntegralClosure A R B` stating A is the integral closure of R in B; inverse membership in division rings, `Algebra.IsIntegral.finite` (integral + finite type = finite), transitivity, lifting and equivalence of integral closures, integral closures of fields are fields

## Search Tags

integral-closure integrally-closed integral-element monic-polynomial IsIntegral RingHom.IsIntegralElem Algebra.IsIntegral IsIntegralClosure IsIntegrallyClosedIn IsIntegrallyClosed integralClosure subalgebra fraction-ring FractionRing AKLB galois-restriction galRestrict integral-trace intTrace integral-norm intNorm going-down-theorem Stacks-00H8 almost-integral IsAlmostIntegral completeIntegralClosure complete-integral-closure finite-type finite-module algebraic-extension field-extension Dedekind-domain Noetherian integrality-over-ideals Stacks-00H5 Stacks-00GW Stacks-00GX Kurosh-problem
