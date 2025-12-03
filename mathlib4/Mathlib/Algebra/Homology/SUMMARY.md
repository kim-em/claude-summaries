---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Homology
generated: 2025-12-02T12:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 42
subdirs_count: 6
---

# Homology

## Overview

The `Homology/` directory provides a complete and rigorous framework for homological algebra in mathlib4, systematically developing the theory from foundational building blocks to sophisticated derived category constructions. The framework begins with `ShortComplex/` providing three-object diagrams `X₁ → X₂ → X₃` with dual left/right homology data, exactness characterizations, and the snake lemma, serving as the atomic unit of homological reasoning. Building on this foundation, the root directory defines general `HomologicalComplex` structures with arbitrary index types and complex shapes, implements chain homotopies and quasi-isomorphisms, and develops bifunctors, total complexes, and double complex theory. The `Embedding/` subdirectory provides essential technical infrastructure for relating complexes via injective index maps, enabling extension/restriction functors and canonical truncations with homological preservation. The `HomotopyCategory/` subdirectory constructs the homotopy category by identifying homotopic maps, establishing its pretriangulated and triangulated structure via mapping cones following Verdier's formalism, and proving homological functor properties. The `DerivedCategory/` subdirectory implements the derived category as localization at quasi-isomorphisms with complete triangulated structure, homology functors forming shift sequences with long exact sequences, calculus of fractions, canonical t-structure, and Ext groups. Supporting infrastructure includes `LeftResolution/` for functorial projective resolutions via iterative kernel constructions, and `Factorizations/` for model category axioms proving morphism factorizations essential for identifying derived categories with homotopy categories of injective complexes. The entire framework supports both abstract categorical reasoning and concrete computational applications in abelian categories.

## Key Files

| File | Purpose |
|------|---------|
| ComplexShape.lean | Defines `ComplexShape ι` structure describing shapes of homological complexes indexed by type `ι`, with relation `Rel : ι → ι → Prop` controlling where differentials are allowed; includes `up` (cohomology) and `down` (homology) standard shapes |
| HomologicalComplex.lean | Core definition of `HomologicalComplex V c` with chain groups `X i`, differentials `d i j` satisfying `d ≫ d = 0`, category structure with chain maps, and fundamental constructions (`ChainComplex`, `CochainComplex`, `xNext`, `xPrev`, `dFrom`, `dTo`) |
| ExactSequence.lean | Exact sequences for `ComposableArrows C n` functors, with `IsComplex` (consecutive compositions zero) and `Exact` (exactness at each degree) properties, including short complexes and inductive constructions |
| Homotopy.lean | Chain homotopies between chain maps: `Homotopy f g` consists of components `h i j : C.X i ⟶ D.X j` satisfying homotopy condition `f = dNext h + prevD h + g`, proving homotopic maps induce same homology maps |
| QuasiIso.lean | Quasi-isomorphisms: morphisms inducing isomorphisms on homology via `QuasiIsoAt f i` (isomorphism at degree `i`) and `QuasiIso f` (isomorphism at all degrees), with equivalences to exactness conditions |
| Single.lean | Functor `single V j c : V ⥤ HomologicalComplex V c` constructing complexes supported in single degree `j`, with characterization of chain maps to single-degree complexes |
| HomotopyCategory.lean | Homotopy category construction where homotopic chain maps are identified, quotient by homotopy equivalence relation |
| Bifunctor.lean | Bifunctors on homological complexes, producing new complexes from pairs of complexes |
| BifunctorAssociator.lean | Associativity natural isomorphisms for bifunctors on homological complexes (large file, 44KB) |
| TotalComplex.lean | Total complex construction from bicomplexes, direct sum totalization for double complexes |
| TotalComplexShift.lean | Shift operations on total complexes with sign conventions for differential grading |
| HomologySequence.lean | Long exact sequences in homology induced by short exact sequences of complexes |
| HomologySequenceLemmas.lean | Technical lemmas supporting homology sequence constructions |
| ImageToKernel.lean | Relationship between image and kernel in homological complexes for exactness |
| Localization.lean | Localization of categories of homological complexes at quasi-isomorphisms |
| LocalCohomology.lean | Local cohomology functors and their properties |
| Double.lean | Double complexes (bicomplexes) with two anticommuting differentials |
| HomologicalBicomplex.lean | Homological properties of bicomplexes |
| Monoidal.lean | Monoidal structure on categories of homological complexes |
| Additive.lean | Additive structure on homological complexes and chain maps |
| Linear.lean | Linear/module structure on homological complex categories |
| Opposite.lean | Opposite complexes (reversing direction of differentials) |
| DifferentialObject.lean | Objects with a single differential satisfying `d ≫ d = 0` (degree 0 complexes) |
| Functor.lean | Functoriality of homological complex constructions |
| ConcreteCategory.lean | Concrete category structure for homological complexes |
| GrothendieckAbelian.lean | Grothendieck abelian category properties for homological complexes |
| HasNoLoop.lean | Complexes with no loops in their shape structure |
| CommSq.lean | Commutative squares in homological algebra |
| Square.lean | Square diagrams and their properties |
| Refinements.lean | Refinements of homological complex structures |
| ComplexShapeSigns.lean | Sign conventions for complex shapes (Koszul sign rule) |
| AlternatingConst.lean | Alternating constructions for homological complexes |
| Augment.lean | Augmentation maps and augmented complexes |
| BifunctorFlip.lean | Symmetry isomorphisms for bifunctors |
| BifunctorHomotopy.lean | Homotopy theory for bifunctors on complexes |
| BifunctorShift.lean | Shift operations for bifunctors |
| SingleHomology.lean | Homology of single-degree complexes |
| TotalComplexSymmetry.lean | Symmetry properties of total complex construction |
| HomotopyCofiber.lean | Homotopy cofiber constructions (mapping cones) |

## Subdirectories

- [x] `ShortComplex/` - Short complexes (composable pairs of morphisms): fundamental building blocks for homological algebra with three objects `X₁ → X₂ → X₃`, dual left/right homology data providing compatible descriptions via isomorphism, exactness characterizations (vanishing homology), snake lemma extracting long exact sequences from commutative ladders, and specialized theories for preadditive (additive homology functors) and abelian categories (canonical homology from coimage-image constructions)
- [x] `DerivedCategory/` - Derived categories: localization at quasi-isomorphisms producing `DerivedCategory C` as triangulated category with shift functors and distinguished triangles, homology functors forming shift sequences with connecting homomorphisms and long exact sequences, exact functors inducing triangulated functors, calculus of left/right fractions for morphism factorizations, canonical t-structure with truncation triangles, fully faithful single functors embedding abelian categories, and Ext groups as universe-polymorphic small shifted hom-types with long exact sequences and concrete computations via resolutions
- [x] `HomotopyCategory/` - Homotopy category of chain complexes: quotient by homotopy equivalence relation identifying homotopic chain maps, pretriangulated and triangulated structure via mapping cone constructions following Verdier's formalism with Conrad's sign conventions, shift functors with differential sign rules, homological functor property proven via degreewise split sequences in abelian categories, K-injective complexes for deriving contravariant functors, and single functors embedding objects as concentrated complexes with shift compatibility
- [x] `Embedding/` - Complex shape embeddings: injective maps `f : ι → ι'` preserving differential relations enabling index type transformations, extension functors padding with zeros outside image, restriction functors projecting onto image (requires `IsRelIff`), canonical ≥-truncation functors replacing below-range entries with opcycles (cokernels) producing epimorphisms `πTruncGE`, dual ≤-truncation functors using cycles (kernels) producing monomorphisms `ιTruncLE`, complementary embeddings partitioning target index sets with quasi-isomorphism connections, and connecting morphisms gluing chain/cochain complexes into ℤ-indexed complexes with homology preservation
- [x] `LeftResolution/` - Left resolutions (projective resolutions): functorial construction via `LeftResolution ι` structure containing functor `F : A ⥤ C` with natural epimorphisms `π : ι ∘ F ⟹ id`, iterative chain complex construction `chainComplexFunctor : A ⥤ ChainComplex C ℕ` building resolutions via kernel sequences with exactness proofs, extensions to idempotent completions via Karoubi envelopes ensuring zero morphism preservation for deriving functors on complexes, and transport along category equivalences for moving resolutions between equivalent settings
- [x] `Factorizations/` - Factorization lemmas for model category structure: defines `degreewiseEpiWithInjectiveKernel` morphism property as fibration class (multiplicative, closed under composition), proves CM5b factorization axiom for bounded below cochain complexes in abelian categories with enough injectives showing any morphism factors as monomorphism followed by trivial fibration (quasi-isomorphism with degreewise injective kernel), constructs factorization via auxiliary complex with zero differentials and injective objects using mapping cone and biproduct techniques, essential for identifying bounded below derived category with homotopy category of injective complexes enabling total derived functor construction

## Search Tags

homological-algebra chain-complex cochain-complex homology cohomology exact-sequence homotopy quasi-isomorphism derived-category spectral-sequence double-complex total-complex differential-graded snake-lemma five-lemma long-exact-sequence short-exact-sequence triangulated-category localization projective-resolution