---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Convex
generated: 2026-01-24T09:15:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 1
---

# Convex

## Overview

The `Convex/` directory contains formalized convex geometry results that work at a purely algebraic level without requiring topology, norms, or inner products. This complements the topological convexity theory in `Mathlib.Analysis.Convex` by providing foundational algebraic structures. The primary content is a comprehensive theory of convex cones, including bundled `ConvexCone` and `PointedCone` types, complete lattice structure on cones, correspondence between cones and ordered modules, dual cones via bilinear pairings, and tensor products of pointed cones (both minimal and maximal constructions).

## Key Files

| File | Purpose |
|------|---------|
| README.md | Documentation explaining the scope of this folder (convexity without norms/inner products) and listing covered topics (cones) |

## Subdirectories

- [x] `Cone/` - Algebraic theory of convex cones: bundled `ConvexCone` and `PointedCone` types, properties (pointed/blunt/flat/salient), complete lattice structure, maps between cones, duality via bilinear pairings, tensor products, and correspondence with ordered modules

## Search Tags

convex-geometry convex-sets cones convexity algebraic-convexity norm-free inner-product-free foundational-convexity convex-cones pointed-cones dual-cones tensor-products ordered-modules salient-cones generating-cones
