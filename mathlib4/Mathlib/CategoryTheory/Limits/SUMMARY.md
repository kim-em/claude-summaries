---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits
generated: 2025-12-07T09:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 41
subdirs_count: 8
---

# Limits

## Overview

The `Limits/` directory provides the comprehensive formalization of limits and colimits in category theory, building from the foundational definitions of cones and cocones through the full theory of existence, preservation, reflection, and creation of limits. It implements the core theory (`Cones`, `IsLimit`, `HasLimits`), categorical properties of limit-preserving functors (`Preserves`, `Creates`), special limit constructions and shapes (`Shapes/` for products, pullbacks, equalizers, etc.), limits in specific categories (`Types`, `FunctorCategory`, `ConcreteCategory`), and advanced topics (final functors, van Kampen colimits, filtered colimits, presheaf representations). This infrastructure is essential for all of mathlib's categorical constructions, providing the foundation for adjunctions, completeness properties, sheaf theory, and higher categorical structures.

## Key Files

| File | Purpose |
|------|---------|
| Cones.lean | Cones and cocones over functors with natural transformations from constant functors, cone morphisms, and category of cones |
| IsLimit.lean | Core definition of `IsLimit` structure expressing universal property of limit cones via unique factorization |
| HasLimits.lean | Existence of limits: `LimitCone`, `HasLimit` typeclass, convenience functions (`limit`, `limit.π`, `limit.lift`), and completeness classes |
| Creates.lean | Functors that create limits (can lift limit cones from target to source) with `CreatesLimit` and related classes |
| Preserves/ | (subdirectory) Limit-preserving functors and preservation of specific shapes |
| Shapes/ | (subdirectory) Specific limit shapes: products, pullbacks, equalizers, pushouts, coproducts, kernels, cokernels, finite limits, etc. |
| Final.lean | Final and initial functors with equivalence between limits over F⋙G and limits over G for final F, plus colimit characterizations |
| Presheaf.lean | Density theorem: every presheaf is a colimit of representables, left Kan extensions along Yoneda, and free cocompletion |
| VanKampen.lean | Van Kampen colimits and universal colimits (stable under pullback), with equifibered natural transformations |
| Yoneda.lean | Limits in presheaf categories computed pointwise via Yoneda embedding |
| ConeCategory.lean | Category structure on cones with cone morphisms and functoriality of cone constructions |
| Opposites.lean | Duality between limits and colimits via opposite categories with natural isomorphisms |
| FilteredColimitCommutesFiniteLimit.lean | Filtered colimits commute with finite limits in Type and other categories |
| FilteredColimitCommutesProduct.lean | Specific case: filtered colimits commute with binary products |
| Fubini.lean | Fubini theorem for iterated limits: limit of limits equals limit over product category |
| ExactFunctor.lean | Bundled exact functors (preserving finite limits and/or colimits) as categories |
| FormalCoproducts.lean | Formal coproducts and their universal properties |
| Indization/ | (subdirectory) Ind-objects and ind-completion of categories |
| IndYoneda.lean | Ind-Yoneda lemma for colimits of representables |
| Connected.lean | Limits over connected diagrams with unique morphisms between cone points |
| IsConnected.lean | Connectedness conditions for limit existence |
| Bicones.lean | Bicones (simultaneous cones and cocones) for bifunctor diagrams |
| ColimitLimit.lean | Interaction between colimits and limits for bifunctors |
| Comma.lean | Limits and colimits in comma categories |
| ConeCategory.lean | Categorical structure on cones and cocones |
| ConcreteCategory/ | (subdirectory) Limits in concrete categories with underlying set functors |
| Elements.lean | Limits in category of elements |
| EpiMono.lean | Epimorphisms and monomorphisms as colimits and limits of parallel pairs |
| EssentiallySmall.lean | Essentially small diagrams and limit existence |
| Filtered.lean | Limits and colimits in filtered categories |
| FinallySmall.lean | Finally small functors and their properties |
| FintypeCat.lean | Limits and colimits in category of finite types |
| FullSubcategory.lean | Limits in full subcategories |
| FunctorCategory/ | (subdirectory) Limits in functor categories computed pointwise |
| FunctorToTypes.lean | Limits of functors to Type computed as sections |
| Lattice.lean | Lattice structure on subobjects via limits and colimits |
| MonoCoprod.lean | Monomorphisms and coproducts interaction |
| MorphismProperty.lean | Morphism properties stable under limits or colimits |
| Over.lean | Limits in over categories (slice categories) |
| Pi.lean | Limits in product categories computed componentwise |
| Preorder.lean | Limits in preorders as meets and joins |
| Presentation.lean | Presentations of objects via limits of free objects |
| Set.lean | Limits in category of sets |
| Sifted.lean | Sifted colimits (commuting with finite products) |
| Skeleton.lean | Limits in skeletal categories |
| SmallComplete.lean | Small-complete categories with all small limits |
| Types/ | (subdirectory) Limits and colimits in category of types |
| Unit.lean | Limits over empty diagrams as terminal objects |

## Subdirectories

- [ ] `ConcreteCategory/` - Limits in concrete categories with forgetful functors (pending)
- [ ] `Constructions/` - Limit constructions and transformations (pending)
- [ ] `Final/` - Additional theory of final functors (pending)
- [ ] `FunctorCategory/` - Limits in functor categories (pointwise limits) (pending)
- [ ] `Indization/` - Ind-objects and ind-completion (pending)
- [ ] `Preserves/` - Limit preservation, reflection, and creation by functors (pending)
- [ ] `Shapes/` - Specific limit shapes: products, pullbacks, equalizers, terminal objects, etc. (pending)
- [ ] `Types/` - Limits and colimits in Type category (pending)

## Search Tags

limits colimits cones cocones universal-property limit-cone colimit-cocone has-limits completeness cocompleteness preserves-limits creates-limits final-functors filtered-colimits van-kampen density-theorem yoneda-lemma presheaves exact-functors fubini ind-objects representables
