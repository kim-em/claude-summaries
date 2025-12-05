---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Module/Ball
generated: 2025-12-05T09:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# Ball

## Overview

The `Ball/` directory provides specialized theory for metric balls and spheres in normed spaces. It establishes multiplicative actions of unit balls/spheres on balls/spheres (treating them as subtype sets with scalar multiplication), defines homeomorphisms between normed spaces and unit balls, studies pointwise scalar multiplication properties (including ball rescaling and convexity), and provides radial/polar-like coordinates via homeomorphisms between nonzero elements and sphere × (0,∞). This complements the general normed space theory with geometric structure specific to balls and spheres.

## Key Files

| File | Purpose |
|------|---------|
| Action.lean | Multiplicative actions of closed unit balls and unit spheres on balls/spheres centered at origin; proves `MulAction`, `ContinuousSMul`, `IsScalarTower`, and `SMulCommClass` instances for all combinations (closed ball/sphere acting on ball/closed ball/sphere); includes lemmas that points on spheres are distinct from their negatives in characteristic zero |
| Homeomorph.lean | Homeomorphisms between normed spaces and balls; `OpenPartialHomeomorph.univUnitBall` maps `E → ball 0 1` via `x ↦ (√(1 + ‖x‖²))⁻¹ • x`; `Homeomorph.unitBall` as global homeomorphism; `OpenPartialHomeomorph.unitBallBall` for affine homeomorphism `r • · +ᵥ c` between unit ball and arbitrary ball; `univBall` combines these for smooth open partial homeomorphisms |
| Pointwise.lean | Properties of pointwise scalar multiplication on sets; diameter and extended diameter under scalar multiplication (`ediam_smul₀`, `diam_smul₀`); ball/sphere/closed ball rescaling formulas (`smul_ball`, `smul_sphere'`, `smul_closedBall'`); boundedness preservation under scalar multiplication; thickening operations on balls (`thickening_ball`, `cthickening_closedBall`); ball arithmetic (`ball_add_ball`, `closedBall_add_closedBall`); existence of intermediate points with controlled distances (`exists_dist_eq`, `exists_dist_lt_lt`) |
| RadialEquiv.lean | Radial/polar-like coordinate systems for normed spaces; `homeomorphSphereProd E r hr` provides homeomorphism between `{0}ᶜ ⊆ E` and `sphere 0 r × Ioi 0` via `x ↦ (r • ‖x‖⁻¹ • x, ‖x‖/r)`; `homeomorphUnitSphereProd` specializes to unit sphere (generalized polar coordinates); proves open sets on `ℝ × sphere` under scalar multiplication remain open |

## Subdirectories

(none)

## Search Tags

balls spheres metric-balls closed-balls multiplicative-actions scalar-multiplication pointwise-operations homeomorphisms unit-ball sphere-actions polar-coordinates radial-equivalence diameter thickening ball-arithmetic convexity normed-spaces geometric-structure affine-homeomorphisms continuous-smul
