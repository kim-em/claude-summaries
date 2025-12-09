---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat/Cast/Order
generated: 2025-12-09T11:30:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 3
subdirs_count: 0
---

# Order

## Overview

The `Order/` directory establishes order-theoretic properties of natural number casts in algebraic structures with ordering. It proves that `Nat.cast` is monotone and (under `CharZero`) strictly monotone, enabling comparison between natural numbers and their images in ordered semirings and fields. The directory provides comprehensive inequalities relating cast values to zero and one, handles division in ordered fields, and includes specialized lemmas for absolute values, min/max operations, and subtraction in canonically ordered structures.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core monotonicity and comparison theorems: `mono_cast` (monotone), `strictMono_cast` and `castOrderEmbedding` (under `CharZero`), bidirectional inequalities `cast_le`/`cast_lt`, positivity lemmas `cast_pos`/`cast_nonneg`, and `ofNat` variants for numeric literals |
| Ring.lean | Bundled ordered semiring instances: specialized versions of `cast_nonneg` and `cast_pos` for `IsOrderedRing`, `cast_min`/`cast_max` for linear orders, `cast_tsub` for truncated subtraction in canonically ordered structures, `abs_cast`, negative cast equalities, and auxiliary inequalities `mul_le_pow` and `two_mul_sq_add_one_le_two_pow_two_mul` |
| Field.lean | Ordered field division properties: `cast_div_le` showing natural division is always ≤ field division, inverse inequalities `cast_inv_le_one`, reciprocal lemmas `one_div_pos_of_nat`/`one_div_le_one_div`/`one_div_lt_one_div`, and subtraction-from-one bounds `one_sub_one_div_cast_nonneg`/`one_sub_one_div_cast_le_one` |

## Subdirectories

(none)

## Search Tags

nat-cast order monotone strict-monotone inequality comparison CharZero ordered-semiring ordered-field division inverse reciprocal absolute-value min-max truncated-subtraction
