---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Function/LpSpace
generated: 2026-01-25T23:20:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 1
---

# LpSpace

## Overview

The `LpSpace/` directory contains the core definitions and theory for Lp spaces in measure theory. Lp spaces consist of equivalence classes of measurable functions with finite eLpNorm. This includes the fundamental definition of the Lp space as an additive subgroup of almost everywhere equal functions, completeness results showing Lp is a complete metric space for 1 ≤ p, the embedding of bounded continuous functions into Lp for finite measures, continuity results for composition with measure-preserving maps, indicator functions of sets as Lp elements, and the action of domain multiplication groups on Lp spaces. The `DomAct/` subdirectory develops the theory of how the domain multiplication group acts on Lp spaces via measure-preserving transformations, establishing that this action preserves all algebraic and metric structure while remaining continuous under appropriate topological conditions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of Lp space as subtype of α →ₘ[μ] E with finite eLpNorm, notations α →₁[μ] E and α →₂[μ] E, Lipschitz action by composition including continuous linear maps, positive/negative parts |
| Complete.lean | Completeness of Lp spaces: proves Lp is a complete metric space for 1 ≤ p via liminf inequalities for eLpNorm under pointwise convergence |
| ContinuousCompMeasurePreserving.lean | Continuity of composition with continuous measure-preserving maps: proves composition of Lp function with measure-preserving map is continuous in both arguments for R₁ spaces with inner regular measures |
| ContinuousFunctions.lean | Embedding of bounded continuous functions into Lp: shows bounded continuous functions on finite-measure spaces lie in Lp with norm bounds, defines toLp bounded linear map |
| Indicator.lean | Indicator functions as Lp elements: defines indicatorConstLp for characteristic functions of measurable sets with finite measure, proves continuity and algebraic properties, includes compact support results |

## Subdirectories

- [x] `DomAct/` - Action of domain multiplication groups Mᵈᵐᵃ on Lp spaces via measure-preserving transformations

## Search Tags

lp-space lebesgue-space normed-space complete-metric-space elpnorm measure-preserving bounded-continuous-function indicator-function compact-support domain-action smul-invariant liminf-convergence
