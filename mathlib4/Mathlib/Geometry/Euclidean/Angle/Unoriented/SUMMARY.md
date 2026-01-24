---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Euclidean/Angle/Unoriented
generated: 2026-01-24T20:15:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 0
---

# Unoriented

## Overview

This directory formalizes unoriented (unsigned) angles in real inner product spaces and Euclidean affine spaces. It provides the foundational definition of angle between vectors via arccos of the normalized inner product, extends this to angles at points in affine spaces, and develops a comprehensive theory including trigonometric relations (sine, cosine, tangent), right-angled triangle geometry (Pythagorean theorem and its converses), angle preservation under conformal maps, cross product norms, orthogonal projections, and the triangle inequality for angles. The theory works in arbitrary dimensions, unlike the oriented angle theory which is specific to 2D.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of unoriented angle between vectors as `arccos(inner(x,y) / (norm(x) * norm(y)))`; basic properties (commutativity, bounds 0 to pi, behavior with scaling/negation/zero); characterizations of angle 0, pi/2, pi in terms of inner products and collinearity; norm relations for angle 0 and pi |
| Affine.lean | Angles at points in Euclidean affine spaces using `angle` notation `angle p1 p2 p3`; invariance under translations, homotheties, isometries; vertical angles theorem; relations to `Sbtw`/`Wbtw` (strict/weak betweenness); collinearity characterizations via angle values; midpoint angle properties |
| RightAngle.lean | Pythagorean theorem (iff versions with angle = pi/2); angles in right triangles expressed via arccos/arcsin/arctan; trigonometric ratios (sin/cos/tan) as ratios of sides; versions for both vector addition and subtraction; comprehensive coverage of all side/angle relationships |
| Conformal.lean | Angle preservation under conformal maps: `IsConformalMap.preserves_angle` and `ConformalAt.preserves_angle` showing differentiable conformal maps preserve angles between vectors |
| CrossProduct.lean | Relates cross product norm to individual vector norms and angle: `norm(a cross b) = norm(a) * norm(b) * sin(angle a b)` for 3D vectors |
| Projection.lean | Angles involving orthogonal projections: the angle from a point through its orthogonal projection to any point in the subspace is pi/2 |
| TriangleInequality.lean | Triangle inequality for angles: `angle x z <= angle x y + angle y z`; equality characterization via collinearity or nonnegative span membership; helper lemmas about orthogonal decomposition and unit vector angles |

## Subdirectories

(none)

## Search Tags

unoriented-angle unsigned-angle angle-between-vectors inner-product arccos pythagorean-theorem right-angle right-triangle trigonometric-ratios sine cosine tangent conformal-map angle-preservation cross-product triangle-inequality collinear betweenness affine-angle orthogonal-projection
