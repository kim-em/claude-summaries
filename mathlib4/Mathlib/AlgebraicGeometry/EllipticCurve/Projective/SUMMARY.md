---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry/EllipticCurve/Projective
generated: 2025-12-04T20:45:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Projective

## Overview

The `Projective/` subdirectory provides the complete formalization of elliptic curves in projective coordinates, where points are represented as equivalence classes `[x : y : z]` of triples under scaling by units. This representation includes the point at infinity `[0 : 1 : 0]` as a proper projective point, avoiding the need for special handling as in affine coordinates. The directory establishes the homogeneous Weierstrass equation `Y²Z + a₁XYZ + a₃YZ² = X³ + a₂X²Z + a₄XZ² + a₆Z³`, defines the nonsingular condition via partial derivatives, provides explicit formulae for negation and addition of projective point representatives, and proves that nonsingular projective points form an abelian group isomorphic to the affine point group.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines the equivalence relation on projective point representatives (triples up to scaling by units), the homogeneous Weierstrass polynomial `W(X, Y, Z)` and its partial derivatives `W_X`, `W_Y`, `W_Z`, the `Nonsingular` condition requiring at least one partial derivative to be nonzero, proves Euler's homogeneous function theorem, establishes conversions between projective and affine coordinates, and provides lemmas for working with point equivalence classes |
| Formula.lean | Provides explicit polynomial formulae for group operations on projective point representatives: `negY` for negation, `dblZ`/`dblX`/`dblY` for point doubling (the 2-torsion operation), and `addZ`/`addX`/`addY` for point addition, with all formulae being homogeneous of degree 4 to ensure closure under the group operations, along with computational proofs relating these formulae to their affine counterparts |
| Point.lean | Defines the type `WeierstrassCurve.Projective.Point` of nonsingular projective points, implements negation `neg` and addition `add` operations that preserve the nonsingular condition, establishes the group law by proving `instAddCommGroup` making projective points an abelian group, provides conversions `toAffine`/`fromAffine` and `toAffineLift`/`fromAffine` between projective and affine point types, and proves `toAffineAddEquiv` showing the projective and affine point groups are isomorphic |

## Subdirectories

*(None)*

## Search Tags

elliptic-curves projective-coordinates homogeneous-equation weierstrass-polynomial partial-derivatives nonsingular-condition point-at-infinity equivalence-classes group-law negation addition point-doubling affine-projective-equivalence abelian-group euler-homogeneous-theorem
