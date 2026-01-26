---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Algebraic
generated: 2026-01-26T20:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# Algebraic

## Overview

The `Algebraic/` directory contains the core theory of algebraic and transcendental elements in ring extensions. An element of an R-algebra is algebraic over R if it is a root of a nonzero polynomial with coefficients in R; otherwise it is transcendental. The directory establishes the fundamental definitions, proves the relationship between algebraic and integral elements (algebraic equals integral over fields), proves transitivity of algebraic extensions, and provides specialized results for polynomial algebras, multivariate polynomials, and strongly transcendental elements (a notion useful for Zariski's main theorem).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of algebraic and transcendental elements; `IsAlgebraic`, `Transcendental`, `Algebra.IsAlgebraic`, `Algebra.Transcendental` for both elements and algebras; equivalence between element-wise and global algebraicity |
| Basic.lean | Fundamental results including transitivity of algebraicity, characterization via kernel of evaluation map, preservation under algebra homomorphisms, polynomial indeterminates are transcendental, composition of algebraic/transcendental elements |
| Integral.lean | Relationship between algebraic and integral elements; proves integral implies algebraic, and algebraic equals integral over fields; finite-dimensional modules are algebraic; algebraic elements have integral multiples; transitivity of algebraic extensions; algebraic closure as subalgebra |
| Cardinality.lean | Cardinality bounds for algebraic extensions; proves algebraic extension has cardinality at most max(#R, ℵ₀) via counting roots of polynomials |
| LinearIndependent.lean | Linear independence of transcendental elements; for transcendental x over field F, the set {(x - a)⁻¹ \| a : F} is linearly independent over F |
| MvPolynomial.lean | Transcendentality in multivariate polynomial rings; proves variables X i are transcendental over base ring and over subalgebras supported on disjoint variable sets |
| Pi.lean | Algebraic functions as elements of function spaces R → S; defines non-instance SMul and Algebra structures on R[X] acting on function types via evaluation |
| StronglyTranscendental.lean | Strongly transcendental elements (useful for Zariski's main theorem); element x is strongly transcendental if p(x) * u = 0 implies p * u = 0; equivalent to transcendental for fields and fraction rings; stable under localization and quotients by minimal primes |

## Subdirectories

(none)

## Search Tags

algebraic transcendental integral polynomial-root algebra-extension field-extension tower-law cardinality multivariate-polynomial strongly-transcendental Zariski linear-independence evaluation-homomorphism kernel finite-dimensional minimal-polynomial
