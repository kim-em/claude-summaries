---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Manifold/IntegralCurve
generated: 2026-01-24T06:35:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# IntegralCurve

## Overview

The `IntegralCurve/` directory formalizes integral curves of vector fields on smooth manifolds. An integral curve `γ : ℝ → M` of a vector field `v` satisfies the property that its derivative at each point `t` equals the vector field evaluated at `γ(t)`. The library provides three variants: global integral curves (`IsMIntegralCurve`), local integral curves at a point (`IsMIntegralCurveAt`), and integral curves on a set (`IsMIntegralCurveOn`). Key results include local existence and uniqueness theorems (via Picard-Lindelöf), transformation lemmas for translation and scaling of curves, and a "uniform time lemma" establishing global existence when local curves exist with uniform time bounds.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions `IsMIntegralCurve`, `IsMIntegralCurveAt`, `IsMIntegralCurveOn`; equivalences between variants; continuity and differentiability properties; expression in local charts via `tangentCoordChange` |
| ExistUnique.lean | Local existence theorem `exists_isMIntegralCurveAt_of_contMDiffAt` for C^1 vector fields at interior points (via Picard-Lindelöf); uniqueness theorem `isMIntegralCurveAt_eventuallyEq_of_contMDiffAt`; global uniqueness on Hausdorff manifolds; periodicity-vs-injectivity dichotomy |
| Transform.lean | Translation lemmas (`comp_add`) showing `γ ∘ (· + dt)` is an integral curve when `γ` is; scaling lemmas (`comp_mul`) showing `γ ∘ (· * a)` is an integral curve of `a • v`; constant curves at zeros of the vector field |
| UniformTime.lean | Uniform time lemma: if local integral curves exist with uniform time bound `ε > 0` at every point, then global integral curves exist; piecewise extension of integral curves on overlapping intervals |

## Subdirectories

(none)

## Search Tags

integral-curve vector-field IsMIntegralCurve IsMIntegralCurveAt IsMIntegralCurveOn picard-lindelof existence uniqueness HasMFDerivAt tangent-vector smooth-manifold periodic-curve translation scaling uniform-time global-existence
