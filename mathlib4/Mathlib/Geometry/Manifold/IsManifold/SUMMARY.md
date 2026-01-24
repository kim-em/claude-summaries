---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Manifold/IsManifold
generated: 2026-01-24T21:15:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# IsManifold

## Overview

The `IsManifold/` directory contains the core definitions and properties for C^n manifolds in Mathlib. It defines the `IsManifold` typeclass (which packages a charted space with a structure groupoid ensuring C^n coordinate changes), the `ModelWithCorners` structure (which specifies how a model space H embeds in a normed vector space E), and extended charts (`extChartAt`) that map directly into E. The directory also formalizes the interior and boundary of manifolds with corners, including the `BoundarylessManifold` typeclass for manifolds without boundary.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `ModelWithCorners` (embedding of model space H into vector space E), `contDiffGroupoid` (groupoid of C^n transitions), `IsManifold` typeclass, `TangentSpace` and `TangentBundle` type synonyms, products of manifolds, boundaryless models |
| ExtChartAt.lean | Extended charts `extChartAt` mapping into E (not just H), their properties (continuity, neighborhoods), coordinate changes between extended charts, smoothness of coordinate changes, local compactness and metrizability theorems |
| InteriorBoundary.lean | Defines interior/boundary points of manifolds, `BoundarylessManifold` typeclass, proves manifolds decompose into interior ∪ boundary, computes interior/boundary of products, open subsets, and disjoint unions |

## Subdirectories

(none)

## Search Tags

ismanifold model-with-corners contdiff-groupoid extchartat extended-chart interior boundary boundaryless-manifold charted-space tangent-space tangent-bundle manifold-with-boundary manifold-with-corners coordinate-change smooth-manifold locally-compact finite-dimensional
