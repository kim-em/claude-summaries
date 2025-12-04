---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology/SimplicialObject
generated: 2025-12-04T17:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# SimplicialObject

## Overview

The `SimplicialObject/` directory contains the general theory of simplicial objects in arbitrary categories. A simplicial object is defined as a contravariant functor from the simplex category to a category `C`, providing the foundational abstractions for working with sequences of objects connected by face and degeneracy maps. The directory includes core definitions (basic simplicial and cosimplicial objects with notation), structural theorems (split simplicial objects, coskeletal objects), functorial constructions (the opFunctor involution, the Gabriel-Zisman II functor), and establishes key categorical properties like limits and colimits.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `SimplicialObject C` as functors `SimplexCategoryᵒᵖ ⥤ C`, dual `CosimplicialObject` definition, notation `X _⦋n⦌` for simplicial objects and `X ^⦋n⦌` for cosimplicial, face maps `δ` and degeneracy maps `σ`, categorical properties (limits/colimits, extensionality), and basic morphisms |
| Coskeletal.lean | Theory of n-coskeletal simplicial objects (those that are right Kan extensions of their n-truncations), characterization via the coskeleton adjunction `coskAdj n`, and canonical isomorphism `isoCoskOfIsCoskeletal : X ≅ (cosk n).obj X` for coskeletal objects |
| II.lean | Gabriel-Zisman construction of the functor `II : SimplexCategory ⥤ SimplexCategoryᵒᵖ` (a cosimplicial object in SimplexCategoryᵒᵖ) which sends `⦋n⦌` to `⦋n + 1⦌` by swapping faces and degeneracies, used in homotopy theory and the calculus of fractions |
| Op.lean | Covariant involution `opFunctor : SimplicialObject C ⥤ SimplicialObject C` induced by reversing the simplex category via `SimplexCategory.rev`, proves it's an equivalence (`opEquivalence`), and shows composition with itself is naturally isomorphic to the identity |
| Split.lean | Theory of split simplicial objects: a splitting `s : Splitting X` decomposes each `X _⦋n⦌` as a coproduct of "nondegenerate simplices" `s.N i` indexed by epimorphisms in SimplexCategory; includes the category `SimplicialObject.Split C` of split simplicial objects |

## Subdirectories

*(No subdirectories)*

## Search Tags

simplicial-object cosimplicial-object presheaf simplex-category face-map degeneracy-map split-simplicial coskeletal right-kan-extension truncation opfunctor involution gabriel-zisman coproduct nondegenerate-simplex category-theory
