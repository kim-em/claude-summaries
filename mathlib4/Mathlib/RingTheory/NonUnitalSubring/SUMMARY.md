---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/NonUnitalSubring
generated: 2026-02-01T10:15:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 2
subdirs_count: 0
---

# NonUnitalSubring

## Overview

This folder defines non-unital subrings ("rngs" - rings without identity) and their properties in Mathlib. A `NonUnitalSubring R` is a subset of a non-unital ring `R` that is closed under addition, negation, multiplication, and contains zero (but not necessarily a multiplicative identity). The implementation builds on `NonUnitalSubsemiring` combined with `AddSubgroup` structure.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `NonUnitalSubringClass` typeclass, `NonUnitalSubring` structure bundling `NonUnitalSubsemiring` with `AddSubgroup`, membership lemmas, `subtype` homomorphism, inherited ring instances, and the `inclusion` homomorphism for subring inclusions |
| Basic.lean | Extended theory: complete lattice structure on non-unital subrings, `center` definition (elements commuting with everything), `closure` construction with Galois insertion, `comap`/`map` for pushforward/pullback along homomorphisms, `prod` for product subrings, `range` and `eqLocus` for homomorphisms, and various induction principles |

## Subdirectories

*(none)*

## Search Tags

non-unital-subring rng subring-without-identity NonUnitalSubring NonUnitalSubringClass closure center comap map lattice galois-insertion ring-homomorphism subsemigroup additive-subgroup complete-lattice
