---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/LocalRing/RingHom
generated: 2026-02-01T19:45:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 1
subdirs_count: 0
---

# RingHom

## Overview

The `RingHom/` directory contains the theory of local ring homomorphisms (`IsLocalHom`). A ring homomorphism is local if it reflects units: whenever the image of an element is a unit, the element itself must be a unit. This file establishes the fundamental properties of local ring homomorphisms, including composition closure, the TFAE characterization relating local homomorphisms to maximal ideal behavior, and the important result that surjective homomorphisms from local rings preserve locality.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory of `IsLocalHom`: identity is local, composition of local homs is local, TFAE characterization (image of maximal ideal contained in maximal ideal, comap of maximal ideal equals maximal ideal), surjective local homs transfer locality, division ring homs are automatically local |

## Subdirectories

*(none)*

## Search Tags

IsLocalHom local-ring-homomorphism local-hom maximal-ideal-map comap-maximal-ideal surjective-local-hom division-ring-hom RingEquiv-isLocalRing units-map-surjective reflect-units
