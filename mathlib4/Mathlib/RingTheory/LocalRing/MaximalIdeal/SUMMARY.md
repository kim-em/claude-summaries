---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/LocalRing/MaximalIdeal
generated: 2026-02-01T20:30:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 2
subdirs_count: 0
---

# MaximalIdeal

## Overview

The `MaximalIdeal/` directory defines and develops the theory of the maximal ideal in local rings. In a local ring, the maximal ideal is defined as the set of all non-units, and this directory proves it is indeed the unique maximal ideal. Key results include the singleton nature of the maximal spectrum, the relationship between the maximal ideal and the Jacobson radical, characterization of when a local ring is a field (iff maximal ideal is trivial), and inheritance of locality to subsemirings/subrings when units lift.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines `IsLocalRing.maximalIdeal R` as the ideal of non-units; proves it is an ideal using `nonunits_add` and `mul_mem_nonunits_right` |
| Basic.lean | Proves the maximal ideal is maximal and unique; establishes `Unique (MaximalSpectrum R)` for local rings; proves Jacobson radical equals maximal ideal; characterizes fields as local rings with trivial maximal ideal; provides `Subsemiring.isLocalRing_of_unit` and `Subring.isLocalRing_of_unit` for inheriting locality |

## Subdirectories

(none)

## Search Tags

maximal-ideal local-ring IsLocalRing maximalIdeal nonunits unique-maximal-ideal MaximalSpectrum jacobson-radical isField Subsemiring Subring locality-inheritance ker-eq-maximalIdeal
