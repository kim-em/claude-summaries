---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/LocalRing
generated: 2026-02-01T10:15:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: preliminary
files_count: 7
subdirs_count: 3
---

# LocalRing

## Overview

The `LocalRing/` directory contains the theory of local rings - commutative rings with a unique maximal ideal. This includes the foundational definition (`IsLocalRing` predicate), characterization theorems, the maximal ideal construction, residue field theory, local ring homomorphisms (`IsLocalHom`), and results about modules over local rings. The theory connects to localization, flatness, Nakayama's lemma, and finite presentation.

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

- [x] `MaximalIdeal/` - Construction and properties of the unique maximal ideal in local rings
- [x] `ResidueField/` - Residue field k = R/m and its properties
- [ ] `RingHom/` - Local ring homomorphisms (IsLocalHom)

## Search Tags

local-ring maximal-ideal residue-field IsLocalRing IsLocalHom unique-maximal-ideal local-subring localization-at-prime Nakayama flat-module finite-presentation free-module tensor-product non-local-ring maximal-spectrum quotient-local-ring subring-local-ring
