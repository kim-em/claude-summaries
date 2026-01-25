---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/NumberField
generated: 2026-01-25T22:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 13
subdirs_count: 6
---

# NumberField

## Overview

The `NumberField/` directory contains the comprehensive formalization of algebraic number fields and their fundamental structures in Mathlib. A number field is defined as a finite-dimensional extension of ℚ with characteristic zero. This directory provides the complete infrastructure for algebraic number theory, from foundational definitions to deep theorems.

The ring of integers `𝓞 K` (the integral closure of ℤ in K) is formalized as a Dedekind domain with integral bases. The theory includes discriminants (with the Hermite-Minkowski theorem showing nontrivial fields have |discriminant| > 2), fractional ideals with ℤ-bases, and norm computations. Ideal theory encompasses asymptotic counting formulas, the Kummer-Dedekind criterion for prime splitting, and ramification theory.

Places form a central organizing principle: infinite places (from complex embeddings) come in real and complex variants, while finite places correspond to v-adic valuations from prime ideals. The canonical embedding maps K into ℝ^r₁ × ℂ^r₂ (where (r₁, r₂) is the signature), enabling geometric methods via lattice theory and Minkowski's Convex Body Theorem. This geometric framework underpins the proof of Dirichlet's Unit Theorem (units modulo torsion form a free ℤ-module of rank r₁ + r₂ - 1) and class number bounds.

Adele rings (products of all completions) provide a global-local perspective, while the product formula relates norms across all places. Special classes of number fields receive dedicated treatment: cyclotomic fields ℚ(ζₙ) with their ring of integers ℤ[ζₙ], discriminants, and PID results for small primes; CM-fields (totally complex quadratic extensions of totally real fields) with maximal real subfield theory; and totally real/complex fields characterized by their place structures. The Dedekind zeta function provides the analytic perspective on class numbers and regulators.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `NumberField` class, `RingOfIntegers` (𝓞 K) as integral closure of ℤ, integral bases, and instances showing ring of integers is Dedekind domain |
| AdeleRing.lean | Adele ring as product of infinite and finite adele rings, with principal subgroup of adeles |
| InfiniteAdeleRing.lean | Infinite adele ring as finite product of completions over infinite places, with ring isomorphism to ℝ^r₁ × ℂ^r₂ |
| ClassNumber.lean | Class number as cardinality of class group, Minkowski bound, theorems for proving ring of integers is PID |
| CMField.lean | CM-fields: totally complex quadratic extensions of totally real fields, with maximal real subfield theory |
| CanonicalEmbedding/ | Canonical embedding of number field into ℝ^r₁ × ℂ^r₂ based on real and complex places |
| Cyclotomic/ | Cyclotomic extensions specific to number fields |
| DedekindZeta.lean | Dedekind zeta function for number fields |
| Discriminant/ | Discriminant of number fields and related invariants |
| EquivReindex.lean | Reindexing equivalences for bases and embeddings |
| FinitePlaces.lean | Finite places as v-adic absolute values from non-zero prime ideals, with v-adic completions |
| FractionalIdeal.lean | Fractional ideals of number fields with ℤ-bases and norm computations |
| House.lean | House of algebraic number (maximum modulus of conjugates) |
| Ideal/ | Ideal theory specific to number fields |
| InfinitePlace/ | Infinite places (real and complex embeddings) and their completions |
| Norm.lean | Norm morphism between rings of integers for field extensions |
| ProductFormula.lean | Product formula relating absolute values across all places |
| Completion.lean | Import stub for completion theory |
| Units/ | Unit group structure and regulator theory |

## Subdirectories

- [x] `CanonicalEmbedding/` - Canonical embedding into product of completions
- [x] `Cyclotomic/` - Cyclotomic extension theory for number fields
- [x] `Discriminant/` - Discriminant computations and properties
- [x] `Ideal/` - Ideal theory in rings of integers
- [x] `InfinitePlace/` - Infinite places and their structure
- [x] `Units/` - Units in rings of integers, regulator

## Search Tags

number-field algebraic-number-theory ring-of-integers dedekind-domain integral-closure class-number adeles ideles fractional-ideal discriminant places infinite-places finite-places canonical-embedding CM-field totally-real totally-complex units regulator product-formula house norm-map cyclotomic v-adic completion
