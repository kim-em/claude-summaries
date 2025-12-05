---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/NormedSpace
generated: 2025-12-05T08:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 19
subdirs_count: 5
---

# NormedSpace

## Overview

The `NormedSpace/` directory is a comprehensive deprecated import layer providing backward compatibility for code that references the old `Mathlib.Analysis.NormedSpace.*` module paths. All 19 top-level files are deprecated modules (deprecated between September and November 2025) that forward to new locations in the reorganized `Mathlib.Analysis.Normed.*` hierarchy (covering `Normed.Module.*`, `Normed.Operator.*`, `Normed.Algebra.*`, `Normed.Ring.*`, and `Normed.Group.*`). The directory encompasses a wide range of normed space theory including ball actions, conformal linear maps, module connectivity, dual numbers, extended normed spaces, RCLike abstractions, Riesz lemma, indicator functions, and M-structure. The five subdirectories provide deprecated imports for advanced topics: alternating multilinear maps with curry/uncurry operations (`Alternating/`), Hahn-Banach extension and separation theorems (`HahnBanach/`), multilinear maps with curry operations (`Multilinear/`), operator norms covering basic theory through completeness and multiplicative structure (`OperatorNorm/`), and pi tensor products with injective and projective seminorms (`PiTensorProduct/`). This directory serves as a transitional layer maintaining API stability during the major normed space reorganization, ensuring existing code continues to function while the library migrates to the new module hierarchy.

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
- [x] `Multilinear/` - Multilinear maps between normed spaces (complete)
- [x] `OperatorNorm/` - Operator norms for continuous linear maps (complete)
- [x] `PiTensorProduct/` - Pi tensor products of normed spaces (complete)

## Search Tags

normed-spaces deprecated-imports backward-compatibility module-reorganization alternating-maps hahn-banach operator-norm multilinear-maps tensor-products conformal-maps dual-numbers riesz-lemma rclike ball-actions indicator-functions
