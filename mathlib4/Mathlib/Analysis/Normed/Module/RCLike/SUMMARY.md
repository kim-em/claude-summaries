---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Module/RCLike
generated: 2025-12-05T08:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# RCLike

## Overview

The `RCLike/` directory provides specialized theory for normed spaces over the fields `ℝ` (real numbers) and `ℂ` (complex numbers), unified through the `RCLike` typeclass. It contains results that require properties specific to these fields but are not available for arbitrary normed fields. Key topics include vector normalization, operator norm bounds from ball/sphere bounds, norm preservation of continuous linear map extensions from ℝ to 𝕜, and topological properties of balls and spheres in real normed spaces (closure, interior, frontier formulas).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Module index re-exporting `Analysis.RCLike.Basic`, `Real.lean`, and operator theory; proves `RCLike.norm_coe_norm` (norm of scalar embedding equals original norm), `norm_smul_inv_norm` (unit normalization), `norm_smul_inv_norm'` (normalization to arbitrary length r); `LinearMap.bound_of_sphere_bound` and `bound_of_ball_bound'` (derive operator norm bounds from bounds on sphere/ball); `ContinuousLinearMap.opNorm_bound_of_ball_bound` (operator norm ≤ c/r given ‖f z‖ ≤ c on ball of radius r); `NormedSpace.sphere_nonempty_rclike` (spheres are nonempty for r ≥ 0 in nontrivial spaces) |
| Extend.lean | Norm preservation when extending continuous ℝ-linear functionals to 𝕜-linear functionals; `norm_extendTo𝕜'_bound` (‖fr.extendTo𝕜' x‖ ≤ ‖fr‖ * ‖x‖), `norm_extendTo𝕜'` (‖fr.extendTo𝕜'‖ = ‖fr‖ as operator norm equality), `norm_extendTo𝕜` (simp lemma for restricted scalars version); relies on `LinearMap.norm_extendTo𝕜'_apply_sq` identity |
| Real.lean | Topological and geometric properties specific to real normed spaces; `Real.punctured_nhds_module_neBot` (no isolated points in nontrivial ℝ-modules); `closure_ball`, `frontier_ball`, `interior_closedBall`, `frontier_closedBall` (topological characterizations for r ≠ 0); primed versions for nontrivial separated spaces; `exists_norm_eq` (surjectivity of norm map onto [0,∞)); `range_norm = Ici 0`, `nnnorm_surjective`, `NormedSpace.sphere_nonempty ↔ 0 ≤ r` |

## Subdirectories

None.

## Search Tags

rclike real-closed-like normed-spaces-over-reals normed-spaces-over-complex vector-normalization operator-norm-bounds ball-bounds sphere-bounds continuous-linear-map-extension norm-preservation real-normed-spaces closure-ball frontier-ball interior-closedBall frontier-sphere topological-properties nontrivial-spaces surjectivity-norm functional-extension scalar-tower
