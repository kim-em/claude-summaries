---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Shapes/Preorder
generated: 2025-12-07T12:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 6
subdirs_count: 0
---

# Preorder

## Overview

This directory provides specialized machinery for working with limits and colimits indexed by preordered and well-ordered types. It establishes fundamental results about how order-theoretic properties (least/greatest elements, successor structure, limit ordinals) interact with categorical limit constructions, and introduces the key concept of well-order-continuous functors that preserve colimits at limit ordinals. The centerpiece is a framework for transfinite compositions—morphisms that can be decomposed as colimits indexed by well-ordered types—which is essential for constructions by transfinite induction in category theory (see the small object argument).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Basic results: preorders with least elements have all limits, preorders with greatest elements have all colimits |
| Fin.lean | Proves 0 is initial and Fin.last is terminal in Fin types, enabling limit/colimit computations for finite chains |
| HasIterationOfShape.lean | Typeclass for categories supporting transfinite induction: requires colimits indexed by J and by initial segments Set.Iio j for limit ordinals j |
| PrincipalSeg.lean | Constructs canonical cocones for functors restricted along principal segments (order embeddings f : α <i β with top element) |
| TransfiniteCompositionOfShape.lean | Structure expressing that a morphism f : X ⟶ Y is a transfinite composition indexed by well-ordered type J via a well-order-continuous functor |
| WellOrderContinuous.lean | Well-order-continuous functors: functors F : J ⥤ C from well-ordered types that preserve colimits at limit ordinals (F(m) = colim_{j<m} F(j)) |

## Subdirectories

(No subdirectories)

## Search Tags

preorder-limits well-ordered-types transfinite-composition well-order-continuous limit-ordinals successor-ordinals initial-segments principal-segments transfinite-induction finite-chains order-bot order-top HasIterationOfShape colimits-at-limits
