---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits
generated: 2025-12-07T22:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 41
subdirs_count: 8
---

# Limits

## Overview

The `Limits/` directory provides the comprehensive formalization of limits and colimits in category theory, serving as the central infrastructure for universal constructions throughout mathlib. The directory is organized into three major layers: (1) **Core abstract theory** establishing the fundamental definitions and properties of limits via cones/cocones, universal properties (`IsLimit`), existence typeclasses (`HasLimits`), and functoriality, along with duality theory relating limits and colimits through opposite categories; (2) **Concrete shapes and constructions** providing specialized implementations for all standard diagram shapes (products, pullbacks, equalizers, kernels, biproducts, wide pullbacks, terminal objects, etc.) with convenient notation and APIs, theorems showing how complex limits can be built from simpler primitives (e.g., all limits from products and equalizers), and explicit constructions in the category of types serving as fundamental examples; (3) **Functorial properties and advanced theory** characterizing how functors interact with limits through preservation, reflection, and creation (`Preserves/`), computing limits in structured categories (functor categories compute limits pointwise via `FunctorCategory/`, concrete categories via `ConcreteCategory/`), and specialized topics including final/initial functors enabling limit computation along functors, filtered colimits and their interaction with finite limits, ind-objects and ind-completion (`Indization/`), van Kampen colimits for descent theory, and the density theorem showing presheaves as colimits of representables. Together with its eight subdirectories (`Shapes/` for specific limit shapes, `Types/` for explicit type-theoretic constructions, `Preserves/` for functorial properties, `FunctorCategory/` for pointwise limits, `Constructions/` for building complex limits from primitives, `ConcreteCategory/` for set-theoretic characterizations, `Final/` for final functor theory, and `Indization/` for ind-objects), this directory provides the complete infrastructure needed for categorical reasoning throughout mathlib, forming the foundation for adjunctions, completeness properties, sheaf theory, abelian categories, and higher categorical structures.

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

- [x] `ConcreteCategory/` - Set-theoretic characterizations of limits in concrete categories: limit extensionality (elements determined by projections), colimit element existence (elements from diagram components), filtered colimit equality via zigzags, and preservation of algebraic properties like zero-smul-divisor-freeness in module categories
- [x] `Constructions/` - Building complex limits from primitive ones: constructing all limits from products and equalizers, finite limits from binary products and equalizers, pullbacks from products, filtered/cofiltered limit constructions, limits in over categories, epimorphism/monomorphism preservation, and special cases with zero objects
- [x] `Final/` - Specialized theory of final and initial functors: characterization of connected categories via constant functors, parallel pair initiality conditions, and bijections on sections/colimit types induced by initial/final functors to Type
- [x] `FunctorCategory/` - Pointwise limits in functor categories: evaluation functors jointly reflect/preserve limits, `combineCones` stitches pointwise cones, characterization of preservation via pointwise evaluation, epimorphisms/monomorphisms determined componentwise, and instances for filtered/finite limits
- [x] `Indization/` - Complete theory of ind-objects and ind-completion: ind-objects as filtered colimits of representables, recognition theorems via costructured arrow categories, closure under filtered colimits and finite limits, construction of `Ind C` category with canonical functors, and fundamental theorems on limit/colimit existence (Kashiwara-Schapira)
- [x] `Preserves/` - Comprehensive theory of limit/colimit preservation by functors: core typeclasses (`PreservesLimit`, `PreservesColimit`, `PreservesLimitsOfShape`), `preservesLimitIso` for preserved limits, preservation by opposite/bifunctor/Yoneda/Grothendieck constructions, finite limit preservation (left exact functors), filtered colimit preservation (flat functors), shape-specific preservation equivalences, and limit creation theory
- [x] `Shapes/` - All standard limit shapes with dedicated APIs: terminal/initial objects, products/coproducts (binary and indexed), equalizers/coequalizers, pullbacks/pushouts with pasting lemmas, kernels/cokernels, biproducts with ⊞ notation, images and factorization systems, regular/strong epimorphisms and monomorphisms, zero objects/morphisms, wide pullbacks, multiequalizers, split equalizers, finite limits, transfinite compositions in preorders, and duality via opposite categories
- [x] `Types/` - Explicit constructions in category of types: limits as sections (dependent functions), colimits as quotients of sigma types, products as pi types, coproducts as sigma types, pullbacks as subtypes of products, pushouts as quotients, equalizers as subtypes, filtered colimits with equality characterization via existence of common extension, and Yoneda correspondences between cones/cocones and hom-functor limits

## Search Tags

limits colimits cones cocones universal-property limit-cone colimit-cocone has-limits completeness cocompleteness preserves-limits creates-limits final-functors filtered-colimits van-kampen density-theorem yoneda-lemma presheaves exact-functors fubini ind-objects representables
