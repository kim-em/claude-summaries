---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/LocalRing
generated: 2026-02-01T19:50:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 7
subdirs_count: 3
---

# LocalRing

## Overview

The `LocalRing/` directory provides a comprehensive theory of local rings - commutative rings characterized by having a unique maximal ideal. The foundational `IsLocalRing` predicate is defined via the property that for any `a + b = 1`, either `a` or `b` is a unit. The theory is developed across three main areas: the maximal ideal (constructed as the set of non-units, proven unique), the residue field (quotient R/m and the more general κ(p) for prime ideals, with fiber theory for scheme morphisms), and local ring homomorphisms (`IsLocalHom` - those that reflect units). Supporting results cover modules over local rings (Nakayama's lemma, freeness of finitely presented flat modules), non-local rings (products, nontrivial maximal spectrum), quotients, and subrings.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `IsLocalRing` as a predicate: for any `a + b = 1`, either `a` or `b` is a unit |
| Basic.lean | Basic properties of local rings: alternative characterizations via unique maximal ideal, unique nonzero prime, closure under surjective homomorphisms; proves fields are local rings |
| LocalSubring.lean | `LocalSubring` structure for local subrings of fields with domination ordering; localization at primes as local subrings |
| Module.lean | Finite modules over local rings: Nakayama-style vanishing criteria, freeness conditions for finitely presented flat modules, tensor product characterizations |
| NonLocalRing.lean | Non-local ring characterizations: product rings are non-local, equivalence with nontrivial maximal spectrum, surjections onto products of fields |
| Quotient.lean | Quotients of local rings: spanning conditions lift through quotients, dimension equality for free modules, basis construction, power of maximal ideal conditions |
| Subring.lean | Inheritance of locality: subrings of local rings are local if elements are either units or zero divisors |

## Subdirectories

- [x] `MaximalIdeal/` - Construction of maximal ideal as non-units, uniqueness proof, Jacobson radical equality, field characterization
- [x] `ResidueField/` - Residue field k = R/m, κ(p) for primes, fiber theory (κ(p) ⊗ S), separability/algebraicity instances, polynomial applications
- [x] `RingHom/` - Local ring homomorphisms (IsLocalHom): unit reflection, TFAE characterization via maximal ideals, surjective hom results

## Search Tags

local-ring maximal-ideal residue-field IsLocalRing IsLocalHom unique-maximal-ideal local-subring localization-at-prime Nakayama flat-module finite-presentation free-module tensor-product non-local-ring maximal-spectrum quotient-local-ring subring-local-ring jacobson-radical fiber PrimeSpectrum separable algebraic polynomial ResidueField
