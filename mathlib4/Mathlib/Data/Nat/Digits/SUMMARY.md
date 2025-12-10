---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat/Digits
generated: 2025-12-11T10:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 3
subdirs_count: 0
---

# Digits

## Overview

The `Digits/` directory provides a comprehensive API for extracting and manipulating the digits of natural numbers in arbitrary bases. It defines `Nat.digits b n` which returns the little-endian list of digits of `n` in base `b`, and `Nat.ofDigits b L` which reconstructs a number from its digit list. The directory includes classical divisibility tests (divisibility by 3, 9, and 11 based on digit sums and alternating sums), modular arithmetic properties of digit representations, and bounds on the length of `Nat.toDigits` from core Lean. This completes Theorem #85 from Freek's 100 theorems list.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `digits`, `digitsAux`, `ofDigits`, and fundamental properties including `ofDigits_digits` (roundtrip), digit bounds (`digits_lt_base`), base conversions, and length bounds for `Nat.toDigits`/`repr` |
| Lemmas.lean | Advanced lemmas: `digits_len` relating length to logarithm, `ofDigits_eq_sum_mapIdx`, binary digit equivalence (`digits_two_eq_bits`), modular arithmetic properties (`ofDigits_modEq`, `zmodeq_ofDigits_digits`), and explicit digit computation (`getD_digits`) |
| Div.lean | Divisibility tests based on digits: divisibility by 3 (`three_dvd_iff`) and 9 via digit sums, divisibility by 11 via alternating sums, and a theorem that palindromic numbers with even digit length are divisible by 11 |

## Subdirectories

*(none)*

## Search Tags

digits base-representation ofDigits little-endian divisibility-test mod-3 mod-9 mod-11 digit-sum alternating-sum palindrome binary toDigits repr number-theory freek-100
