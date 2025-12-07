---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/FunctorCategory/Shapes
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# Shapes

## Overview

The `Shapes/` directory provides concrete instances of how specific limit shapes (products, pullbacks, kernels) behave in functor categories. Each file establishes pointwise isomorphisms showing that evaluating a limit/colimit of functors at an object `d` yields the corresponding limit/colimit of the evaluated functors. These results demonstrate that the general pointwise limit theory from `Basic.lean` applies to classical categorical constructions like products, pullbacks, and kernels.

## Key Files

| File | Purpose |
|------|---------|
| Kernels.lean | Proves that the kernel inclusion `ker.ι C` is itself a kernel in the functor category, and dually for cokernels, using `evaluationJointlyReflectsLimits/Colimits` |
| Products.lean | Establishes isomorphisms `(∏ᶜ f).obj d ≅ ∏ᶜ (fun s => (f s).obj d)` and dually for coproducts, showing that products/coproducts of functors evaluate pointwise |
| Pullbacks.lean | Proves `(pullback f g).obj d ≅ pullback (f.app d) (g.app d)` and the dual for pushouts, with simp lemmas for projections/injections |

## Subdirectories

None.

## Search Tags

functor-category-shapes pointwise-limits products coproducts pullbacks pushouts kernels cokernels evaluation-isomorphisms limit-shapes colimit-shapes discrete-limits cospan-limits
