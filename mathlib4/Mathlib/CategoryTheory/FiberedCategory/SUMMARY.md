---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/FiberedCategory
generated: 2025-12-07T00:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 8
subdirs_count: 0
---

# FiberedCategory

## Overview

The `FiberedCategory/` directory contains the formalization of fibered categories and Grothendieck fibrations in mathlib4, following the theory from SGA 1. It provides the infrastructure for working with categories fibered over a base category via a functor `p : 𝒳 ⥤ 𝒮`, including the fundamental notions of Cartesian and cocartesian morphisms, (pre)fibered categories, fiber categories over each object in the base, and the bicategory of based categories. This framework is essential for algebraic geometry (descent theory, stacks) and categorical approaches to indexed/dependent type theory.

## Key Files

| File | Purpose |
|------|---------|
| HomLift.lean | API for expressing that morphisms lift through functors via `IsHomLift` typeclass, handling non-definitional equalities |
| Cartesian.lean | Cartesian and strongly Cartesian morphisms with universal properties, following SGA 1 VI 5.1 |
| Cocartesian.lean | Dual theory of cocartesian and strongly cocartesian morphisms (adapted from Cartesian.lean) |
| Fibered.lean | Definitions of prefibered (`IsPreFibered`) and fibered (`IsFibered`) categories per SGA 1 VI.6.1 |
| Fiber.lean | Fiber categories `Fiber p S` as subcategories of objects mapping to `S` with morphisms lifting `𝟙 S` |
| HasFibers.lean | Typeclass for extrinsic fiber presentations allowing custom fiber categories equivalent to standard fibers |
| BasedCategory.lean | Bicategory of based categories (categories with functor to base) with based functors and natural transformations |
| Grothendieck.lean | Proof that Grothendieck construction gives fibered category with HasFibers instance |

## Subdirectories

None.

## Search Tags

fibered-categories grothendieck-fibrations cartesian-morphisms cocartesian-morphisms fiber-categories based-categories descent-theory sga stacks algebraic-geometry indexed-categories dependent-types bicategories
