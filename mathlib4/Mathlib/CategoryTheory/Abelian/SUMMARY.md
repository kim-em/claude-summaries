---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Abelian
generated: 2025-12-07T08:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 19
subdirs_count: 6
---

# Abelian

## Overview

The `Abelian/` directory provides a comprehensive formalization of abelian categories and their properties in mathlib4. An abelian category is a preadditive category with finite products, kernels and cokernels, where every monomorphism and epimorphism is normal. This directory includes the basic definition and fundamental theorems (mono + epi = iso, factorization through images/coimages), exactness properties and diagram-chasing techniques using pseudoelements, derived functors (left and right derived), special classes of objects (injective/projective), Grothendieck axioms and categories, the Freyd-Mitchell embedding theorem showing every small abelian category embeds into modules over a ring, and transfer theorems for constructing abelian structures.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of abelian categories as preadditive categories with finite products, kernels, cokernels, and normal mono/epis; proves mono+epi=iso and coimage-image comparison is an isomorphism |
| NonPreadditive.lean | Shows every category with zero object, kernels, cokernels, and normal mono/epis admits a preadditive structure, reconstructing addition on morphisms from categorical limits |
| Exact.lean | Exactness properties in abelian categories relating to kernels and images; proves exact sequences characterized by imageSubobject = kernelSubobject |
| Pseudoelements.lean | Pseudoelement formalization allowing diagram-chasing proofs; elements as equivalence classes of arrows with metatheorems for exactness, mono/epi surjectivity/injectivity |
| Images.lean | Abelian image (kernel of cokernel) and coimage (cokernel of kernel) with canonical comparison morphism |
| FreydMitchell.lean | Freyd-Mitchell embedding theorem: every small abelian category embeds fully, faithfully, and exactly into modules over a ring via Grothendieck category techniques |
| LeftDerived.lean | Left-derived functors F.leftDerived n for additive functors using projective resolutions and homotopy categories |
| RightDerived.lean | Right-derived functors F.rightDerived n for additive functors using injective resolutions and homotopy categories |
| Ext.lean | Ext groups Ext R C n as bifunctor Cᵒᵖ ⥤ C ⥤ Module R defined by deriving the hom bifunctor |
| Transfer.lean | Transfer abelian structure from category D to C via adjunction; if G ⊣ F with G left exact and F ⋙ G ≅ 𝟭 C, then C inherits abelian structure |
| FunctorCategory.lean | Shows functor categories C ⥤ D are abelian when D is abelian; componentwise kernels, cokernels, and images |
| Opposite.lean | Opposite of an abelian category is abelian with dual constructions |
| Subobject.lean | Subobject-specific results in abelian categories |
| Yoneda.lean | Yoneda lemma specializations for abelian categories |
| Monomorphisms.lean | Properties of monomorphisms in abelian categories |
| EpiWithInjectiveKernel.lean | Epimorphisms with injective kernels and their properties |
| Refinements.lean | Refinement lemmas for exact sequences and factorizations |
| Indization.lean | Ind-completion constructions for abelian categories |
| CommSq.lean | Commutative square diagrams in abelian categories |

## Subdirectories

- [x] `DiagramLemmas/` - Classic diagram lemmas (four lemma, five lemma, snake lemma, etc.) (complete)
- [x] `GrothendieckAxioms/` - AB3, AB4, AB5 axioms for Grothendieck abelian categories (complete)
- [~] `GrothendieckCategory/` - Grothendieck abelian categories with colimits, generators, and enough injectives (preliminary)
- [ ] `Injective/` - Injective objects, injective resolutions, and enough injectives (pending)
- [ ] `Projective/` - Projective objects, projective resolutions, and enough projectives (pending)
- [ ] `SerreClass/` - Serre subcategories and quotient categories (pending)

## Search Tags

abelian-categories preadditive kernels cokernels exact-sequences homological-algebra derived-functors ext-groups injective-objects projective-objects pseudoelements diagram-chasing freyd-mitchell-embedding grothendieck-categories coimage-image-comparison normal-monomorphism normal-epimorphism
