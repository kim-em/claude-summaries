---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Ring/Divisibility
generated: 2025-12-01T19:50:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Divisibility

## Overview

The `Divisibility/` directory contains the theory of divisibility in rings and semirings. It provides fundamental lemmas about the divisibility relation (`∣`) in various algebraic structures, from basic semigroups through rings and commutative rings. The directory is split into `Basic.lean` (minimal imports for use by tactics like `linarith`) and `Lemmas.lean` (additional results with heavier dependencies, including nilpotent element divisibility and scalar action interactions).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core divisibility lemmas with minimal imports: equivalences under multiplicative equivalences (`map_dvd_iff`), divisibility in distributive structures (`dvd_add`), interaction with negation (`dvd_neg`, `neg_dvd`), and divisibility in rings with addition/subtraction (`dvd_add_left`, `dvd_sub_comm`). Includes `Equiv.dvd` constructing an equivalence between a semigroup and elements divisible by a given element. |
| Lemmas.lean | Extended divisibility theory requiring heavier imports: divisibility under scalar multiplication (`dvd_smul_of_dvd`, `dvd_nsmul_of_dvd`, `dvd_zsmul_of_dvd`), nilpotent element divisibility for commuting elements (`Commute.pow_dvd_add_pow_of_pow_eq_zero_right` and variants), linear system divisibility (`dvd_mul_sub_mul_mul_left_of_dvd`), and absolute value interaction with associated elements (`associated_abs_left_iff`). |

## Subdirectories

(none)

## Search Tags

divisibility ring semiring dvd add-sub negation multiplicative-equivalence scalar-multiplication nilpotent commute associated absolute-value gcd linear-combination decomposition-monoid
