---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Euclidean
generated: 2026-01-24T22:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 12
subdirs_count: 3
---

# Euclidean

## Overview

The `Euclidean/` directory provides a comprehensive formalization of Euclidean geometry in real inner product spaces and Euclidean affine spaces. The library builds on normed add-commutative groups with inner products and normed add-torsors to develop both classical synthetic geometry and coordinate-based approaches.

**Simplex and polytope theory**: Simplices in Euclidean spaces have rich structure including circumspheres (circumcenter, circumradius), inspheres (incenter, inradius), exspheres (excenter, exradius), altitudes, and Monge points (the n-dimensional generalization of the orthocenter). The library proves existence and uniqueness of circumcenters, the Euler line relationship for Monge points, and orthocentric system properties.

**Triangle geometry**: Classical results include the law of cosines, law of sines, pons asinorum, the sum of angles equaling π, and comprehensive congruence (SSS, SAS, ASA, AAS) and similarity (AA, SAS) criteria via the `Congruent` typeclass.

**Angle theory**: Both oriented (signed, 2D-specific using complex exponentials) and unoriented (unsigned, arbitrary-dimension using arccos) angles are formalized. This supports the Pythagorean theorem, inscribed angle theorem, Thales' theorem, cyclic quadrilateral theorems, and angle bisector characterizations.

**Sphere geometry**: The `Sphere` structure bundles center and radius, with theories for cospherical/concyclic points, tangent lines and spaces, power of a point, intersecting chords/secants theorems (Freek No. 55), Ptolemy's theorem (Freek No. 95), and second intersection points.

**Geometric inversion**: Circle/sphere inversion is formalized as an involution with distance formulas, calculus properties (differentiability, smoothness), and the key result that spheres through the center map to hyperplanes.

**Projections and distances**: Orthogonal projection onto affine subspaces, reflection in affine subspaces, perpendicular bisectors via equidistance characterization, and signed distances with trilinear coordinates.

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

- [x] `Angle/` - Angles in Euclidean spaces: both oriented (signed, 2D) and unoriented (unsigned, arbitrary dimension) angle theories, inscribed angle theorem, Thales' theorem, cyclic quadrilaterals, angle bisectors, Pythagorean theorem
- [x] `Inversion/` - Geometric inversion: involutivity, distance formulas, Ptolemy's inequality, calculus (derivatives, smoothness), images of spheres and hyperplanes
- [x] `Sphere/` - Sphere geometry: cospherical/concyclic points, power of a point, intersecting chords/secants theorems (Freek No. 55), Ptolemy's theorem (Freek No. 95), tangent lines/spaces, second intersection points

## Search Tags

euclidean-geometry inner-product-space affine-space simplex circumcenter circumradius incenter inradius excenter exradius altitude monge-point orthocenter euler-line triangle law-of-cosines law-of-sines pons-asinorum congruence SSS SAS ASA AAS similarity perpendicular-bisector orthogonal-projection reflection signed-distance trilinear-coordinates cospherical concyclic angle oriented-angle unoriented-angle inscribed-angle thales-theorem cyclic-quadrilateral pythagorean-theorem inversion circle-inversion ptolemy freek-55 freek-95 sphere tangent power-of-point intersecting-chords
