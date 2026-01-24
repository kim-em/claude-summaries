---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Euclidean/Sphere
generated: 2026-01-24T07:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# Sphere

## Overview

The `Sphere/` directory formalizes sphere geometry in Euclidean affine spaces. It defines the `Sphere` structure (bundling center and radius), cospherical and concyclic point sets, and develops a comprehensive theory of sphere-line and sphere-sphere interactions. Key results include classical theorems on intersecting chords and secants, Ptolemy's theorem (Freek No. 95), power of a point, tangent lines and tangent spaces, and the second intersection point of a line through a sphere point.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core sphere definitions: `Sphere` structure, membership, `Cospherical` (equidistant from a point), `Concyclic` (cospherical and coplanar), diameter (`IsDiameter`, `ofDiameter`), two-sphere intersection theorems, and affine independence of cospherical points |
| OrthRadius.lean | Defines `orthRadius`: the affine subspace orthogonal to the radius vector at a point (tangent space when point is on sphere, polar of inversion otherwise); properties of parallel orthRadius subspaces |
| Power.lean | Power of a point (`Sphere.power`): distance² - radius², Intersecting Chords Theorem (Freek No. 55), Intersecting Secants Theorem, Tangent-Secant Theorem, characterization of points inside/outside/on sphere via power sign |
| Ptolemy.lean | Ptolemy's Theorem (Freek No. 95): for cyclic quadrilateral with diagonals meeting at P, proves `dist a b * dist c d + dist b c * dist d a = dist a c * dist b d` |
| SecondInter.lean | `Sphere.secondInter`: computes second intersection of a line through a sphere point; properties include involutivity, collinearity, betweenness for interior points, and applications to simplex face relationships |
| Tangent.lean | Tangency definitions: `IsTangentAt`, `IsTangent` (sphere-subspace tangency), `tangentSet`, `tangentsFrom`, `commonTangents`, `commonIntTangents`, `commonExtTangents` (internal/external common tangents), `IsExtTangent`, `IsIntTangent` (sphere-sphere tangency), distance characterizations |

## Subdirectories

(none)

## Search Tags

sphere cospherical concyclic diameter center radius power-of-point intersecting-chords intersecting-secants tangent tangent-line tangent-space orthRadius second-intersection ptolemy freek-55 freek-95 euclidean-geometry affine-space inner-product cyclic-quadrilateral internal-tangent external-tangent
