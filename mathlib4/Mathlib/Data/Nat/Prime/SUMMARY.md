---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat/Prime
generated: 2025-12-11T22:15:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 7
subdirs_count: 0
---

# Prime

## Overview

The `Prime/` directory contains the foundational theory of prime numbers in mathlib4. It defines `Nat.Prime` as `Irreducible` for natural numbers (numbers >= 2 whose only divisors are 1 and themselves), provides the `minFac` function for computing the smallest prime factor, and develops key properties including divisibility, coprimality with primes, Euclid's theorem on infinitude of primes, and connections between `Nat.Prime` and the general algebraic `Prime` predicate. The directory also covers interactions with factorials, powers, and the integers.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `Nat.Prime` (defined as `Irreducible`), `minFac`/`minFacAux` (smallest prime factor), `Nat.Primes` subtype, decidability instances; key theorems `prime_def`, `prime_def_le_sqrt`, `prime_iff` (equivalence with `_root_.Prime`) |
| Basic.lean | Extended theory: `prime_mul_iff`, even/odd properties of primes, coprimality lemmas (`coprime_of_dvd'`, `coprime_primes`, `coprime_pow_primes`), `Prime.dvd_of_dvd_pow`, divisibility of prime powers (`dvd_prime_pow`) |
| Factorial.lean | Interaction with factorials: `Prime.dvd_factorial` (p divides n! iff p <= n), `coprime_factorial_iff`, `Prime.coprime_factorial_of_lt` |
| Infinite.lean | Euclid's theorem: `exists_infinite_primes` (for every n, exists prime p >= n), `not_bddAbove_setOf_prime` |
| Int.lean | Connection to integers: `prime_iff_prime_int` (Nat.Prime p iff Prime (p : Z)), `Prime.pow_inj` for prime powers, `Int.prime_two`, `Int.prime_three` |
| Nth.lean | Nth prime computations: `nth_prime_zero_eq_two`, `nth_prime_one_eq_three`, etc. (simp lemmas for first 5 primes) |
| Pow.lean | Powers of primes: `pow_minFac` (minFac of n^k equals minFac of n), `Prime.pow_minFac` |

## Subdirectories

(none)

## Search Tags

prime-numbers primality minFac smallest-prime-factor irreducible coprime divisibility Euclid infinitude-of-primes factorial prime-powers integers decidable nth-prime
