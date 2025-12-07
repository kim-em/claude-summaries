---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory
generated: 2025-12-07T08:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 57
subdirs_count: 57
---

# CategoryTheory

## Overview

The `CategoryTheory/` directory contains the comprehensive formalization of category theory in mathlib4, providing the foundational infrastructure for categorical reasoning across mathematics. It implements the core categorical concepts (categories, functors, natural transformations, isomorphisms), fundamental constructions (opposites, products, limits, adjunctions, equivalences), specialized structures (abelian categories, monoidal categories, enriched categories, bicategories), and advanced topics (Yoneda lemma, Grothendieck construction, site theory, triangulated categories). This framework serves as the mathematical backbone for algebraic geometry, algebraic topology, homological algebra, and other areas of mathlib that benefit from categorical abstraction.

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

- [x] `Abelian/` - Abelian categories with kernels, cokernels, and exact sequences (complete)
- [x] `Action/` - Group actions and representations as functors (complete)
- [x] `Adjunction/` - Adjoint functors with unit and counit (complete)
- [x] `Bicategory/` - Bicategories with 2-morphisms and coherence (complete)
- [x] `Category/` - Basic category instances and constructions (complete)
- [x] `Center/` - Center of categories as endomorphisms of identity functor (complete)
- [ ] `ChosenFiniteProducts/` - Chosen finite products infrastructure (pending)
- [ ] `Closed/` - Closed categories with internal homs (pending)
- [ ] `Comma/` - Comma categories and slice categories (pending)
- [ ] `ComposableArrows/` - Composable sequences of arrows (pending)
- [ ] `ConcreteCategory/` - Concrete categories with underlying sets/types (pending)
- [ ] `CopyDiscardCategory/` - Categories with copy and discard operations (pending)
- [ ] `Dialectica/` - Dialectica categories (pending)
- [ ] `Discrete/` - Discrete categories from types (pending)
- [ ] `Distributive/` - Distributive categories (pending)
- [ ] `EffectiveEpi/` - Effective epimorphisms and descent (pending)
- [ ] `Endofunctor/` - Endofunctors and fixed points (pending)
- [ ] `Enriched/` - Enriched categories over monoidal categories (pending)
- [ ] `Equivalence/` - Additional equivalence constructions and properties (pending)
- [ ] `FiberedCategory/` - Fibered categories and Grothendieck fibrations (pending)
- [ ] `Filtered/` - Filtered categories and directed colimits (pending)
- [ ] `FinCategory/` - Finite categories (pending)
- [ ] `Functor/` - Functors and functor properties (fully faithful, conservative, etc.) (pending)
- [ ] `Galois/` - Galois categories and fundamental groups (pending)
- [ ] `Generator/` - Generators and separators in categories (pending)
- [ ] `GradedObject/` - Additional graded object constructions (pending)
- [ ] `Groupoid/` - Additional groupoid constructions (pending)
- [ ] `GuitartExact/` - Guitart exact squares (pending)
- [ ] `Idempotents/` - Idempotent completion and Karoubi envelope (pending)
- [ ] `Join/` - Join of categories (pending)
- [ ] `LiftingProperties/` - Lifting properties and weak factorization systems (pending)
- [ ] `Limits/` - Limits and colimits (products, pullbacks, equalizers, etc.) (pending)
- [ ] `Linear/` - Linear categories (enriched over modules) (pending)
- [ ] `Localization/` - Localization of categories (pending)
- [ ] `LocallyCartesianClosed/` - Locally cartesian closed categories (pending)
- [ ] `MarkovCategory/` - Markov categories for probability (pending)
- [ ] `Monad/` - Monads and algebras (pending)
- [ ] `Monoidal/` - Monoidal categories and tensor products (pending)
- [ ] `MorphismProperty/` - Properties of morphisms (stable, multiplicative, etc.) (pending)
- [ ] `ObjectProperty/` - Properties of objects in categories (pending)
- [ ] `PathCategory/` - Path category from a quiver (pending)
- [ ] `Pi/` - Product categories (pending)
- [ ] `Preadditive/` - Preadditive categories with additive hom-groups (pending)
- [ ] `Presentable/` - Presentable and accessible categories (pending)
- [ ] `Products/` - Product category constructions (pending)
- [ ] `Quotient/` - Quotient categories (pending)
- [ ] `Shift/` - Shift functors and graded structures (pending)
- [ ] `Sigma/` - Coproduct (sigma) categories (pending)
- [ ] `Sites/` - Grothendieck topologies and sheaves (pending)
- [ ] `SmallObject/` - Small object argument for factorization systems (pending)
- [ ] `Subobject/` - Subobject lattices (pending)
- [ ] `Subpresheaf/` - Subpresheaves and sieves (pending)
- [ ] `Sums/` - Coproduct constructions (pending)
- [ ] `Topos/` - Topoi (elementary and Grothendieck) (pending)
- [ ] `Triangulated/` - Triangulated categories (pending)
- [ ] `Types/` - Category of types (pending)
- [ ] `WithTerminal/` - Adding terminal objects to categories (pending)

## Search Tags

category-theory categories functors natural-transformations limits colimits adjunctions equivalences monoidal-categories abelian-categories yoneda-lemma grothendieck-construction enriched-categories bicategories sites sheaves topoi triangulated-categories homological-algebra categorical-logic presheaves representable-functors
