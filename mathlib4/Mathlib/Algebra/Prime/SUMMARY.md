---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Prime
generated: 2025-12-04T02:35:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Prime

## Overview

The `Prime/` directory defines the fundamental notion of prime elements in commutative monoids with zero. It establishes the key predicate `Prime p` requiring that `p` is nonzero, not a unit, and satisfies the prime divisibility property: `p ∣ a * b → p ∣ a ∨ p ∣ b`. The directory contains both the core definition and a comprehensive theory of prime elements, including their relationship to irreducible elements (which are equivalent in decomposition monoids via `irreducible_iff_prime`), power divisibility properties, and interactions with monoid homomorphisms.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `Prime p` predicate for commutative monoids with zero, basic properties (ne_zero, not_unit, dvd_or_dvd), power divisibility lemmas, and fundamental theorem `irreducible_iff_prime` in decomposition monoids |
| Lemmas.lean | Extended theory of prime elements: homomorphism transport via `comap_prime` and `MulEquiv.prime_iff`, advanced divisibility results for powers (`pow_dvd_of_dvd_mul_left`, `succ_dvd_or_succ_dvd_of_succ_sum_dvd_mul`), non-squareness of primes, and auxiliary results on `DvdNotUnit` and power injectivity |

## Subdirectories

(None - this is a leaf directory)

## Search Tags

prime prime-elements irreducible divisibility commutative-monoid decomposition-monoid dvd-or-dvd pow-divisibility monoid-homomorphism cancel-monoid primal not-square algebra-foundations
