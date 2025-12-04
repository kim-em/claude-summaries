---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry/EllipticCurve/Affine
generated: 2025-12-04T22:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Affine

## Overview

The `Affine/` subdirectory provides a complete formalization of elliptic curves in affine coordinates, building from basic definitions through the full group law. It establishes the affine coordinate representation of Weierstrass curves, defines the Weierstrass equation and nonsingular condition, develops explicit formulas for point negation and addition via the secant-and-tangent process, and proves that nonsingular points form an abelian group. The development culminates in constructing an injective group homomorphism from nonsingular affine points to the ideal class group of the affine coordinate ring, providing a rigorous algebraic foundation for the group structure.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines the fundamental Weierstrass polynomial W(X,Y) in affine coordinates, the Equation predicate (W(x,y) = 0), and the Nonsingular condition (at least one partial derivative is non-zero); proves that elliptic curves are nonsingular at every point; establishes compatibility with base change and ring homomorphisms |
| Formula.lean | Develops explicit formulas for the group operations: negation formula (negY), slope computation (for both secants and tangents), and addition formulas (addX, addY); proves that these operations preserve the Weierstrass equation and nonsingular condition; includes key identities like the cyclic sum formula for collinear points |
| Point.lean | Defines the affine coordinate ring F[W] = F[X,Y]/⟨W(X,Y)⟩ and proves it is an integral domain; defines the inductive type of nonsingular points (either the point at infinity or a nonsingular affine point); establishes the complete group structure on nonsingular points; constructs the injective group homomorphism to the ideal class group via explicit ideal computations and norm degree calculations |

## Subdirectories

None.

## Search Tags

affine-coordinates weierstrass-equation nonsingular-condition polynomial-derivatives secant-tangent-process negation-formula slope-formula addition-formula group-law coordinate-ring ideal-class-group fractional-ideals norm-computation power-basis double-quotient elliptic-curve-points point-at-infinity base-change
