---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/SmallObject
generated: 2025-12-08T15:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: preliminary
files_count: 6
subdirs_count: 1
---

# SmallObject

## Overview

The `SmallObject/` directory implements Quillen's small object argument, a fundamental construction in category theory used to obtain functorial factorization systems. Given a class of morphisms `I : MorphismProperty C`, the small object argument (when it applies) factors any morphism `f : X ⟶ Y` as `ιObj I κ f ≫ πObj I κ f = f`, where the first morphism is a relative `I`-cell complex (a transfinite composition of pushouts of coproducts of morphisms in `I`) and the second has the right lifting property with respect to `I`. This construction proceeds by transfinite iteration indexed by a suitable regular cardinal `κ`, iterating a functor `Arrow C ⥤ Arrow C` that attaches `I`-cells at each step. The framework includes general machinery for transfinite constructions via well-ordered induction and proofs that the left lifting property is stable under transfinite composition.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Main entry point and typeclass `HasSmallObjectArgument I` asserting existence of a suitable cardinal for the small object argument, with theorems characterizing `I.rlp.llp` as retracts of transfinite compositions |
| Construction.lean | Defines the functor `SmallObject.functor f : Arrow C ⥤ Arrow C` that attaches `f`-cells via pushouts of coproducts indexed by commutative squares |
| IsCardinalForSmallObjectArgument.lean | Technical typeclass `IsCardinalForSmallObjectArgument I κ` specifying conditions on a regular cardinal κ (smallness, colimit existence, presentability-like conditions) that enable the small object argument, plus the main factorization construction |
| TransfiniteCompositionLifting.lean | Proves the left lifting property is stable under transfinite composition via well-order induction, constructing compatible liftings at limit stages using continuity |
| TransfiniteIteration.lean | General framework for iterating a successor structure `Φ : SuccStruct C` along a well-ordered type `J` to obtain `Φ.iteration J` as a colimit |
| WellOrderInductionData.lean | Infrastructure for limits of inverse systems indexed by well-ordered types, showing surjectivity of `F.sections → F.obj (op ⊥)` given compatible extension data at successor and limit stages |

## Subdirectories

- [x] `Iteration/` - Detailed implementation machinery for transfinite iteration of successor structures (complete)

## Search Tags

small-object-argument quillen-small-object-argument factorization-systems weak-factorization-systems lifting-properties relative-cell-complexes transfinite-composition transfinite-iteration well-ordered-types cardinals regular-cardinals pushouts coproducts model-categories homotopical-algebra
