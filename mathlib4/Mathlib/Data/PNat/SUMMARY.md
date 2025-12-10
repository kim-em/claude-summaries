---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/PNat
generated: 2025-12-11T12:00:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 10
subdirs_count: 0
---

# PNat

## Overview

This folder develops `ℕ+` (PNat), the type of positive natural numbers (natural numbers strictly greater than zero). PNat is defined as a subtype `{ n : ℕ // 0 < n }` with efficient VM representation. The folder provides arithmetic operations (addition, multiplication, subtraction, division, modulo), algebraic instances (commutative monoid, ordered cancel monoid), primality predicates, GCD/LCM operations, prime factorization as multisets, an extended Euclidean algorithm, and interval computations. The design ensures that division and modulo always produce positive results by adjusting when the divisor evenly divides.

## Key Files

| File | Purpose |
|------|---------|
| Notation.lean | Defines `PNat` type as `{ n : ℕ // 0 < n }`, notation `ℕ+`, and coercion to `ℕ` |
| Defs.lean | Core definitions: `One`, `OfNat`, `natPred`, `succPNat`, `toPNat`, mod/div operations with positive-result semantics |
| Basic.lean | Algebraic instances (CommMonoid, CancelCommMonoid, OrderedCancelMonoid), arithmetic lemmas, induction principles (`recOn`, `strongInductionOn`), subtraction |
| Equiv.lean | Equivalence `Equiv.pnatEquivNat : ℕ+ ≃ ℕ` via `natPred`/`succPNat` |
| Order.lean | Order instances: `SuccOrder`, `SuccAddOrder`, `NoMaxOrder` for ℕ+ |
| Prime.lean | Primality: `PNat.Prime`, `gcd`, `lcm`, `Coprime` predicates and theorems; coercion from `Nat.Primes` to `ℕ+` |
| Factors.lean | Prime factorization: `PrimeMultiset` type, `factorMultiset : ℕ+ → PrimeMultiset`, bijection `factorMultisetEquiv : ℕ+ ≃ PrimeMultiset`, GCD/LCM as inf/sup on multisets |
| Xgcd.lean | Extended Euclidean algorithm for ℕ+: computes `(w, x, y, z, d)` such that `a = (w+x)d`, `b = (y+z)d`, `wz = xy + 1`; related to SL₂(ℕ) structure |
| Find.lean | `PNat.find`: smallest positive natural satisfying a decidable predicate (wraps `Nat.find`) |
| Interval.lean | Finite interval computations: `LocallyFiniteOrder` instance, cardinality of `Icc`, `Ico`, `Ioc`, `Ioo` intervals |

## Subdirectories

(none)

## Search Tags

pnat positive-natural-numbers natural-numbers arithmetic gcd lcm prime factorization multiset euclidean-algorithm coprime divisibility intervals locally-finite-order commutative-monoid
