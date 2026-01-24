---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/AffineSpace/Simplex
generated: 2026-01-25T23:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Simplex

## Overview

The `Simplex/` subdirectory formalizes n-dimensional simplices in affine space and their geometric properties. A simplex is defined as a bundled structure containing `n + 1` affinely independent points. The directory provides comprehensive theory of simplex operations (faces, mapping, reindexing, restriction), interior and boundary points characterized by barycentric coordinates, and centroid-related theorems including Commandino's theorem in arbitrary dimensions. The `Basic.lean` file establishes fundamental simplex structures and operations, while `Centroid.lean` develops rich theory of centroids, face-opposite centroids, and medians with precise geometric relationships.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core simplex definitions: `Simplex k P n` structure with `n + 1` affinely independent points, `Triangle` abbreviation (2-simplex), face construction via subset selection, `faceOpposite` for facets excluding one vertex, mapping under injective affine maps, reindexing along equivalences, restriction to affine subspaces, and interior/closedInterior sets characterized by barycentric coordinate ranges |
| Centroid.lean | Simplex centroid theory: `centroid` as uniform average of vertices, `faceOppositeCentroid` for facet centroids, `median` as line through vertex and opposite-face centroid, geometric relations (centroid divides median in n:1 ratio), Commandino's theorem (`point_vsub_centroid_eq_smul_vsub`), median concurrency at centroid, preservation under maps/reindexing/restriction |

## Subdirectories

*(none)*

## Search Tags

simplex affine-geometry n-simplex triangle affine-independence face faceOpposite interior closedInterior barycentric-coordinates centroid faceOppositeCentroid median commandino-theorem affine-map reindex restrict convex-combination weighted-sum geometric-center facet simplex-operations
