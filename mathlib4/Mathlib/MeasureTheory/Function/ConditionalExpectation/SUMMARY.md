---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Function/ConditionalExpectation
generated: 2026-01-25T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# ConditionalExpectation

## Overview

The `ConditionalExpectation/` directory implements the conditional expectation operator in measure theory. This is a fundamental construction in probability theory and functional analysis that projects integrable functions onto subspaces corresponding to sub-σ-algebras. The construction proceeds in four stages: first defining conditional expectation for L² functions via orthogonal projection, then extending to indicators of measurable sets, then to L¹ functions via a continuous linear map, and finally to general integrable functions. The directory includes theory for uniqueness, properties of conditional expectation with respect to indicators, bilinear pull-out properties, real-valued specializations including Radon-Nikodym derivatives, and characterizations of functions that are almost everywhere measurable with respect to a sub-σ-algebra.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Main definition of conditional expectation `condExp` (notation `μ[f\|m]`) as an integrable, m-strongly measurable function satisfying the defining integral equality on m-measurable sets; builds on CondexpL1 to provide the function-valued conditional expectation |
| CondexpL2.lean | Conditional expectation in L²: defines `condExpL2` as the orthogonal projection onto the subspace of almost everywhere m-measurable L² functions (lpMeas), first step in the construction |
| CondexpL1.lean | Conditional expectation in L¹: extends from indicators to general L¹ functions via `condExpL1CLM`, a continuous linear map from L¹ to itself; uses the same construction technique as the Bochner integral |
| AEMeasurable.lean | Functions almost everywhere measurable with respect to a sub-σ-algebra: defines `lpMeas F 𝕜 m p μ` as the subspace of Lp containing functions AE-measurable with respect to m; establishes isometry with trimmed measure Lp space; provides induction principles for Lp functions |
| Unique.lean | Uniqueness of conditional expectation: proves that two Lp functions which are AE m-measurable and have equal integrals on all m-measurable sets are equal almost everywhere |
| Indicator.lean | Conditional expectation of indicator functions: proves `μ[s.indicator f\|m] = s.indicator μ[f\|m]` when s is m-measurable; includes results about conditional expectation on restricted measures |
| PullOut.lean | Pull-out property for bilinear maps: proves `μ[B f g\|m] = B f μ[g\|m]` when f is m-measurable and B is a continuous bilinear map; specializes to scalar multiplication and multiplication |
| Real.lean | Conditional expectation of real-valued functions: relates conditional expectation to Radon-Nikodym derivatives (`rnDeriv_ae_eq_condExp`), proves uniform integrability of conditional expectations, establishes norm inequalities via Jensen-type arguments |

## Subdirectories

(none)

## Search Tags

conditional-expectation orthogonal-projection sub-sigma-algebra l2-space l1-space lpMeas ae-measurable uniqueness indicator-function pull-out-property bilinear-map radon-nikodym-derivative uniform-integrability trim-measure measurable-subspace probability-theory
