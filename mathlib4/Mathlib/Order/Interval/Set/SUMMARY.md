---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Interval/Set
generated: 2026-01-26T22:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 25
subdirs_count: 0
---

# Set

## Overview

The `Set/` directory provides the comprehensive implementation of intervals as infinite sets in Mathlib. Starting with core definitions (`Defs.lean`) and basic properties (`Basic.lean`), it covers all standard interval notations (`Icc`, `Ico`, `Ioc`, `Ioo`, `Ici`, `Iic`, `Ioi`, `Iio`) and the fundamental `OrdConnected` typeclass. The directory includes specialized modules for linear orders, monotone function behavior on intervals, images and preimages, projections onto intervals, disjointness properties, and interactions with various type constructors (`Fin`, `Pi`, `WithBot`, `WithTop`). It also provides unordered intervals (`uIcc`) that work regardless of endpoint ordering, making them suitable for applications like geometric bounding boxes.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core interval definitions (`Iio`, `Iic`, `Ioo`, `Ico`, `Icc`, `Ioc`, `Ici`, `Ioi`) and `OrdConnected` typeclass declaring that a set contains `Icc x y` whenever it contains both `x` and `y` |
| Basic.lean | Fundamental properties of set intervals: decidability instances, membership facts, inclusion relations, set operations (union/inter/diff), emptiness conditions, subsingleton characterizations; carefully curated monotonicity results avoiding exhaustive enumeration |
| OrdConnected.lean | Properties of order-connected sets: preservation under preimages of monotone/antitone functions, standard intervals are order-connected, images under order embeddings, dual operations |
| LinearOrder.lean | Interval properties specific to linear orders: complement relations (`(Iic a)ᶜ = Ioi a`), set difference formulas (`Ici a \ Ioi b = Icc a b`), trichotomy-based reasoning |
| UnorderedInterval.lean | Unordered intervals `uIcc a b = Icc (a ⊓ b) (a ⊔ b)` (notation `[[a, b]]`) that don't require `a ≤ b`; in products/pi-types gives bounding boxes; equivalent to `segment ℝ a b` for reals |
| Monotone.lean | How monotone/antitone functions map intervals to intervals (`MonotoneOn.mapsTo_Icc`, `AntitoneOn.mapsTo_Icc`, etc.); strict versions for open intervals |
| Image.lean | Images and preimages of intervals under monotone/antitone functions and order embeddings; used by monotone function theory |
| ProjIcc.lean | Projection maps `projIci`, `projIic`, `projIcc` that clamp values to closed intervals; extension operators `IccExtend`, `IciExtend`, `IicExtend` for extending functions defined on intervals to entire type |
| Disjoint.lean | Disjointness relations between intervals (e.g., `Iic a` and `Ioi b` are disjoint when `a ≤ b`); requires `Data.Set.Lattice` import, so separated from Basic.lean to avoid cycles |
| Fin.lean | Preimages and images of intervals under `Fin` operations (`Fin.val`, `Fin.cast`, `Fin.castSucc`, `Fin.succ`, `Fin.rev`, etc.) |
| Pi.lean | Intervals in pi-types/function spaces: `Ici x` in `Π i, α i` equals product of `Ici (x i)`; piecewise constructions preserve interval membership |
| WithBotTop.lean | Images and preimages of intervals under `some : α → WithTop α` and `some : α → WithBot α` embeddings |
| SuccPred.lean | Relations between intervals in successor/predecessor orders: `Ico (succ a) b = Ioo a b`, `Ioc a (pred b) = Ioo a b`, insertion lemmas for adjoining endpoints |
| OrderEmbedding.lean | How order embeddings preserve interval structure when their range is order-connected |
| OrderIso.lean | Order isomorphisms preserve all interval types; preimages and images interchange under duality |
| OrdConnectedComponent.lean | Order-connected components (maximal order-connected subsets containing a point); dual to topological connected components in ordered spaces |
| OrdConnectedLinear.lean | Order-connectedness characterizations specific to linear orders |
| SurjOn.lean | Surjectivity of monotone functions on intervals (e.g., monotone `f` on `Icc a b` is surjective onto `Icc (f a) (f b)` under continuity-like conditions) |
| Union.lean | Unions of families of intervals, particularly unions of nested intervals |
| Infinite.lean | Intervals containing infinitely many elements (typically in `SuccOrder` or `DenselyOrdered` contexts) |
| Limit.lean | Limit points and interval boundaries in successor/predecessor orders |
| Final.lean | Properties of intervals at final/maximal elements |
| InitialSeg.lean | Initial segments and their relation to intervals |
| IsoIoo.lean | Order isomorphisms between open intervals `Ioo a b` |
| SuccOrder.lean | Interval properties in types with successor structure |

## Subdirectories

(none)

## Search Tags

set-interval Icc Ico Ioc Ioo Ici Iic Ioi Iio ord-connected order-connected unordered-interval uIcc monotone antitone projection interval-image interval-preimage linear-order fin pi withbot withtop succ-pred order-embedding interval-properties disjoint-intervals bounding-box segment
