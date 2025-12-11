---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Set/Lattice
generated: 2025-12-11T22:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 1
subdirs_count: 0
---

# Lattice

## Overview

The `Lattice/` subdirectory contains lemmas on the interaction between the indexed union/intersection operations (`iUnion`, `iInter`, `biUnion`, `biInter`) and function operations on sets (`image`, `preimage`, `image2`, `kernImage`). It also covers how set-theoretic function predicates (`MapsTo`, `InjOn`, `SurjOn`, `BijOn`) interact with indexed unions and intersections. This file extends the lattice structure on sets with lemmas about unions/intersections in products and sequences.

## Key Files

| File | Purpose |
|------|---------|
| Image.lean | Core lemmas connecting indexed unions/intersections with images and preimages: Galois connections for image/preimage and preimage/kernImage, lemmas for `MapsTo`/`InjOn`/`SurjOn`/`BijOn` with `iUnion`/`iInter`, image/preimage distribution over unions/intersections, product set operations with unions/intersections, and `image2`/`seq` interactions with indexed operations |

## Subdirectories

(none)

## Search Tags

set lattice union intersection iUnion iInter biUnion biInter image preimage image2 kernImage MapsTo InjOn SurjOn BijOn product seq Galois-connection indexed-union indexed-intersection
