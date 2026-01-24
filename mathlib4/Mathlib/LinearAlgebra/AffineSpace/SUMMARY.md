---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/AffineSpace
generated: 2026-01-25T23:05:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 17
subdirs_count: 2
---

# AffineSpace

## Overview

The `AffineSpace/` directory formalizes affine spaces and affine geometry in mathlib4, providing a comprehensive framework from foundational definitions through geometric applications. An affine space is defined as notation for `AddTorsor V P`, capturing the structure where a vector space `V` acts freely and transitively on a point space `P`. The directory develops the complete theory including affine maps (structure-preserving transformations), affine equivalences (affine isomorphisms), affine combinations (weighted sums with weight constraints), affine independence (geometric independence), and affine bases with barycentric coordinates. Specialized constructions cover centroids, midpoints, slopes, and classical geometric theorems like Ceva's theorem. The `AffineSubspace/` subdirectory provides the core theory of affine subspaces as subsets closed under affine combinations, with `affineSpan`, `vectorSpan`, lattice structure, and parallel subspace theory. The `Simplex/` subdirectory formalizes n-dimensional simplices as bundled affinely independent point families, developing comprehensive simplex operations, interior/boundary characterizations via barycentric coordinates, and centroid theorems including Commandino's theorem in arbitrary dimensions. This foundational material supports both abstract affine geometry and concrete applications across finite and infinite-dimensional spaces.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core affine space definition: introduces `AffineSpace V P` notation for `AddTorsor V P`, providing the fundamental structure where vector space `V` acts freely and transitively on point space `P` |
| AffineMap.lean | Affine maps `P1 →ᵃ[k] P2`: structure-preserving maps between affine spaces with underlying function `toFun : P1 → P2` and linear part `linear : V1 →ₗ[k] V2` satisfying `toFun (v +ᵥ p) = linear v +ᵥ toFun p`, includes constructors (const, id, lineMap, homothety) |
| AffineEquiv.lean | Affine equivalences `P1 ≃ᵃ[k] P2`: invertible affine maps where both forward and inverse are affine, built from `Equiv` for points and `LinearEquiv` for vectors, includes group structure on `AffineEquiv k P P` |
| Combination.lean | Affine combinations of points: `weightedVSubOfPoint` (weighted vector combination from base point), `weightedVSub` (base-independent when weights sum to 0), `affineCombination` (point result when weights sum to 1), defines affine span and convex hulls |
| Independent.lean | Affine independence `AffineIndependent k p`: family of points where no nontrivial weighted subtraction (with weight sum 0) yields zero vector, equivalent to linear independence of differences from base point and uniqueness of affine combination weights |
| Basis.lean | Affine bases and barycentric coordinates: `AffineBasis ι k P` representing affine-independent spanning families, `coord : P →ᵃ[k] k` giving barycentric coordinate maps, defines `fintypeAffineCoords` and `finsuppAffineCoords` as spaces where coordinates sum to 1 |
| Centroid.lean | Centroids of finite point sets: `centroidWeights` (constant weight `(#s)⁻¹` for each point), `centroid` (affine combination with centroid weights), sum of weights equals 1 when cardinality is nonzero |
| Midpoint.lean | Midpoint construction `midpoint R x y`: defined as `lineMap x y (⅟2)` for rings with invertible 2, proves linearity in both arguments and characterization `x + y = z + z` iff `z = midpoint R x y` |
| Slope.lean | Slope of functions into affine spaces: `slope f a b = (b - a)⁻¹ • (f b -ᵥ f a)` measuring rate of change on intervals, foundation for mean value theorems and convexity analysis |
| Ordered.lean | Affine geometry in ordered modules: monotonicity theorems for `lineMap` and `slope` when module has compatible order structure, links convexity to slope monotonicity |
| FiniteDimensional.lean | Finite-dimensional affine subspaces: proves `vectorSpan` and `affineSpan` of finite sets have finite-dimensional directions, defines `Collinear` (sets spanning subspace of dimension ≤ 1) |
| Matrix.lean | Matrix representations of barycentric coordinates: `AffineBasis.toMatrix q` giving matrix whose rows are barycentric coordinates of points `q` with respect to basis, proves affine independence from matrix invertibility |
| Ceva.lean | Ceva's theorem: proves existence of affine combinations satisfying proportionality conditions for concurrent cevians in simplices |
| Pointwise.lean | Pointwise additive action on affine subspaces: `v +ᵥ s` translates affine subspace `s` by vector `v` via `AffineEquiv.constVAdd` |
| Restrict.lean | Restriction of affine maps to affine subspaces with coercion and composition properties |
| MidpointZero.lean | Midpoint properties when one argument is zero in the additive structure |
| ContinuousAffineEquiv.lean | Import aggregator for continuous affine equivalences (deferred to topology files) |

## Subdirectories

- [x] `AffineSubspace/` - Core theory of affine subspaces as subsets closed under affine combinations, with affineSpan, vectorSpan, direction, complete lattice structure, map/comap operations, and parallel subspace relations
- [x] `Simplex/` - n-dimensional simplices as bundled affinely independent point families, with face operations, interior/boundary characterizations via barycentric coordinates, centroid theory, and Commandino's theorem

## Search Tags

affine-space affine-map affine-equiv add-torsor affine-combinations barycentric-coordinates affine-independence affine-basis centroid midpoint slope collinear lineMap weightedVSub vectorSpan affineSpan finite-dimensional ceva-theorem ordered-affine pointwise-action affine-subspace simplex
