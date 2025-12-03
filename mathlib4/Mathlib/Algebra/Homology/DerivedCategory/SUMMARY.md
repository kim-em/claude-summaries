---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Homology/DerivedCategory
generated: 2025-12-02T11:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 9
subdirs_count: 1
---

# DerivedCategory

## Overview

The `DerivedCategory/` directory implements the derived category of an abelian category as the localization of cochain complexes indexed by ℤ with respect to quasi-isomorphisms, providing the complete triangulated structure with shift functors and distinguished triangles. The implementation includes localization functors (Q from cochain complexes, Qh from homotopy category), homology functors forming a shift sequence with long exact sequences, calculus of left/right fractions for morphism factorizations, and the canonical t-structure with truncation triangles. The framework proves that exact functors induce triangulated functors on derived categories, establishes fully faithfulness of single functors embedding abelian categories into their derived categories, and constructs distinguished triangles from short exact sequences. The Ext/ subdirectory provides universe-polymorphic Ext groups as small shifted hom-types, complete with long exact sequences, composition structure, and concrete computations via projective/injective resolutions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core construction of `DerivedCategory C` as `HomologicalComplexUpToQuasiIso C (ComplexShape.up ℤ)` with localization functors `Q` and `Qh`, triangulated structure via localization at subcategory of acyclic complexes, shift functors, and universe management via `HasDerivedCategory.{w}` typeclass (13KB) |
| ExactFunctor.lean | Proves exact functors `F : C₁ ⥤ C₂` (preserving finite limits/colimits) induce triangulated functors `F.mapDerivedCategory : DerivedCategory C₁ ⥤ DerivedCategory C₂` with shift compatibility via `CommShift` instances |
| Fractions.lean | Calculus of left and right fractions: factorizes morphisms `f : Q.obj X ⟶ Q.obj Y` as `inv (Q.map s) ≫ Q.map g` (right) or `Q.map g ≫ inv (Q.map s)` (left) with quasi-iso `s`, including bounded variants using truncation for `IsStrictlyLE`/`IsStrictlyGE` complexes (9KB) |
| FullyFaithful.lean | Proves `singleFunctor C n : C ⥤ DerivedCategory C` is fully faithful for all `n : ℤ`, establishing the abelian category embeds into its derived category via canonical isomorphism with homology functor composition |
| HomologySequence.lean | Constructs homology functors `homologyFunctor C n : DerivedCategory C ⥤ C` as homological functors forming shift sequence, with connecting homomorphisms `δ` and long exact sequences for distinguished triangles including exactness criteria |
| Linear.lean | Establishes that derived categories of linear (R-module enriched) abelian categories are R-linear: proves `Linear R (DerivedCategory C)` with linear localization functors Q, Qh, shift functors, and single functors |
| ShortExact.lean | Constructs distinguished triangle `triangleOfSES` in derived category from short exact sequence of cochain complexes via mapping cone, with connecting homomorphism and isomorphism to standard triangle |
| SingleTriangle.lean | Constructs distinguished triangle from short exact sequence `S` in abelian category `C` via single functor application, producing triangle in `DerivedCategory C` with objects `(singleFunctor C 0).obj S.Xᵢ` |
| TStructure.lean | Defines canonical t-structure on `DerivedCategory C` with `IsLE X n` (bounded above) and `IsGE X n` (bounded below) characterized by vanishing homology, proves truncation triangles exist, includes homology characterizations (8KB) |

## Subdirectories

- [x] `Ext/` - Ext groups in abelian categories: `Ext.{w} X Y n` as small shifted hom-types in derived category, composition of extensions, long exact sequences, computations via projective/injective resolutions (complete)

## Search Tags

derived-category triangulated-category localization quasi-isomorphism homotopy-category homology-functor shift-sequence exact-functor t-structure ext-groups calculus-of-fractions acyclic-complex distinguished-triangle short-exact-sequence connecting-homomorphism single-functor fully-faithful abelian-category cochain-complex verdier-localization
