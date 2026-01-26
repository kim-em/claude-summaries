---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Ideal/AssociatedPrime
generated: 2026-01-26T22:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# AssociatedPrime

## Overview

The `AssociatedPrime/` directory develops the theory of associated primes for modules over commutative rings. An associated prime of a module `M` is a prime ideal `I` that equals the annihilator of some non-zero element `x ∈ M`. This directory provides the basic definition, proves that finitely generated modules over Noetherian rings have only finitely many associated primes, and establishes the relationship between associated primes of a module and its localization. Key results include the characterization of zero divisors as the union of associated primes, and the existence of filtrations of modules by quotients of prime ideals.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `IsAssociatedPrime` and `associatedPrimes`; fundamental properties including behavior under exact sequences, products, and module equivalences; proof that union of associated primes equals zero divisors in Noetherian rings |
| Finiteness.lean | Proves finitely generated modules over Noetherian rings have finitely many associated primes; establishes existence of filtrations with quotients isomorphic to `R/p` for prime ideals; provides induction principle for finitely generated modules |
| Localization.lean | Relationship between `Ass(M)` and `Ass(S⁻¹M)` for localized modules; proves that localization of associated primes at a prime ideal gives associated primes of the localized module; shows minimal primes of annihilator are contained in associated primes |

## Subdirectories

None.

## Search Tags

associated-prime annihilator module-theory commutative-algebra Noetherian-ring prime-ideal zero-divisor localization filtration exact-sequence finitely-generated primary-decomposition
