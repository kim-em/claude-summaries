---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat/GCD
generated: 2025-12-11T12:00:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 3
subdirs_count: 0
---

# GCD

## Overview

The `GCD/` directory contains lemmas about the greatest common divisor (`gcd`), least common multiple (`lcm`), and coprimality (`Coprime`) for natural numbers. The definitions themselves are provided in batteries; this directory builds additional theory on top. It includes basic properties, interactions with arithmetic operations (addition, multiplication, powers), division lemmas, and connections to primality and big operators (products over lists, multisets, and finsets).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core lemmas for `Nat.gcd`, `Nat.lcm`, and `Nat.Coprime`: uniqueness of gcd, coprimality with sums/differences/multiples, power interactions (`pow_sub_one_gcd_pow_sub_one`), divisibility through lcm, `Coprime.lcm_eq_mul`, `coprime_iff_isRelPrime`, and division/lcm relationships |
| BigOperators.lean | Coprimality lemmas for products: `coprime_list_prod_left_iff`, `coprime_multiset_prod_left_iff`, `coprime_prod_left_iff` for finsets, and fintype variants |
| Prime.lean | Interaction between primes and lcm: `Prime.dvd_or_dvd_of_dvd_lcm`, `Prime.dvd_lcm` iff characterization, `Prime.not_dvd_lcm` |

## Subdirectories

(none)

## Search Tags

gcd lcm coprime greatest-common-divisor least-common-multiple nat natural-numbers divisibility prime big-operators product
