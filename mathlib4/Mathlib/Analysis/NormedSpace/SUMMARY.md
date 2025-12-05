---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/NormedSpace
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 19
subdirs_count: 5
---

# NormedSpace

## Overview

The `NormedSpace/` directory is a deprecated import layer providing backward compatibility for code that references the old `Mathlib.Analysis.NormedSpace.*` module paths. All files are deprecated modules (deprecated between September 2025 and November 2025) that forward to new locations in the reorganized `Mathlib.Analysis.Normed.*` hierarchy (covering `Normed.Module.*`, `Normed.Operator.*`, `Normed.Algebra.*`, `Normed.Ring.*`, and `Normed.Group.*`). The directory also contains subdirectories for more complex topics like alternating maps, operator norms, multilinear maps, the Hahn-Banach theorem, and pi tensor products.

## Key Files

| File | Purpose |
|------|---------|
| BallAction.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.Ball.Action` (deprecated 2025-09-02) |
| ConformalLinearMap.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Operator.Conformal` (deprecated 2025-09-16) |
| Connected.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.Connected` (deprecated 2025-11-21) |
| DualNumber.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Algebra.DualNumber` (deprecated 2025-09-02) |
| ENormedSpace.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.ENormedSpace` (deprecated 2025-11-21) |
| Extend.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.RCLike.Extend` (deprecated 2025-09-18) |
| Extr.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.Extr` (deprecated 2025-11-21) |
| FunctionSeries.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Group.FunctionSeries` (deprecated 2025-09-02) |
| HomeomorphBall.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.Ball.Homeomorph` (deprecated 2025-09-02) |
| IndicatorFunction.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Group.Indicator` (deprecated 2025-09-02) |
| Int.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Ring.Int` (deprecated 2025-09-02) |
| MStructure.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.MStructure` (deprecated 2025-11-21) |
| MultipliableUniformlyOn.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.MultipliableUniformlyOn` (deprecated 2025-11-21) |
| Normalize.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.Normalize` (deprecated 2025-11-21) |
| Pointwise.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.Ball.Pointwise` (deprecated 2025-09-02) |
| RCLike.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.RCLike.Basic` (deprecated 2025-09-02) |
| Real.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.RCLike.Real` (deprecated 2025-09-02) |
| RieszLemma.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.RieszLemma` (deprecated 2025-11-21) |
| SphereNormEquiv.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.Ball.RadialEquiv` (deprecated 2025-09-02) |

## Subdirectories

- [x] `Alternating/` - Alternating multilinear maps in normed spaces (complete)
- [x] `HahnBanach/` - Hahn-Banach extension theorem for continuous linear functionals (complete)
- [ ] `Multilinear/` - Multilinear maps between normed spaces (pending)
- [ ] `OperatorNorm/` - Operator norms for continuous linear maps (pending)
- [ ] `PiTensorProduct/` - Pi tensor products of normed spaces (pending)

## Search Tags

normed-spaces deprecated-imports backward-compatibility module-reorganization alternating-maps hahn-banach operator-norm multilinear-maps tensor-products conformal-maps dual-numbers riesz-lemma rclike ball-actions indicator-functions
