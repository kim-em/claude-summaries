---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology/ModelCategory
generated: 2025-12-04T16:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 14
subdirs_count: 0
---

# ModelCategory

## Overview

The `ModelCategory/` directory contains the formalization of model category theory in Lean 4, implementing the axiomatic framework for homotopical algebra due to Quillen. It provides the core typeclass `ModelCategory C` which encodes the five model category axioms (CM1-CM5) for a category equipped with three distinguished classes of morphisms: fibrations, cofibrations, and weak equivalences. The directory includes fundamental constructions for doing homotopy theory (cylinder and path objects), defines homotopy relations (left and right homotopies), proves key results like the Whitehead theorem and Ken Brown's factorization lemma, and includes Joyal's trick for verifying lifting properties. All implementations follow Quillen's foundational work and modern references like Goerss-Jardine and are authored primarily by Joël Riou.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core model category typeclass with axioms CM1-CM5, defining a model category via three classes of morphisms (fibrations, cofibrations, weak equivalences) satisfying lifting properties and factorization axioms; includes alternate constructor using weak factorization systems |
| CategoryWithCofibrations.lean | Foundation typeclasses `CategoryWithFibrations`, `CategoryWithCofibrations`, and `CategoryWithWeakEquivalences` for categories equipped with distinguished morphism classes; defines trivial fibrations and trivial cofibrations; includes duality results for opposite categories |
| Instances.lean | Derives basic properties and instances from model category axioms: stability under composition/retracts/base-change, multiplicativity of morphism properties, behavior under pushouts/pullbacks/products, and weak factorization system characterizations |
| Homotopy.lean | Relates left and right homotopies in model categories, proving they coincide when objects are both cofibrant and fibrant; includes the Whitehead theorem showing weak equivalences between fibrant-cofibrant objects are homotopy equivalences (using Brown's lemma) |
| LeftHomotopy.lean | Defines left homotopy relation between morphisms relative to cylinder objects; introduces `LeftHomotopyRel` and quotient type `LeftHomotopyClass X Y`; proves it's an equivalence relation when X is cofibrant |
| RightHomotopy.lean | Dual construction defining right homotopy relation relative to path objects; introduces `RightHomotopyRel` and `RightHomotopyClass X Y`; proves it's an equivalence relation when Y is fibrant |
| Cylinder.lean | Defines cylinder objects (precylinders and good cylinders) for an object X, consisting of an object I with weak equivalence π : I → X and two sections i₀, i₁; used in the definition of left homotopies; proves existence of very good cylinders in model categories |
| PathObject.lean | Dual to Cylinder.lean, defines path objects for an object A consisting of object P with weak equivalence ι : A → P and two retractions p₀, p₁; used for right homotopies; proves existence of very good path objects |
| BrownLemma.lean | Ken Brown's factorization lemma: any morphism f : X → Y between cofibrant objects factors as i ≫ p with i a cofibration, p a trivial fibration having a section s that is also a cofibration; moreover if f is a weak equivalence, all three morphisms are weak equivalences |
| IsCofibrant.lean | Defines cofibrant and fibrant objects (objects for which the map from initial/to terminal is a cofibration/fibration); proves basic properties like stability under coproducts and products |
| JoyalTrick.lean | Joyal's trick for constructing model categories: proves that the left lifting property of cofibrations with respect to trivial fibrations follows from the lifting property of trivial cofibrations with respect to fibrations, plus stability conditions |
| Over.lean | Constructs model category structure on over categories Over S: a morphism in Over S is a cofibration/fibration/weak equivalence iff its underlying left component is in C; verifies all model category axioms transfer to the slice |
| Opposite.lean | Shows that the opposite of a model category is a model category, with fibrations and cofibrations swapped; proves all axioms transfer to the opposite category |

## Subdirectories

(No subdirectories)

## Search Tags

model-category homotopical-algebra fibration cofibration weak-equivalence quillen axioms cm1 cm2 cm3 cm4 cm5 weak-factorization-system lifting-property cylinder-object path-object left-homotopy right-homotopy homotopy-equivalence whitehead-theorem brown-lemma joyal-trick cofibrant-object fibrant-object over-category opposite-category factorization trivial-fibration trivial-cofibration
