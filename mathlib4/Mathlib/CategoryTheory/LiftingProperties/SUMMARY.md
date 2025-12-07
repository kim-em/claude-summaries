---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/LiftingProperties
generated: 2025-12-07T08:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 5
subdirs_count: 0
---

# LiftingProperties

## Overview

The `LiftingProperties/` directory formalizes the lifting property between morphisms in category theory and develops its fundamental theory. A morphism `i : A ⟶ B` has the left lifting property with respect to `p : X ⟶ Y` (equivalently, `p` has the right lifting property with respect to `i`) when every commutative square with `i` on the left and `p` on the right admits a diagonal lift. This directory establishes basic properties of lifting properties (closure under composition, isomorphism, retracts), shows compatibility with adjunctions and parametrized adjunctions, and proves lifting properties are preserved by limits and colimits (pullbacks, pushouts, products, coproducts). Lifting properties are fundamental to weak factorization systems and model category theory.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `HasLiftingProperty` typeclass with closure properties under composition, isomorphisms, opposites, and retracts |
| Adjunction.lean | Lifting property preservation by adjunctions: `G.map i` has left lifting property w.r.t. `p` iff `i` has left lifting property w.r.t. `F.map p` |
| ParametrizedAdjunction.lean | Lifting properties for parametrized adjunctions with bifunctors, pushout/pullback squares, and equivalence of lifting properties via adjunction |
| Limits.lean | Lifting property preservation by limits and colimits: pushouts, pullbacks, products, and coproducts |
| Over.lean | Lifting properties in Over categories, showing morphisms in `Over S` have lifting properties when underlying morphisms in `C` do |

## Subdirectories

None.

## Search Tags

lifting-properties left-lifting-property right-lifting-property commutative-squares diagonal-lifts weak-factorization-systems adjunctions parametrized-adjunctions pushouts pullbacks products coproducts over-categories model-categories
