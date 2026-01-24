---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Euclidean
generated: 2026-01-24T06:15:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: preliminary
files_count: 12
subdirs_count: 3
---

# Euclidean

## Overview

The `Euclidean/` directory formalizes Euclidean geometry in real inner product spaces and Euclidean affine spaces. It builds on the foundation of normed add-commutative groups with inner products and normed add-torsors, defining geometric constructs like simplices, circumcenters, incenters, altitudes, and various triangle properties. The library covers classical Euclidean geometry topics including the law of cosines, law of sines, triangle congruence and similarity criteria (SSS, SAS, ASA, AAS), Monge points, orthogonal projections, perpendicular bisectors, and geometric inversion. It also includes specialized theories for angles (both oriented and unoriented), spheres, and circle geometry.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Foundation for Euclidean affine spaces: inner products of weighted vector subtraction, distances via affine combinations, quadratic distance formulas, and two-circle intersection theorems |
| Simplex.lean | Properties of simplices in Euclidean spaces: acute-angled simplices, equilateral simplex angles (π/3), distances from vertices to centroids and face opposite centroids |
| Circumcenter.lean | Circumsphere, circumcenter, and circumradius of simplices: existence and uniqueness proofs, equidistance properties, cospherical point theorems |
| Incenter.lean | Inspheres and exspheres of simplices: incenter, inradius, excenter, exradius definitions, touchpoints with faces, trilinear coordinates |
| Altitude.lean | Altitudes and altitude feet of simplices: orthogonal projection onto opposite faces, height of a simplex vertex |
| MongePoint.lean | Monge point (n-dimensional orthocenter generalization): position on Euler line, Monge planes, orthocentric systems for triangles |
| Triangle.lean | Triangle geometry: law of cosines, law of sines, pons asinorum, sum of angles equals π, distance and angle relationships |
| Congruence.lean | Triangle congruence criteria: SSS, SAS, ASA, AAS congruence theorems using the Congruent typeclass |
| Similarity.lean | Triangle similarity criteria: AA similarity, SAS similarity using proportional sides |
| Projection.lean | Orthogonal projection onto affine subspaces and reflection in affine subspaces |
| PerpBisector.lean | Perpendicular bisector of a segment: characterization via equidistance from endpoints |
| SignedDist.lean | Signed distance between points in a direction, signed distance to affine subspaces, trilinear coordinates |

## Subdirectories

- [x] `Angle/` - Angles in Euclidean spaces: oriented and unoriented angles between vectors, angle bisectors, angles inscribed in circles
- [x] `Inversion/` - Geometric inversion (circle inversion): basic properties, calculus of inversion, images of hyperplanes
- [ ] `Sphere/` - Sphere geometry: basic definitions, orthogonal radius, power of a point, Ptolemy's theorem, second intersection point, tangent lines

## Search Tags

euclidean-geometry inner-product-space affine-space simplex circumcenter circumradius incenter inradius excenter altitude monge-point orthocenter euler-line triangle law-of-cosines law-of-sines congruence SSS SAS ASA AAS similarity perpendicular-bisector orthogonal-projection reflection signed-distance trilinear-coordinates cospherical
