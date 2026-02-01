---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/OreLocalization
generated: 2026-02-01T19:45:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 5
subdirs_count: 0
---

# OreLocalization

## Overview

The `OreLocalization/` directory contains the formalization of Ore localization for non-commutative rings. Ore localization generalizes the classical localization of commutative rings to settings where commutativity fails, allowing construction of fractions r /ₒ s for elements of a ring R with respect to an Ore set S (a multiplicative subset satisfying the Ore condition: for all r ∈ R and s ∈ S, there exist r', s' such that s' * r = r' * s). This construction is fundamental in non-commutative algebra and includes as special cases the construction of division rings from domains and fields of fractions from integral domains.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core construction of Ore localization for monoids with zero; proves MonoidWithZero, CommMonoidWithZero, and DistribMulAction instances; implements addition on Ore localizations via the Ore condition; establishes AddMonoid, AddCommMonoid, AddGroup, and AddCommGroup instances |
| OreSet.lean | Defines Ore sets for rings; provides `oreSetOfIsCancelMulZero` and `oreSetOfNoZeroDivisors` constructors showing cancellability implies the ore_right_cancel condition; characterizes when Ore sets exist via `nonempty_oreSet_iff` |
| Ring.lean | Module and ring structure on Ore localizations; proves Semiring, Ring, CommSemiring, CommRing instances; constructs DivisionRing and Field instances for localizations at non-zero divisors; provides universal property via `universalHom` lifting ring homomorphisms |
| NonZeroDivisors.lean | Specialization to Ore localization at non-zero divisors R⁰; proves nontriviality when localizing at left/right non-zero divisors; constructs multiplicative inverse satisfying 0⁻¹ = 0 and (r /ₒ s)⁻¹ = s /ₒ r; establishes GroupWithZero and CommGroupWithZero instances |
| Cardinality.lean | Cardinality results for Ore localizations of rings; proves #(R[S⁻¹]) = #R when S consists of left non-zero divisors, using injectivity of the numerator homomorphism |

## Subdirectories

(none)

## Search Tags

Ore-localization non-commutative localization fraction Ore-set Ore-condition left-Ore-set ring monoid-with-zero division-ring field-of-fractions non-zero-divisors universal-property semiring module algebra cardinality
