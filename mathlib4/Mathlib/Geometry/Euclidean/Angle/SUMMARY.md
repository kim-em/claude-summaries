---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Euclidean/Angle
generated: 2026-01-24T20:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 2
---

# Angle

## Overview

The `Angle/` directory provides a comprehensive formalization of angles in Euclidean geometry, supporting both oriented (signed) and unoriented (unsigned) angle theories. The library is organized around two complementary approaches: **unoriented angles** work in arbitrary-dimensional real inner product spaces using arccos of normalized inner products, while **oriented angles** are specific to 2D and use complex exponentials via the Kahler form to distinguish clockwise from counterclockwise rotations.

The unoriented theory (`Unoriented/`) provides foundational definitions and results including the Pythagorean theorem and its converses, trigonometric ratios in right triangles, angle preservation under conformal maps, cross product norms in 3D, the triangle inequality for angles, and orthogonal projection properties.

The oriented theory (`Oriented/`) builds on 2D structure to define rotations as linear isometries, prove the inscribed angle theorem for oriented angles, relate angles to collinearity and same-side/opposite-side properties, and provide comprehensive right-triangle trigonometry.

At this level, two files integrate these theories: `Sphere.lean` proves classical circle geometry results (Thales' theorem, inscribed angle theorem, cyclic quadrilateral properties, law of sines via circumradius), while `Bisector.lean` connects angle bisectors to equidistance from affine subspaces via orthogonal projections.

## Key Files

| File | Purpose |
|------|---------|
| Bisector.lean | Angle bisector characterization: a point is equidistant from two affine subspaces iff the (unoriented or oriented) angles from that point to its orthogonal projections onto the subspaces are equal |
| Sphere.lean | Circle and sphere angle geometry: Thales' theorem (angle in semicircle is right), inscribed angle theorem (central angle = 2x inscribed), cyclic quadrilateral theorems, tangent line characterization via right angle, law of sines relating side length to circumradius, explicit circumcenter/circumradius formulas via angles |

## Subdirectories

- [x] `Oriented/` - Oriented (signed) angles in 2D using complex exponentials: rotations, affine geometry, right-triangle trigonometry, orthogonal projections
- [x] `Unoriented/` - Unoriented (unsigned) angles in arbitrary dimension: Pythagorean theorem, trigonometric ratios, conformal maps, cross products, triangle inequality

## Search Tags

angle oriented-angle unoriented-angle oangle signed-angle unsigned-angle inner-product arccos inscribed-angle central-angle thales-theorem cyclic-quadrilateral cospherical concyclic circumradius circumcenter law-of-sines angle-bisector equidistance tangent-line right-angle pythagorean-theorem trigonometry rotation conformal-map cross-product triangle-inequality orthogonal-projection
