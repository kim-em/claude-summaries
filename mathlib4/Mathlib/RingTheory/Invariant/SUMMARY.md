---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Invariant
generated: 2026-02-01T08:30:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 3
subdirs_count: 0
---

# Invariant

## Overview

This directory formalizes invariant extensions of rings under group actions, where `Algebra.IsInvariant A B G` states that every fixed point of `B` under the action of `G` lies in the image of `A`. The main application is algebraic number theory: given a Galois extension L/K of number fields with Galois group G, the rings of integers 𝓞K and 𝓞L satisfy this invariant property. Key results include integrality of invariant extensions, transitivity of Galois action on prime ideals lying over a given prime, surjectivity of stabilizer maps onto residue field automorphisms, and normality of residue field extensions. The theory is developed for both finite groups and profinite groups with continuous actions.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines `Algebra.IsInvariant A B G` predicate via the `isInvariant_iff` characterization: every element fixed by all group elements comes from the base ring |
| Basic.lean | Core theory for finite groups: proves invariant extensions are integral (`IsInvariant.isIntegral`), Galois group action transitivity on primes over a given prime (`exists_smul_of_under_eq`), stabilizer surjectivity onto residue field automorphisms (`stabilizerHom_surjective`), and normality of residue field extensions (`Ideal.Quotient.normal`) |
| Profinite.lean | Generalizes results to profinite groups with continuous actions on discrete rings: integrality (`isIntegral_of_profinite`), prime transitivity (`exists_smul_of_under_eq_of_profinite`), and stabilizer surjectivity (`stabilizerHom_surjective_of_profinite`) via cofiltered limits over open normal subgroups |

## Subdirectories

(none)

## Search Tags

invariant-ring group-action fixed-points Galois algebraic-number-theory ring-of-integers prime-ideal stabilizer residue-field Frobenius profinite-group integral-extension transitivity automorphism normal-extension AKLB
