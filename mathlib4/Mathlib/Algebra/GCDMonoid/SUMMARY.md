---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/GCDMonoid
generated: 2025-12-04T02:16:31Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# GCDMonoid

## Overview

The `GCDMonoid/` directory defines monoids with normalization functions, greatest common divisors (GCD), and least common multiples (LCM). It introduces three core algebraic structures: `NormalizationMonoid` (assigning canonical representatives to associate classes), `GCDMonoid` (monoids with GCD/LCM operations determined up to units), and `NormalizedGCDMonoid` (combining both with normalized GCD/LCM). The directory provides both the abstract typeclass definitions with comprehensive theory and concrete instances for fundamental types (ℕ, ℤ, PUnit) as well as operations lifted to multisets and finsets.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `NormalizationMonoid`, `GCDMonoid`, and `NormalizedGCDMonoid` typeclasses with `normalize` function, `normUnit` assignment, `gcd`/`lcm` operations, comprehensive GCD/LCM theory (commutativity, associativity, distributivity, divisibility), constructors (`gcdMonoidOfGCD`, `normalizedGCDMonoidOfGCD`, etc.), and connections to `Associates` (1318 lines) |
| Nat.lean | `NormalizedGCDMonoid` instances for ℕ and ℤ: proves `gcd`/`lcm` align with `Nat.gcd`/`Nat.lcm`, establishes normalization for ℤ via absolute value, defines `associatesIntEquivNat` equivalence mapping associate classes `{-n, n}` to `n : ℕ`, and proves associated elements in ℤ satisfy `a = b ∨ a = -b` |
| Multiset.lean | GCD and LCM operations for multisets via fold: defines `Multiset.gcd`/`Multiset.lcm` with divisibility characterizations (`a ∣ s.gcd ↔ ∀ b ∈ s, a ∣ b`), proves normalization and monotonicity, handles deduplication invariance, provides extraction lemma `extract_gcd` for factoring out common divisors |
| Finset.lean | GCD and LCM operations for finsets building on multiset theory: defines `Finset.gcd`/`Finset.lcm` with insert/union/image lemmas, divisibility characterizations, zero-detection, multiplicative extraction (`gcd_mul_left`), extraction with unit residue (`extract_gcd`), and division normalization (`gcd_div_eq_one`) |
| IntegrallyClosed.lean | Proves GCD domains are integrally closed: `GCDMonoid.toIsIntegrallyClosed` shows elements integral over `R` lie in `R` using `IsLocalization.surj_of_gcd_domain` to express fraction ring elements as coprime ratios, leveraging that GCD divides polynomial discriminants |
| PUnit.lean | Trivial `NormalizedGCDMonoid` instance for the one-element type `PUnit` where all operations return `unit` |

## Subdirectories

*(No subdirectories)*

## Search Tags

gcd-monoid lcm normalization-monoid normalized-gcd-monoid greatest-common-divisor least-common-multiple associate-classes canonical-representatives multiset finset integrally-closed nat int typeclass algebra divisibility
