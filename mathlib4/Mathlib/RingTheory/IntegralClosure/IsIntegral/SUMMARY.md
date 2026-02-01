---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/IntegralClosure/IsIntegral
generated: 2026-02-01T18:42:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 3
subdirs_count: 0
---

# IsIntegral

## Overview

The `IsIntegral/` directory provides the core predicate `IsIntegral R x` asserting that an element x of an R-algebra is integral over R (i.e., is a root of a monic polynomial with coefficients in R). It contains foundational definitions, basic properties of integral elements (mapping under ring homomorphisms, adjoin spans being finitely generated), and the related concept of almost integral elements with the complete integral closure.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines `RingHom.IsIntegralElem f x` (x is integral w.r.t. ring hom f) and `IsIntegral R x` (x is integral over R via algebraMap); minimal imports for maximum reusability |
| Basic.lean | Properties of integral elements: mapping under ring homs (`IsIntegral.map`), compatibility with algebra towers (`IsIntegral.tower_top`), integrality of 0/1/algebraMap, `fg_adjoin_singleton` (adjoin of integral element is finitely generated as R-module), product algebras, and composition with injective maps |
| AlmostIntegral.lean | Defines `IsAlmostIntegral R s` (exists r in non-zero-divisors s.t. r * s^n is in R for all n); defines `completeIntegralClosure R S` as the subalgebra of almost integral elements; proves equivalence with `IsIntegral` for Noetherian domains with fraction rings (Stacks 00GW, 00GX) |

## Subdirectories

(none)

## Search Tags

IsIntegral RingHom.IsIntegralElem monic-polynomial integral-element algebraMap algebra-tower fg-adjoin finitely-generated-module IsAlmostIntegral almost-integral completeIntegralClosure complete-integral-closure non-zero-divisors Noetherian fraction-ring FractionRing
