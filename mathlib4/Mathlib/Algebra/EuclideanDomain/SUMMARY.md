---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/EuclideanDomain
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# EuclideanDomain

## Overview

The `EuclideanDomain/` directory defines Euclidean domains and their theory in mathlib4. A Euclidean domain is a non-trivial commutative ring with division and remainder operations satisfying `b * (a / b) + a % b = a`, equipped with a well-founded relation ensuring GCD algorithm termination. The implementation is generalized to support transfinite Euclidean domains where the degree function can take values in any well-ordered set (not just `ℕ`), following work by Motzkin, Hiblot, and Nagata. The directory provides core definitions, comprehensive theory including Bézout's lemma, and canonical instances showing that both fields and integers are Euclidean domains.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core `EuclideanDomain` typeclass definition with quotient/remainder operations and well-founded relation `r`, GCD algorithm implementation via recursion on `b % a`, extended Euclidean algorithm (`xgcd`, `xgcdAux`) computing `(x,y)` such that `gcd a b = x*a + y*b`, and LCM definition as `a * b / gcd a b` |
| Basic.lean | Comprehensive theory of Euclidean domains including division/modulus lemmas (`mod_eq_zero ↔ b ∣ a`, `div_self`, `mod_self`), Bézout's lemma `gcd_eq_gcd_ab` stating `gcd a b = a * gcdA a b + b * gcdB a b`, GCD properties (divisibility, uniqueness conditions), LCM theory with `gcd_mul_lcm`, and proof that Euclidean domains are integral domains with no zero divisors |
| Field.lean | Proves `Field.toEuclideanDomain` instance showing any field is a Euclidean domain with division `a/b`, remainder `a - a*b/b`, and trivial well-founded relation `r a b := a = 0 ∧ b ≠ 0`, includes simplified GCD formula `gcd a b = if a = 0 then b else a` for fields |
| Int.lean | Proves `Int.euclideanDomain` instance showing integers form a Euclidean domain using standard division/modulus (`ediv`/`emod`), with well-founded relation `r a b := a.natAbs < b.natAbs` based on absolute values ensuring GCD termination |

## Subdirectories

*(No subdirectories)*

## Search Tags

euclidean-domain transfinite-euclidean-domain gcd lcm bezout-lemma extended-euclidean-algorithm quotient remainder well-founded division-algorithm integral-domain field-instance int-instance xgcd
