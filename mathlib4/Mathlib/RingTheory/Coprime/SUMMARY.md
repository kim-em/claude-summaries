---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Coprime
generated: 2026-01-26T21:35:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 3
subdirs_count: 0
---

# Coprime

## Overview

The `Coprime/` directory formalizes coprimality of ring elements using the Bézout identity (existence of `a`, `b` such that `a*x + b*y = 1`), which is stronger than the relatively prime condition (no common divisors). The directory provides the core definition `IsCoprime`, parallel development of `IsRelPrime` for elements with no common divisors, and extensive lemmas about both notions including interactions with products, powers, ring operations, and applications to ideals. This notion is fundamental to ring theory and appears in many classical results about factorization and divisibility.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `IsCoprime` as Bézout identity; basic properties (symmetry, coprime with units, products, divisibility lemmas); parallel development of `IsRelPrime` lemmas; group scalar action compatibility; handling negation and absolute values in ordered rings |
| Lemmas.lean | Extended lemmas requiring BigOperators: product and power lemmas for both `IsCoprime` and `IsRelPrime`; pairwise coprimality characterizations; connection between `IsCoprime` for integers and `Int.gcd`; finite product divisibility results |
| Ideal.lean | Generalization of pairwise coprimality to ideals: `iSup_iInf_eq_top_iff_pairwise` theorem relating suprema of intersections to pairwise coprimality of ideals (non-principal version of `exists_sum_eq_one_iff_pairwise_coprime`) |

## Subdirectories

(none)

## Search Tags

coprime IsCoprime Bezout-identity relatively-prime IsRelPrime gcd pairwise-coprime ideal-coprime divisibility ring-theory commutative-algebra product power finite-product
