---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat/Factorization
generated: 2025-12-11T09:15:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 6
subdirs_count: 0
---

# Factorization

## Overview

The `Factorization/` directory provides the core theory of prime factorizations for natural numbers in mathlib4. It defines `n.factorization` as a finitely-supported function `ℕ →₀ ℕ` mapping each prime `p` to its multiplicity in `n` (using p-adic valuations). This representation enables algebraic manipulation of factorizations and establishes the equivalence between `ℕ+` and prime-power finitely-supported functions. The directory also provides specialized induction principles based on prime factorizations, LCM decomposition lemmas, prime power characterizations, and floor/ceiling root operations adjoint to exponentiation in the divisibility order.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `n.factorization` as `ℕ →₀ ℕ` mapping primes to multiplicities; `ordProj[p] n` (largest power of p dividing n) and `ordCompl[p] n` (complementary part); `factorizationLCMLeft`/`Right` for LCM decomposition; basic lemmas on zero/one, products, powers, and coprimality |
| Basic.lean | Extended factorization theory: divisibility characterizations via factorization ordering; `ordProj`/`ordCompl` properties; factorization of gcd/lcm; Icc characterizations of prime power divisors; lemmas on coprime factors; `prod_pow_prime_padicValNat` and unique power extraction |
| Induction.lean | Prime factorization induction principles: `recOnPrimePow`, `recOnPosPrimePosCoprime`, `recOnPrimeCoprime`, `recOnMul`, `induction_on_primes`, `prime_composite_induction`; evaluation of multiplicative functions via factorization |
| LCM.lean | Properties of `factorizationLCMLeft`/`Right`: positivity, coprimality, divisibility into a and b, product equals lcm; split from Basic.lean to reduce imports |
| PrimePow.lean | Prime power characterizations via factorization: `IsPrimePow` iff `minFac^factorization = n`, iff single-element factorization, iff unique prime divisor; `Nat.Primes.prodNatEquiv` between `Primes × ℕ` and prime powers; coprime prime power divisibility; prime power extraction from `p^m = a^n` |
| Root.lean | Floor and ceiling roots: `floorRoot n a` and `ceilRoot n a` divide p-adic valuations by n (rounding down/up); Galois connections `a^n ∣ b ↔ a ∣ floorRoot n b` and `a ∣ b^n ↔ ceilRoot n a ∣ b`; right/left adjoints to `a ↦ a^n` in divisibility order |

## Subdirectories

(none)

## Search Tags

factorization prime-factorization multiplicity p-adic-valuation ordProj ordCompl prime-power IsPrimePow floorRoot ceilRoot induction multiplicative-function gcd lcm divisibility natural-numbers number-theory
