---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/UniqueFactorizationDomain
generated: 2026-02-01T23:15:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: complete
files_count: 12
subdirs_count: 0
---

# UniqueFactorizationDomain

## Overview

The `UniqueFactorizationDomain/` directory contains the formalization of unique factorization domains (UFDs) and related structures in commutative algebra. This includes the core definitions of well-founded divisibility monoids (WfDvdMonoid) where strict divisibility is well-founded, and unique factorization monoids where irreducible elements are equivalent to prime elements. The directory provides both abstract theory (existence and uniqueness of factorizations, induction principles) and concrete computational tools (normalized factors, factorizations as finsupps, GCD constructions from factorizations). Key results include Kaplansky's criterion for factoriality, Euclid's lemma, and the construction of GCD structures from unique factorization.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: WfDvdMonoid (well-founded strict divisibility), UniqueFactorizationMonoid (irreducible iff prime), noncomputable factors function extracting multisets of prime factors |
| Basic.lean | Fundamental uniqueness theorems: prime_factors_unique (prime factorizations unique up to association), factors_unique for irreducibles, factors_mul/factors_pow laws, factors_prod (product of factors is associated to original element) |
| FactorSet.lean | FactorSet type representing elements as multisets of irreducible associates (unique by equality, not just association); provides complete lattice structure where inf is GCD and sup is LCM |
| NormalizedFactors.lean | normalizedFactors function producing normalized multisets via NormalizationMonoid; canonical choice of representatives for factorizations; prod_normalizedFactors establishes association |
| GCDMonoid.lean | Construction of GCDMonoid structure from UniqueFactorizationMonoid; toGCDMonoid and toNormalizedGCDMonoid provide GCD/LCM operations via inf/sup on Associates |
| Finite.lean | fintypeSubtypeDvd: elements of UFMs with finitely many units (e.g. ℤ, ideals in rings of integers) have finitely many divisors |
| Finsupp.lean | factorization function representing normalized factors as α →₀ ℕ (finitely supported functions); factorization_mul and factorization_pow laws for arithmetic |
| Ideal.lean | Relationship between UFDs and ideals: prime ideals in UFDs contain prime elements; equivalence between WfDvdMonoid and ascending chain condition on principal ideals in domains |
| Kaplansky.lean | Kaplansky's criterion: integral domain is UFD iff every nonzero prime ideal contains a prime element (iff_exists_prime_mem_of_isPrime) |
| Multiplicative.lean | Multiplicative induction and functions on UFDs: induction_on_coprime for properties preserved by coprime products; multiplicative_of_coprime for functions multiplicative on coprime elements extending to all elements |
| Multiplicity.lean | Connection between multiplicity theory and UFD factorizations: max_power_factor extracts maximal power of irreducible dividing an element; emultiplicity_eq_count_normalizedFactors relates multiplicity to factor counts |
| Nat.lean | Natural numbers as UFD: instUniqueFactorizationMonoid proves ℕ is a UFD using irreducible_iff_prime; factors_eq shows normalizedFactors matches primeFactorsList |

## Subdirectories

(none)

## Search Tags

unique-factorization-domain UFD unique-factorization-monoid well-founded-divisibility WfDvdMonoid irreducible prime factorization normalized-factors GCD-monoid greatest-common-divisor least-common-multiple factor-set multiplicity Kaplansky-criterion principal-ideal ascending-chain-condition Euclid-lemma coprime relatively-prime associates finsupp natural-numbers integral-domain commutative-algebra
