---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Integral/CurveIntegral
generated: 2026-01-25T09:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# CurveIntegral

## Overview

The `CurveIntegral/` directory contains the formalization of curve integrals (also called line integrals or path integrals) for 1-forms along paths in normed spaces. It defines the integral `∫ᶜ x in γ, ω x` of a 1-form `ω : E → E →L[𝕜] F` along a path `γ`, establishes fundamental properties (additivity, reversal, composition), and proves Poincaré's lemma for convex sets showing that closed 1-forms admit primitives.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Curve integral foundations: defines `curveIntegral ω γ` (notation `∫ᶜ x in γ, ω x`) as `∫ t in 0..1, ω(γ(t))(γ'(t))` and `CurveIntegrable ω γ`, proves properties under path operations (refl, symm, trans, cast, segment), algebraic operations (add, neg, smul, restrictScalars), and derivative `HasFDerivWithinAt` of `∫ᶜ x in .segment a b, ω x` w.r.t. endpoint `b` at `a` |
| Poincare.lean | Poincaré lemma for 1-forms on convex sets: proves that closed 1-form (symmetric derivative `dω a x y = dω a y x`) on convex set admits primitive `f` with `fderiv f = ω`, uses divergence theorem on homotopy between paths to show curve integrals of closed forms are homotopy-invariant, includes primitive existence theorems for `HasFDerivWithinAt`, `fderivWithin`, and `fderiv` formulations |

## Subdirectories

(none)

## Search Tags

curve-integral line-integral path-integral 1-form closed-form exact-form poincare-lemma primitive convex-set homotopy-invariant segment-integral has-fderiv-within-at divergence-theorem symmetric-derivative curve-integrable interval-integral fundamental-theorem
