---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Convex/Cone
generated: 2026-01-24T08:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Cone

## Overview

The `Cone/` directory contains the algebraic theory of convex cones operating at a general algebraic level without requiring topology, norms, or inner products. It defines bundled convex cones (`ConvexCone`), pointed cones (`PointedCone`), and various operations and properties including duality, tensor products, and the correspondence between cones and ordered modules. This is foundational work that complements the topological theory in `Mathlib.Analysis.Convex.Cone`.

## Key Files

| File | Purpose |
|------|---------|
| README.md | Documentation explaining this folder's scope (algebraic convex cone theory without topology/norms) and listing covered topics: convex cones, pointed cones, and dual cones |
| Basic.lean | Core definitions and fundamental theory: `ConvexCone` structure with closure under positive scalar multiplication and addition, complete lattice structure, maps/comaps between cones, pointed/blunt/flat/salient properties, correspondence with ordered modules, and cone hull constructions (707 lines) |
| Pointed.lean | Pointed cones defined as submodules over nonnegative scalars (`PointedCone`), providing a bundled version of `ConvexCone.Pointed` that allows using the module API, includes conversion between pointed cones and convex cones, span operations, and maps (240 lines) |
| Dual.lean | Algebraic dual cone construction for pointed cones with respect to a bilinear pairing: `PointedCone.dual p s` consists of all points `y` where `0 ≤ p x y` for all `x ∈ s`, includes double dual properties and interaction with span operations (106 lines) |
| TensorProduct.lean | Tensor products of pointed cones: minimal tensor product (conical combinations of elementary tensors) and maximal tensor product (dual of minimal product of dual cones), proves minimal ≤ maximal and commutativity properties (130 lines) |

## Subdirectories

No subdirectories.

## Search Tags

convex-cones pointed-cones convex-geometry algebraic-geometry cone-theory dual-cones tensor-products ordered-modules salient-cones flat-cones generating-cones reproducing-cones positive-cone convex-hull lattice-structure bilinear-pairing
