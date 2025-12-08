---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory
generated: 2025-12-08T00:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 57
subdirs_count: 57
---

# CategoryTheory

## Overview

The `CategoryTheory/` directory is the comprehensive formalization of category theory in mathlib4, spanning from foundational definitions through advanced specialized theories. At its core, it provides the basic language of categories (functors, natural transformations, isomorphisms, opposites) and fundamental universal constructions (limits/colimits, adjunctions, equivalences, Yoneda lemma). The implementation extends to enriched category theory (categories enriched over monoidal categories), monoidal structures (tensor products, braiding, rigidity, internal algebraic objects), and bicategories with higher-dimensional morphisms. Specialized categorical structures include abelian and preadditive categories (kernels, cokernels, exact sequences, injective/projective objects), triangulated categories (distinguished triangles, octahedron axiom, t-structures), presentable and accessible categories (κ-presentable objects, locally presentable categories), and Galois categories (fundamental groups). The directory also formalizes site theory and sheaves, topoi (both Grothendieck and elementary), fibered categories, localization of categories, lifting properties and weak factorization systems, and various special categories (groupoids, discrete/codiscrete, finite categories). This infrastructure serves as the mathematical backbone for algebraic geometry, algebraic topology, homological algebra, representation theory, and other areas throughout mathlib requiring categorical abstraction.

## Key Files

| File | Purpose |
|------|---------|
| NatTrans.lean | Natural transformations between functors with naturality squares and vertical/horizontal composition |
| Iso.lean | Isomorphisms in categories including bundled `Iso` structures and unbundled `IsIso` typeclass |
| Yoneda.lean | Yoneda embedding as functor `C ⥤ (Cᵒᵖ ⥤ Type v₁)` with proof it is fully faithful, plus Yoneda lemma |
| EpiMono.lean | Properties of epimorphisms and monomorphisms including behavior under opposites |
| Opposites.lean | Opposite category construction `Cᵒᵖ` with reversed morphisms and associated functors |
| Equivalence.lean | Equivalences of categories as half-adjoint equivalences with unit and counit |
| Whiskering.lean | Whiskering operations for composing natural transformations with functors |
| Adhesive.lean | Adhesive categories with van Kampen pushouts along monomorphisms |
| Grothendieck.lean | Grothendieck construction for functors `F : C ⥤ Cat` producing fibered categories |
| Elements.lean | Category of elements construction for functors `F : C ⥤ Type` |
| CommSq.lean | Commutative squares in categories with various structural properties |
| CatCommSq.lean | Commutative squares in the category Cat of categories |
| Balanced.lean | Balanced categories where monomorphisms that are epimorphisms are isomorphisms |
| Simple.lean | Simple objects in categories (no proper subobjects) |
| Skeletal.lean | Skeletal categories where isomorphic objects are equal |
| IsConnected.lean | Connected categories where there exists zigzag of morphisms between any two objects |
| EssentialImage.lean | Essential image of functors (objects isomorphic to image objects) |
| EssentiallySmall.lean | Essentially small categories equivalent to small categories |
| Extensive.lean | Extensive categories with well-behaved finite coproducts |
| ExtremalEpi.lean | Extremal epimorphisms (epis not factoring through proper monos) |
| GlueData.lean | Gluing data for constructing objects from covers |
| GradedObject.lean | Graded objects indexed by monoids or additive groups |
| HomCongr.lean | Homomorphism space isomorphisms induced by object isomorphisms |
| InducedCategory.lean | Category structure induced via a function on objects |
| FullSubcategory.lean | Full subcategory on objects satisfying a predicate |
| IsomorphismClasses.lean | Isomorphism classes of objects in a category |
| LocallyDirected.lean | Locally directed categories (directed on each hom-set) |
| Noetherian.lean | Noetherian objects (ascending chain condition on subobjects) |
| Core.lean | Core of a category (groupoid of isomorphisms) |
| Groupoid.lean | Groupoids where all morphisms are isomorphisms |
| Countable.lean | Countable categories with countable objects and morphisms |
| SingleObj.lean | Single-object category construction from a monoid |
| PUnit.lean | Category instance on PUnit (terminal category) |
| PEmpty.lean | Category instance on PEmpty (empty category) |
| FintypeCat.lean | Category of finite types with functions |
| CodiscreteCategory.lean | Codiscrete category with unique morphism between any two objects |
| CofilteredSystem.lean | Cofiltered systems and limits |
| Conj.lean | Conjugation by isomorphisms |
| ConnectedComponents.lean | Connected components of a category as a quotient |
| DifferentialObject.lean | Objects equipped with a differential (d² = 0) |
| DinatTrans.lean | Dinatural transformations between functors |
| Elementwise.lean | Tactic support for elementwise reasoning in categories |
| Endomorphism.lean | Endomorphism monoid of an object |
| Retract.lean | Retracts in categories (section-retraction pairs) |
| RepresentedBy.lean | Representable functors and their representing objects |
| Subterminal.lean | Subterminal objects (at most one morphism from any object) |
| Thin.lean | Thin categories (at most one morphism between any two objects) |
| UnivLE.lean | Universe level constraints for categories |
| Square.lean | Square diagrams and their properties |
| SmallRepresentatives.lean | Small representatives for essentially small categories |

## Subdirectories

- [x] `Abelian/` - Abelian categories with kernels, cokernels, and exact sequences
- [x] `Action/` - Group actions and representations as functors
- [x] `Adjunction/` - Adjoint functors with unit and counit
- [x] `Bicategory/` - Bicategories with 2-morphisms and coherence
- [x] `Category/` - Basic category instances and constructions
- [x] `Center/` - Center of categories as endomorphisms of identity functor
- [x] `ChosenFiniteProducts/` - Deprecated redirects to Monoidal.Cartesian.* modules
- [x] `Closed/` - Deprecated redirects to Monoidal.Closed modules
- [x] `Comma/` - Comma categories and slice categories
- [x] `ComposableArrows/` - Composable sequences of arrows
- [x] `ConcreteCategory/` - Concrete categories with underlying sets/types
- [x] `CopyDiscardCategory/` - Categories with copy and discard operations
- [x] `Dialectica/` - Dialectica categories
- [x] `Discrete/` - Discrete categories from types
- [x] `Distributive/` - Distributive categories with left/right tensor products preserving coproducts
- [x] `EffectiveEpi/` - Effective epimorphisms and descent
- [x] `Endofunctor/` - Endofunctors and fixed points
- [x] `Enriched/` - Enriched categories over monoidal categories with conical limits and compatibility with ordinary category structure
- [x] `Equivalence/` - Functoriality of equivalence operations including symmetry equivalence and inverse functor
- [x] `FiberedCategory/` - Fibered categories and Grothendieck fibrations
- [x] `Filtered/` - Filtered categories and directed colimits
- [x] `FinCategory/` - Finite categories with finitely many objects and morphisms, including equivalences to concrete Fin-indexed representations
- [x] `Functor/` - Functors and functor properties (fully faithful, conservative, etc.)
- [x] `Galois/` - Galois categories and fundamental groups
- [x] `Generator/` - Generators and separators in categories
- [x] `GradedObject/` - Additional graded object constructions
- [x] `Groupoid/` - Additional groupoid constructions
- [x] `GuitartExact/` - Guitart exact squares
- [x] `Idempotents/` - Idempotent completion and Karoubi envelope
- [x] `Join/` - Join of categories
- [x] `LiftingProperties/` - Lifting properties and weak factorization systems
- [x] `Limits/` - Limits and colimits (products, pullbacks, equalizers, etc.)
- [x] `Linear/` - Linear categories (enriched over modules)
- [x] `Localization/` - Localization of categories with respect to morphism properties
- [x] `LocallyCartesianClosed/` - Locally cartesian closed categories
- [x] `MarkovCategory/` - Markov categories for probability
- [x] `Monad/` - Monads and algebras
- [x] `Monoidal/` - Comprehensive monoidal category theory: tensor products, internal algebraic objects (monoid/comonoid/bimonoid/Hopf), braided/symmetric structures, closed monoidal categories, Cartesian monoidal categories, rigid categories with duals, Day convolution, free monoidal categories and coherence theorem, actions, limits, and transport mechanisms
- [x] `MorphismProperty/` - Properties of morphisms (stable, multiplicative, etc.)
- [x] `ObjectProperty/` - Properties of objects in categories
- [x] `PathCategory/` - Path category from a quiver
- [x] `Pi/` - Pointwise category structure on indexed families of objects
- [x] `Preadditive/` - Preadditive categories with additive hom-groups, injective/projective objects with resolutions, and specialized Yoneda embeddings
- [x] `Presentable/` - Presentable and accessible categories with κ-presentable objects, κ-accessible functors, locally presentable categories, cardinal-filtered categories, and orthogonal-reflection construction for reflective subcategories
- [x] `Products/` - Cartesian product categories with projection/section functors, swap equivalence, evaluation functors, associator and unitor coherence isomorphisms
- [x] `Quotient/` - Quotient categories with preadditive and linear structure preservation
- [x] `Shift/` - Shift functors and graded structures
- [x] `Sigma/` - Coproduct (sigma) categories
- [x] `Sites/` - Grothendieck topologies and sheaves
- [x] `SmallObject/` - Small object argument for factorization systems with transfinite iteration machinery
- [x] `Subobject/` - Subobject lattices
- [x] `Subpresheaf/` - Subpresheaves and sieves
- [x] `Sums/` - Coproduct constructions
- [x] `Topos/` - Topoi (elementary and Grothendieck)
- [x] `Triangulated/` - Triangulated categories with distinguished triangles, octahedron axiom, homological functors, opposite category structures, and t-structures with truncation functors
- [x] `Types/` - Category of types with function morphisms, correspondence between categorical and type-theoretic concepts (monos=injections, epis=surjections, isos=equivs), sections functor, universe lifting, and monomorphism stability properties
- [x] `WithTerminal/` - Freely adjoining terminal and initial objects to categories with universal properties, comma category equivalences, cone/cocone relations, and finiteness results

## Search Tags

category-theory categories functors natural-transformations limits colimits adjunctions equivalences monoidal-categories abelian-categories yoneda-lemma grothendieck-construction enriched-categories bicategories sites sheaves topoi triangulated-categories homological-algebra categorical-logic presheaves representable-functors
