---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/Padics/PadicVal
generated: 2026-01-25T09:30:00Z
git_sha: 64c76eabb64d58848cd5a272f58dfa31f3d1e3ea
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# PadicVal

## Overview

The `PadicVal/` directory contains the foundational definitions and theory of p-adic valuations on natural numbers, integers, and rationals. The p-adic valuation `padicValNat p n` is the largest power of `p` dividing `n`, extended to integers via absolute value and to rationals as the difference between numerator and denominator valuations. The directory includes comprehensive arithmetic properties (multiplicativity, divisibility characterizations), efficient implementation via `maxPowDiv`, and classical results including Legendre's Theorem (p-adic valuation of factorials in terms of base-p digit sums) and Kummer's Theorem (p-adic valuation of binomial coefficients in terms of carries in base-p addition).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `padicValNat p n` as the largest `k` where `p^k ∣ n`, foundational theorems connecting to multiplicity, and relationship to prime factorization via subpermutations |
| Basic.lean | Complete p-adic valuation theory for ℕ, ℤ, ℚ: arithmetic properties (multiplication, division, powers, inverses), ultrametric inequality, Legendre's Theorem for factorials, Kummer's Theorem for binomial coefficients, and efficient `maxPowDiv` implementation |

## Subdirectories

(none)

## Search Tags

p-adic padic valuation padicValNat padicValInt padicValRat multiplicity divisibility factorial binomial-coefficient legendres-theorem kummers-theorem ultrametric maxPowDiv prime-factorization digit-sum carries base-representation
