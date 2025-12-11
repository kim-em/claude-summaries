---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Sign
generated: 2025-12-11T10:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 2
subdirs_count: 0
---

# Sign

## Overview

This folder defines `SignType`, a three-valued type representing signs: negative (-1), zero (0), and positive (1). The type is equipped with a rich algebraic structure including `CommGroupWithZero`, `LinearOrder`, and `BoundedOrder` instances. The folder also provides the `sign` function that maps elements of ordered types to `SignType` based on their relationship to zero, along with extensive lemmas about sign behavior under arithmetic operations.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines the `SignType` inductive type with three constructors (`zero`, `neg`, `pos`), basic instances (`Zero`, `One`, `Neg`, `Mul`, `CommGroupWithZero`, `LinearOrder`, `BoundedOrder`, `HasDistribNeg`), the `cast` coercion to other types, the `sign : α →o SignType` function for ordered types, and foundational lemmas about sign comparisons |
| Basic.lean | Additional theorems requiring more imports: casting between `SignType`, integers, and other types; `sign_mul` showing sign is multiplicative; `signHom : α →*₀ SignType` as a monoid homomorphism; sign behavior with absolute value (`sign_mul_abs`, `abs_mul_sign`); sign of sums; and `exists_signed_sum` theorems decomposing sums into signed contributions |

## Subdirectories

(none)

## Search Tags

sign signtype sign-function positive negative zero trichotomy ordered-ring linear-order sign-homomorphism absolute-value
