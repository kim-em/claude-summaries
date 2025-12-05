---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Affine
generated: 2025-12-05T08:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 8
subdirs_count: 0
---

# Affine

## Overview

The `Affine/` directory provides theory for normed affine spaces—affine spaces (add-torsors) equipped with compatible norm structures. It establishes the metric geometry of affine spaces over normed vector spaces, including fundamental results on homotheties, continuous affine maps with their norm structure, affine isometries and isometric equivalences, barycentric coordinates and simplex properties. Notable highlights include the Mazur-Ulam theorem (isometric bijections between normed affine spaces over ℝ are affine), characterizations of asymptotic cones in terms of boundedness, and properties of simplices such as scalene, equilateral, and regular configurations.

## Key Files

| File | Purpose |
|------|---------|
| AddTorsor.lean | Properties of normed add-torsors over normed spaces; proves distance formulas for homotheties (`dist p₁ (homothety p₁ c p₂) = ‖c‖ * dist p₁ p₂`), midpoint distance relations, and continuity properties of torsor operations |
| AddTorsorBases.lean | Barycentric coordinates and affine bases in normed affine spaces; proves continuity of barycentric coordinate maps (`continuous_barycentric_coord`), characterizes interiors of convex hulls of affine bases, shows barycentric coordinates are open maps in finite dimensions |
| AsymptoticCone.lean | Asymptotic cones in normed spaces; proves that the asymptotic cone of a set is non-trivial if and only if the set is unbounded, characterizes the cobounded filter via asymptotic neighborhoods on the unit sphere in finite-dimensional spaces |
| ContinuousAffineMap.lean | Norm structure on continuous affine maps between normed vector spaces; defines `‖f‖ = max ‖f 0‖ ‖f.cont_linear‖` to establish an isometric isomorphism `(V →ᴬ[𝕜] W) ≃ₗᵢ[𝕜] W × (V →L[𝕜] W)`, proves composition bound `‖f.comp g‖ ≤ ‖f‖ * ‖g‖ + ‖f 0‖` |
| Convex.lean | Simplices and convex polytopes in normed affine spaces; proves that a point with a neighborhood can be enclosed in the interior of a simplex (`exists_mem_interior_convexHull_affineBasis`), and that compact convex sets with neighborhoods contain convex polytopes |
| Isometry.lean | Affine isometries and isometric equivalences between normed add-torsors; defines `AffineIsometry 𝕜 P P₂` (notation `P →ᵃⁱ[𝕜] P₂`) and `AffineIsometryEquiv` (notation `P ≃ᵃⁱ[𝕜] P₂`), proves composition properties, conversion between affine and linear isometries |
| MazurUlam.lean | Mazur-Ulam theorem: isometric bijections between normed affine spaces over ℝ are affine; provides three formulations converting `IsometryEquiv` to `LinearIsometryEquiv` (when fixing zero) and to `AffineIsometryEquiv` (general case), based on Väisälä's proof |
| Simplex.lean | Properties of simplices in normed add-torsors; defines `Scalene` (all edge lengths different), `Equilateral` (all edge lengths equal), and `Regular` (equilateral with additional geometric properties), proves characterization lemmas for these simplex types |

## Subdirectories

(none)

## Search Tags

normed-affine-spaces add-torsors affine-isometry isometric-equivalence continuous-affine-maps mazur-ulam-theorem barycentric-coordinates affine-bases simplices convex-hulls homotheties asymptotic-cones metric-geometry affine-geometry normed-vector-spaces finite-dimensional scalene-simplex equilateral-simplex regular-simplex midpoint-convexity affine-maps
