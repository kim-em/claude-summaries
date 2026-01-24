---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Euclidean/Angle/Oriented
generated: 2026-01-24T20:15:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Oriented

## Overview

The `Oriented/` directory formalizes oriented (signed) angles in 2-dimensional real inner product spaces and Euclidean affine spaces. Unlike unoriented angles (which are always in [0, pi]), oriented angles are elements of `Real.Angle` (the quotient of reals by 2*pi), allowing them to distinguish clockwise from counterclockwise rotations. The theory is built on complex-number representation via the Kahler form and covers basic definitions, rotations, affine geometry applications, right-angled triangle trigonometry, and orthogonal projections.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `Orientation.oangle` as the argument of the Kahler form; properties for zero/negation/scaling/addition of angles; relationship between oriented and unoriented angles; angle sign manipulation; pons asinorum; inner product = norm*norm*cos(oangle); linear independence criteria |
| Rotation.lean | Defines `Orientation.rotation` as a linear isometry rotating by an oriented angle; rotation composition equals angle addition; determinant is 1; inverse is rotation by negation; rotation by pi is negation; rotation by pi/2 is the right-angle rotation J; characterization of linear isometries with positive determinant |
| Affine.lean | Defines `EuclideanGeometry.oangle` (notation `∡`) for oriented angles at a point in affine spaces; properties for collinearity, same-side/opposite-side of lines, midpoints, cyclic quadrilaterals, signed angle sum in triangles; inscribed angle theorem for oriented angles |
| RightAngle.lean | Trigonometric identities (arccos, arcsin, arctan, sin, cos, tan) for oriented angles in right-angled triangles; versions for both vector addition/subtraction and affine point configurations; angle comparison lemmas for right-angled triangles |
| Projection.lean | Oriented angle properties involving orthogonal projections onto affine subspaces; proves that the oriented angle from a point to its projection to another point in the subspace is plus or minus pi/2 |

## Subdirectories

(none)

## Search Tags

oriented-angle oangle signed-angle rotation linear-isometry kahler-form complex-argument right-angle-rotation affine-angle inscribed-angle cyclic-quadrilateral same-side opposite-side collinear right-angled-triangle arccos arcsin arctan orthogonal-projection pons-asinorum two-dimensional
