---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Abelian
generated: 2025-12-07T16:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 19
subdirs_count: 6
---

# Abelian

## Overview

The `Abelian/` directory provides a comprehensive formalization of abelian category theory, one of the foundational frameworks for homological algebra and algebraic geometry in mathlib4. An abelian category is a preadditive category with finite products, kernels and cokernels, where every monomorphism and epimorphism is normal. The directory develops the complete theoretical apparatus in layers: foundational definitions and theorems (mono + epi = iso, coimage-image comparison), exactness characterizations and diagram-chasing via pseudoelements, classical diagram lemmas (four, five, snake) for exact sequences, dimension theory and resolutions for injective and projective objects, derived functors and Ext groups for computing homological invariants, Grothendieck axioms (AB4/AB5) characterizing exactness of colimits, the full theory of Grothendieck abelian categories including existence of enough injectives via the small object argument, Gabriel-Popescu and Freyd-Mitchell embedding theorems demonstrating that abstract abelian categories can be faithfully represented as module categories, Serre subcategories and quotient structures, and transfer mechanisms for inheriting abelian structure. Together, these components provide the categorical infrastructure for derived categories, sheaf cohomology, and modern homological methods throughout mathlib.

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
- [x] `GrothendieckCategory/` - Grothendieck abelian categories with colimits, generators, and enough injectives (complete)
- [x] `Injective/` - Injective objects, injective resolutions, and enough injectives (complete)
- [x] `Projective/` - Projective objects, projective resolutions, and enough projectives (complete)
- [x] `SerreClass/` - Serre subcategories and quotient categories (complete)

## Search Tags

abelian-categories preadditive kernels cokernels exact-sequences homological-algebra derived-functors ext-groups injective-objects projective-objects pseudoelements diagram-chasing freyd-mitchell-embedding grothendieck-categories coimage-image-comparison normal-monomorphism normal-epimorphism
