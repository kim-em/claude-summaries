---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/IntegralClosure
generated: 2026-02-01T12:00:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: preliminary
files_count: 3
subdirs_count: 3
---

# IntegralClosure

## Overview

The `IntegralClosure/` directory formalizes the theory of integral closures in ring extensions. An element x of an R-algebra A is integral over R if it is a root of some monic polynomial with coefficients in R. The integral closure of R in A is the set of all such integral elements, forming a subalgebra. This directory provides the core definitions (`IsIntegral`, `Algebra.IsIntegral`, `IsIntegralClosure`, `IsIntegrallyClosed`), basic properties of integral elements and algebras, and advanced topics including restriction of Galois automorphisms to integral closures, integral trace/norm maps, the going-down theorem for integrally closed domains, and almost integral elements (complete integral closure).

## Key Files

| File | Purpose |
|------|---------|
| IntegrallyClosed.lean | Defines `IsIntegrallyClosedIn R A` and `IsIntegrallyClosed R` (R contains all integral elements of its fraction field); proves equivalence with being an integral closure, preservation under isomorphisms and localizations, and that fields are integrally closed |
| IntegralRestrict.lean | AKLB setup (A integrally closed, K = Frac(A), L finite extension of K, B = integral closure of A in L); defines `galRestrict` (restriction of Gal(L/K) to Aut(B/A)), `Algebra.intTrace` and `Algebra.intNorm` (trace/norm restricted to integral closures), proves transitivity and localization compatibility |
| GoingDown.lean | Proves the going-down theorem: for integral extensions R ⊆ S where R is integrally closed, the extension satisfies the going-down property for prime ideals (Stacks 00H8) |

## Subdirectories

- [x] `Algebra/` - Integral algebras: the class `Algebra.IsIntegral` (all elements integral), integral closure as a subalgebra, integrality over ideals
- [x] `IsIntegral/` - Core predicate `IsIntegral`: definition, basic properties (mapping, adjoin spans), almost integral elements and complete integral closure
- [x] `IsIntegralClosure/` - Characteristic predicate `IsIntegralClosure A R B` stating A is the integral closure of R in B; properties including inverse membership in division rings, equivalence of finite type + integral = finite

## Search Tags

integral-closure integrally-closed integral-element monic-polynomial IsIntegral Algebra.IsIntegral IsIntegralClosure integralClosure subalgebra fraction-ring FractionRing AKLB galois-restriction galRestrict integral-trace intTrace integral-norm intNorm going-down-theorem almost-integral complete-integral-closure algebraic-extension field-extension Dedekind-domain
