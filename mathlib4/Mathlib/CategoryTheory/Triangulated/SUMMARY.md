---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Triangulated
generated: 2025-12-08T15:45:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: preliminary
files_count: 14
subdirs_count: 2
---

# Triangulated

## Overview

The `Triangulated/` directory contains the formalization of triangulated and pretriangulated categories, which are fundamental structures in homological algebra and derived category theory. It implements the core theory of triangles (sequences X → Y → Z → X⟦1⟧ with composition zero), pretriangulated categories (categories with shift functors and distinguished triangles satisfying rotation and completion axioms), triangulated categories (pretriangulated categories satisfying the octahedron axiom), triangulated functors (functors preserving distinguished triangles), homological functors (functors to abelian categories sending distinguished triangles to exact sequences), and t-structures (certain filtrations on triangulated categories). This framework is essential for working with derived categories, spectral sequences, and other advanced homological constructions in algebraic geometry and topology.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of triangles (sextuples (X,Y,Z,f,g,h) with h : Z → X⟦1⟧), triangle morphisms, contractible triangles, and basic operations |
| Pretriangulated.lean | Pretriangulated categories with distinguished triangles, rotation axiom, completion axiom for morphisms, and exact sequence properties |
| Triangulated.lean | Triangulated categories satisfying the octahedron axiom (TR 4), including octahedron datum structures and morphisms |
| Functor.lean | Triangulated functors between pretriangulated categories via mapTriangle functor, with preservation of distinguished triangles |
| HomologicalFunctor.lean | Homological functors from pretriangulated to abelian categories, sending distinguished triangles to exact sequences with long exact sequence machinery |
| Adjunction.lean | Preservation of triangulated structure under adjunctions, showing adjoints of triangulated functors are triangulated |
| Yoneda.lean | Proof that Yoneda functors (preadditiveCoyoneda and preadditiveYoneda) are homological functors |
| Subcategory.lean | Triangulated subcategories with typeclass P.IsTriangulated and calculus of fractions for morphism properties |
| Rotate.lean | Rotation operations on triangles, producing new triangles by cyclic permutation of objects |
| TriangleShift.lean | Shift operations on triangles and their interaction with the category shift |
| Orthogonal.lean | Orthogonality relations between objects in triangulated categories |
| SpectralObject.lean | Spectral objects with filtrations in triangulated categories |

## Subdirectories

- [x] `Opposite/` - Opposite category structures for pretriangulated and triangulated categories (complete)
- [x] `TStructure/` - t-structures on triangulated categories with truncation functors (complete)

## Search Tags

triangulated-categories pretriangulated-categories homological-algebra distinguished-triangles octahedron-axiom triangulated-functors homological-functors exact-sequences derived-categories t-structures shift-functors rotation yoneda-lemma verdier-quotient abelian-categories
