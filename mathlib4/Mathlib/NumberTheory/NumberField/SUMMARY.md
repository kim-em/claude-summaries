---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/NumberField
generated: 2026-01-25T19:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 13
subdirs_count: 6
---

# NumberField

## Overview

The `NumberField/` directory contains the formalization of algebraic number fields and their fundamental structures. A number field is defined as a finite-dimensional extension of ℚ with characteristic zero. The directory encompasses the ring of integers (𝓞 K), adele rings (both finite and infinite), fractional ideals, class numbers, discriminants, places (infinite and finite), units, canonical embeddings, and CM-fields (totally complex quadratic extensions of totally real fields). This provides the foundational infrastructure for algebraic number theory in Mathlib.

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
- [ ] `Cyclotomic/` - Cyclotomic extension theory for number fields
- [ ] `Discriminant/` - Discriminant computations and properties
- [ ] `Ideal/` - Ideal theory in rings of integers
- [ ] `InfinitePlace/` - Infinite places and their structure
- [ ] `Units/` - Units in rings of integers, regulator

## Search Tags

number-field algebraic-number-theory ring-of-integers dedekind-domain integral-closure class-number adeles ideles fractional-ideal discriminant places infinite-places finite-places canonical-embedding CM-field totally-real totally-complex units regulator product-formula house norm-map cyclotomic v-adic completion
