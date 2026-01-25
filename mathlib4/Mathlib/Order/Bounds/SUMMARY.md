---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Bounds
generated: 2026-01-25T22:15:00Z
git_sha: ffb766c85c7ad82861131c2f10a0669884e4fd5f
git_branch: HEAD
status: complete
files_count: 5
subdirs_count: 0
---

# Bounds

## Overview

The `Bounds/` directory provides the foundational theory of upper and lower bounds for sets in ordered types. It defines the core predicates for boundedness (BddAbove, BddBelow), least/greatest elements (IsLeast, IsGreatest), least upper bounds and greatest lower bounds (IsLUB, IsGLB), and cofinality concepts. The directory also contains extensive theory about how these properties behave under monotone/antitone functions, images, products, unions, and order isomorphisms, establishing the fundamental infrastructure for analysis and lattice theory throughout Mathlib.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: upperBounds/lowerBounds sets, BddAbove/BddBelow predicates, IsLeast/IsGreatest for extremal elements, IsLUB/IsGLB for suprema/infima, IsCofinal/IsCofinalFor/IsCoinitialFor for directedness properties |
| Basic.lean | Comprehensive lemma library for bounds: membership characterizations, monotonicity results, conversions between concepts (IsLeast.isGLB, IsGreatest.isLUB), behavior under union/intersection/insert, bounds for specific sets (Ici, Iic, Iio, Ioi, Icc, Ico, Ioc, Ioo, singleton, pair, empty, univ), uniqueness theorems for partial orders |
| Image.lean | Behavior of bounds under monotone/antitone functions: MonotoneOn/Monotone preserve upper bounds and map IsLeast/IsGreatest/IsLUB/IsGLB, AntitoneOn/Antitone reverse bounds, StrictMono/StrictAnti iff characterizations, image2 theory for binary functions, product/Pi type bounds, range boundedness |
| Lattice.lean | Bounds over collections of sets: Galois connection between upperBounds and lowerBounds, upperBounds/lowerBounds of indexed unions (upperBounds (⋃ i, s i) = ⋂ i, upperBounds (s i)), IsLUB/IsGLB characterizations for unions via range |
| OrderIso.lean | Order isomorphism interaction with bounds: upperBounds_image equality (not just subset), IsLUB/IsGLB preserved exactly under order isomorphisms and their preimages, both for direct images (isLUB_image) and preimages (isLUB_preimage) |

## Subdirectories

(none)

## Search Tags

bounds upper-bounds lower-bounds supremum infimum least-upper-bound greatest-lower-bound bounded-above bounded-below isLUB isGLB isLeast isGreatest monotone antitone cofinal image order-isomorphism lattice-theory
