---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/LineDeriv
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# LineDeriv

## Overview

The `LineDeriv/` directory formalizes line derivatives (also known as directional derivatives or Gateaux derivatives) for functions between normed spaces. Line derivatives measure the rate of change of a function along a specific direction vector, defined as `f(x + tv) = f(x) + t·f' + o(t)` for a direction `v`. This is a weaker notion than the Fréchet derivative, as the composition of line-differentiable functions is not generally line-differentiable. The directory includes the basic theory, measurability results, integration by parts formulas, and specific examples like quadratic forms.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines line derivatives (`lineDeriv`, `HasLineDerivAt`, `HasLineDerivWithinAt`, `LineDifferentiableAt`, `LineDifferentiableWithinAt`) as the derivative of `t ↦ f(x + t·v)` at `t=0`; develops API for congruence, monotonicity, uniqueness, and interaction with Fréchet derivatives; proves line-differentiable functions satisfy Lipschitz bounds on line derivatives |
| IntegrationByParts.lean | Proves integration by parts formulas for line derivatives and Fréchet derivatives: `∫ f·g' = -∫ f'·g` for functions on real vector spaces with Haar measure, assuming integrability of products; includes versions for general bilinear forms and specific scalar multiplication; uses Fubini's theorem and one-dimensional integration by parts |
| Measurable.lean | Proves measurability of line derivatives for continuous functions: `lineDeriv 𝕜 f x v` is measurable in `x` (for fixed `v`) and measurable in `(x,v)` jointly; includes strongly measurable and almost everywhere measurable versions; requires locally compact scalar field for fixed direction, second countability for uncurried version |
| QuadraticMap.lean | Proves quadratic forms are line-differentiable with line derivative given by the polar bilinear form: `lineDeriv 𝕜 f a b = polar f a b`; notable because it requires no topology on the domain, so applies to discontinuous quadratic forms on infinite-dimensional spaces |

## Subdirectories

(No subdirectories)

## Search Tags

line-derivative directional-derivative gateaux-derivative derivatives calculus fréchet-derivative integration-by-parts measurability quadratic-forms polar-form bilinear-forms haar-measure lipschitz normed-spaces continuous-functions
