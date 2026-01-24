---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Euclidean/Angle
generated: 2026-01-24T19:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: preliminary
files_count: 2
subdirs_count: 2
---

# Angle

## Overview

The `Angle/` directory formalizes angles in Euclidean geometry, providing both oriented and unoriented angle theories for real inner product spaces and Euclidean affine spaces. It covers angles between vectors, angles at points in affine spaces, and specialized results for angles in circles and spheres. The library includes classical results such as Thales' theorem (angle inscribed in semicircle is right), the inscribed angle theorem (central angle equals twice inscribed angle), cyclic quadrilateral properties, and the law of sines expressed via circumradius. It also provides angle bisector theory relating equidistance from affine subspaces to equal angles.

## Key Files

| File | Purpose |
|------|---------|
| Bisector.lean | Angle bisector properties: equidistance to affine subspaces iff equal angles to orthogonal projections, both for oriented and unoriented angles |
| Sphere.lean | Angles in circles and spheres: Thales' theorem, inscribed angle theorem (central angle = 2x inscribed), cyclic quadrilateral angle properties, tangent line characterization via right angle, law of sines via circumradius, explicit circumcenter/circumradius formulas |

## Subdirectories

- [ ] `Oriented/` - Oriented angles (angles with sign) in 2D: basic definitions using complex exponentials, rotations, right angle properties, affine geometry applications
- [ ] `Unoriented/` - Unoriented angles (unsigned) in arbitrary dimension: basic definitions via inner product, affine geometry, conformal maps, cross products, right angles, triangle inequality

## Search Tags

angle oriented-angle unoriented-angle inscribed-angle central-angle thales-theorem cyclic-quadrilateral circumradius circumcenter law-of-sines angle-bisector equidistance tangent-line right-angle cospherical concyclic
