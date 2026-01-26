---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Ideal/MinimalPrime
generated: 2026-01-26T21:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# MinimalPrime

## Overview

The `MinimalPrime/` subdirectory develops the theory of minimal prime ideals over a given ideal. A minimal prime over an ideal `I` is a prime ideal containing `I` that is minimal with respect to this property. The directory provides the fundamental definition `I.minimalPrimes` as the set of minimal primes over `I`, proves existence and uniqueness results, establishes connections with radicals (the intersection of minimal primes equals the radical), and extends the theory to work with ring homomorphisms, localizations, and quotients. Finiteness results for Noetherian rings are also included.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `Ideal.minimalPrimes` and `minimalPrimes R`; existence theorems; proves intersection of minimal primes equals radical; handles minimal primes in quotients and extensions |
| Localization.lean | Minimal primes and localization theory: proves minimal primes over `f⁻¹I` are preimages of minimal primes over `I`; characterizes minimal primes via quotients; localization functoriality results |
| Noetherian.lean | Finiteness of minimal primes in Noetherian rings using a maximal counterexample argument |

## Subdirectories

*(none)*

## Search Tags

minimal-prime prime-ideal ring-theory commutative-algebra radical localization quotient Noetherian finiteness Zorn-lemma chain-condition minimal-element comap preimage algebraMap integral-extension lie-over going-up
