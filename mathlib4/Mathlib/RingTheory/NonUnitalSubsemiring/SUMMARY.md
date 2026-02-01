---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/NonUnitalSubsemiring
generated: 2026-02-01T18:30:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 2
subdirs_count: 0
---

# NonUnitalSubsemiring

## Overview

This folder defines bundled non-unital subsemirings and their theory. A non-unital subsemiring of a non-unital semiring `R` is a subset that is both an additive submonoid (closed under 0 and +) and a multiplicative subsemigroup (closed under *), but without requiring a multiplicative identity. The two files establish the basic definitions and then the complete lattice structure along with homomorphism operations.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines the `NonUnitalSubsemiring` structure extending `AddSubmonoid` and `Subsemigroup`; the `NonUnitalSubsemiringClass` typeclass for set-like types; basic instances (`Top`, `Bot`, `Inf`); inherited semiring structures on subtype; `subtype` and `inclusion` ring homomorphisms; `codRestrict` for restricting codomain; `eqSlocus` for equalizer subsemirings |
| Basic.lean | Establishes the `CompleteLattice` structure on non-unital subsemirings; defines `map` and `comap` for images/preimages along ring homomorphisms with Galois connection; `srange` for the range of a ring homomorphism; `closure` for generating non-unital subsemirings from sets with induction principles; `center` and `centralizer` constructions; `prod` for product subsemirings; various monotonicity and directed union lemmas; `RingEquiv` constructions for isomorphisms between subsemirings |

## Subdirectories

(none)

## Search Tags

non-unital-subsemiring subsemiring additive-submonoid multiplicative-subsemigroup ring-homomorphism complete-lattice closure center centralizer map comap range product galois-connection
