---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/FieldTheory/IsAlgClosed
generated: 2026-01-24T22:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# IsAlgClosed

## Overview

This directory contains the theory of algebraically closed fields and algebraic closures in Lean. It defines the `IsAlgClosed` typeclass (fields where every polynomial splits) and `IsAlgClosure` typeclass (algebraic closures of a base ring), constructs the algebraic closure of any field, proves uniqueness of algebraic closures up to isomorphism, classifies algebraically closed fields by characteristic and transcendence degree, and develops the spectral mapping theorem for polynomials over algebraically closed fields.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and properties: defines `IsAlgClosed` (every polynomial splits), `IsAlgClosure R K` (K is algebraic closure of R), proves existence of roots for polynomials, shows irreducible polynomials have degree 1, establishes that algebraically closed fields are perfect and infinite, proves lift theorem for extending homomorphisms to algebraically closed fields |
| AlgebraicClosure.lean | Explicit construction of algebraic closure: constructs `AlgebraicClosure k` as quotient of multivariate polynomial ring by maximal ideal, proves it is algebraically closed and algebraic over k, establishes that any two algebraic closures are isomorphic via `IsAlgClosure.equiv` |
| Classification.lean | Classification of algebraically closed fields: proves two algebraically closed fields with same characteristic and same cardinality of transcendence basis are isomorphic (`equivOfTranscendenceBasis`), establishes cardinality bounds for algebraically closed fields in terms of transcendence degree, shows uncountable algebraically closed fields with same characteristic and cardinality are isomorphic |
| Spectrum.lean | Spectral mapping theorem and applications: proves spectral mapping theorem for polynomials over algebraically closed fields (spectrum of p(a) equals image of spectrum of a under p), shows every element in finite-dimensional algebra over algebraically closed field has nonempty spectrum (`nonempty_of_isAlgClosed_of_finiteDimensional`), characterizes spectrum of idempotent elements as subset of {0,1} |

## Subdirectories

(None)

## Search Tags

algebraically-closed algebraic-closure splitting-fields polynomial-roots isomorphism-theorems classification transcendence-basis cardinality spectral-mapping-theorem spectrum eigenvalues finite-dimensional-algebras perfect-fields infinite-fields algebraic-extensions field-extensions galois-theory
