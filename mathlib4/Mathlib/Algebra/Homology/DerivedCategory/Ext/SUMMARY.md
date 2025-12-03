---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Homology/DerivedCategory/Ext
generated: 2025-12-02T09:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 6
subdirs_count: 0
---

# Ext

## Overview

The `Ext/` directory implements Ext groups in abelian categories as universe-polymorphic types `Ext.{w} X Y n : Type w` defined via small shifted hom-types in the derived category. The framework establishes when these types are small (via `HasExt.{w}` typeclass), constructs long exact sequences from short exact sequences with connecting homomorphisms (extClass), proves composition is bilinear, demonstrates smallness for categories with enough projectives or injectives, and provides module structures when the abelian category is linear over a ring R. The design carefully manages universes to handle scenarios where morphism types may be larger than desired Ext group types (e.g., étale sheaves).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `Ext.{w} X Y n` as `SmallShiftedHom` between single complexes in derived category, `HasExt.{w}` typeclass for smallness, composition with associativity, bijections `homEquiv₀` and additive group structure transported from derived category, `mk₀` constructor from morphisms, biproduct compatibility, universe changes via `chgUniv` (20KB) |
| ExactSequences.lean | Long exact sequences from short exact sequences `S`: covariant sequence `Ext X S.Xᵢ n₀ → ... → Ext X S.Xᵢ n₁` and contravariant sequence `Ext S.Xᵢ Y n₀ → ... → Ext S.Xᵢ Y n₁` when `n₀ + 1 = n₁`, with exactness proofs via ladder diagrams and homology sequences (13KB) |
| ExtClass.lean | Constructs `extClass : Ext S.X₃ S.X₁ 1` for short exact sequence `S` via localized composition of mapping cone morphisms, proves compatibility with `singleδ` from triangulated structure, vanishing lemmas `comp_extClass = 0` and `extClass_comp = 0` (4KB) |
| EnoughProjectives.lean | Proves `hasExt_of_enoughProjectives`: if `C` is locally `w`-small abelian category with enough projectives, then `HasExt.{w} C` holds, via induction showing `Ext P Y (n+1) = 0` for projective `P` using split epimorphisms to single functors and vanishing results (5KB) |
| EnoughInjectives.lean | Dual results to EnoughProjectives: proves `hasExt_of_enoughInjectives` for categories with enough injectives, showing `Ext X I (n+1) = 0` for injective `I` via split monomorphisms from single functors (5KB) |
| Linear.lean | Module structures on `Ext X Y n` for R-linear abelian categories: proves `Module R (Ext X Y n)`, characterizes scalar multiplication as `r • x = x.comp (mk₀ (r • 𝟙 Y)) (add_zero n)`, compatibility with composition, bilinear map structures for composition over commutative rings (4KB) |

## Subdirectories

_(none)_

## Search Tags

ext-groups abelian-category derived-category universe-polymorphism small-types shifted-hom long-exact-sequence short-exact-sequence connecting-homomorphism ext-class composition bilinear-map enough-projectives enough-injectives module-structure linear-category locally-small additive-functor
