---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order
generated: 2026-01-27T00:00:00Z
git_sha: ffb766c85c7ad82861131c2f10a0669884e4fd5f
git_branch: HEAD
status: complete
files_count: 88
subdirs_count: 27
---

# Order

## Overview

The `Order/` directory provides the complete formalization of order theory in Mathlib, establishing the mathematical infrastructure for reasoning about ordered structures throughout the library. This directory spans the full hierarchy from basic preorders (reflexive transitive relations) through sophisticated structures like complete Boolean algebras and omega-complete partial orders, with applications ranging from topology and analysis to algebraic geometry and programming language semantics.

The directory is organized around several conceptual layers that build systematically: (1) **Foundational definitions** (`Defs/`, `Basic.lean`, `Lattice.lean`) establish the core typeclass hierarchy from preorders through partial orders, linear orders, semilattices, and lattices, with covering relations, minimal/maximal elements, and upper/lower sets. (2) **Completeness structures** (`CompleteLattice/`, `ConditionallyCompleteLattice/`, `CompleteBooleanAlgebra.lean`) provide suprema and infima for arbitrary sets (complete lattices), bounded sets (conditionally complete lattices), and frame structures for point-free topology. (3) **Morphisms and relationships** (`Hom/`, `RelIso/`, `GaloisConnection/`, `Monotone/`) formalize structure-preserving maps, order embeddings/isomorphisms, Galois connections as categorical adjoints, and monotonicity properties essential for functional analysis. (4) **Specialized order structures** (`BooleanAlgebra/`, `Heyting/`, `Atoms/`, `Bounds/`, `BoundedOrder/`) develop Boolean algebras for classical logic, Heyting algebras for intuitionistic logic, atomic lattices, and bounded orders with top/bottom elements.

Critical subdirectories extend the core theory with essential mathematical infrastructure: `Filter/` provides the foundation for topology and analysis through the complete formalization of filters (including atTop/atBot for limits at infinity, ultrafilters, filter bases, and germs); `Interval/` implements three representations of intervals (abstract objects, finite sets via `LocallyFiniteOrder`, infinite sets with ord-connectedness); `Category/` organizes all order structures into concrete categories from preorders through complete Boolean algebras (with `NonemptyFinLinOrd` as the standard simplicial index category); `SuccPred/` formalizes successor/predecessor operations with archimedean variants, proving linear locally finite orders are countable and order-isomorphic to subsets of ℤ; `UpperLower/` develops upper/lower set theory with closure operators; and `Extension/` proves any partial order extends to a linear order (Szpilrajn) and any well-founded order extends to a well-order.

The directory also includes advanced mathematical theories with specific applications: well-founded relations and ordinals via initial/principal segment embeddings (`WellFounded.lean`, `InitialSeg.lean`) provide the foundation for ordinal arithmetic; chains, antichains, and maximal chains (`Antichain.lean`, `Preorder/Chain.lean`) support Zorn's lemma and the Hausdorff maximality principle (`CompleteLattice/Chain.lean`, `Zorn.lean`); Galois connections and insertions enable lifting order structures between types; filters abstract limits and "eventual" behavior for topology, measure theory, and analysis; fixed-point theorems (Knaster-Tarski, Bourbaki-Witt) underpin inductive definitions; Jordan-Hölder theory on composition series applies to groups and modules; and Krull dimension provides the order-theoretic foundation for dimension theory in algebraic geometry.

## Key Files

| File | Purpose |
|------|---------|
| README.md | Documents order hierarchy structure split across Preorder/BooleanAlgebra/CompleteLattice/ConditionallyCompleteLattice subfolders; notes that content is still being organized into this structure |
| Basic.lean | Core definitions and results about `≤` and `<`: dot notation lemmas, OrderDual type synonym (`αᵒᵈ`), order transfer functions (Preorder.lift, PartialOrder.lift, LinearOrder.lift), DenselyOrdered class |
| Lattice.lean | Semilattices and lattices: SemilatticeSup/SemilatticeInf classes with join (`⊔`) and meet (`⊓`) operations, Lattice typeclass, DistribLattice for distributive lattices, alternative constructors via algebraic properties |
| CompleteBooleanAlgebra.lean | Frames and complete Boolean algebras: Order.Frame (complete lattice with `⊓` distributing over `⨆`), Order.Coframe, CompleteDistribLattice, CompleteBooleanAlgebra, CompletelyDistribLattice (with `iInf_iSup_eq`), CompleteAtomicBooleanAlgebra |
| CompleteLatticeIntervals.lean | Complete lattice structure on intervals in complete lattices |
| CompletePartialOrder.lean | Complete partial orders (CPOs) |
| CompleteSublattice.lean | Complete sublattices of complete lattices |
| WellFounded.lean | Well-founded relations: characterizations via descending chains, WellFounded.min/sup/succ operations, induction principles including WellFounded.induction_bot |
| WellFoundedSet.lean | Well-founded relations on sets; extensive API for well-foundedness on sets |
| InitialSeg.lean | Initial and principal segment embeddings: InitialSeg (`r ≼i s`), PrincipalSeg (`r ≺i s`), order embeddings whose range is a lower set or principal lower set; corresponds to `≤` and `<` on ordinals |
| Antichain.lean | Antichains: IsAntichain (pairwise unrelated elements), IsStrongAntichain, IsMaxAntichain; generalizes incomparable sets and independent sets in graphs |
| Atoms.lean | Atoms and coatoms in orders: IsAtom, IsCoatom, IsAtomic, IsCoatomic, atomistic and coatomistic lattices |
| BooleanGenerators.lean | Boolean algebra generators |
| BooleanSubalgebra.lean | Boolean subalgebras |
| Booleanisation.lean | Booleanisation construction for lattices |
| Bounded.lean | Bounded orders with top and bottom elements |
| BourbakiWitt.lean | Bourbaki-Witt fixed point theorem |
| Birkhoff.lean | Birkhoff's variety theorem |
| Circular.lean | Circular orders (ternary betweenness relation) |
| Closure.lean | Closure operators: Galois insertion framework for closure operations |
| Cofinal.lean | Cofinal sets and functions |
| Comparable.lean | Comparability of elements in orders |
| Compare.lean | Comparison trichotomy for linear orders |
| Concept.lean | Formal concept analysis |
| Copy.lean | Copying order structures via equivalences |
| CountableDenseLinearOrder.lean | Countable dense linear orders without endpoints (Cantor's theorem on uniqueness) |
| Cover.lean | Covering relations: `a ⋖ b` means `a < b` with nothing between; wcovBy (weakly covers) for preorders |
| Directed.lean | Directed sets and directed orders |
| DirectedInverseSystem.lean | Directed inverse systems |
| Disjoint.lean | Disjointness in semilattices: `Disjoint a b` means `a ⊓ b = ⊥` |
| Disjointed.lean | Disjointed sequences (making sequences pairwise disjoint) |
| FixedPoints.lean | Fixed points of monotone functions |
| GameAdd.lean | Game addition on orders |
| Grade.lean | Graded orders (orders with rank function) |
| Height.lean | Height of elements in orders |
| Ideal.lean | Order ideals (downward-closed sets closed under suprema) |
| Irreducible.lean | Irreducible elements in orders |
| IsNormal.lean | Normal functions on ordinals |
| Iterate.lean | Iteration of monotone functions |
| JordanHolder.lean | Jordan-Hölder theorem: for JordanHolderLattice, composition series with same endpoints are equivalent; includes CompositionSeries type and Iso relation |
| KonigLemma.lean | König's lemma for infinite trees |
| KrullDimension.lean | Krull dimension of preordered sets: supremum of lengths of chains, height and coheight of elements; used in algebraic geometry for dimension of varieties and rings |
| LatticeIntervals.lean | Lattice structure on intervals |
| LiminfLimsup.lean | Liminf and limsup for filters and sequences: limit inferior and limit superior via bounded lattice operations |
| Max.lean | Maximum elements in orders |
| MinMax.lean | Minimum and maximum operations |
| Minimal.lean | Minimal and maximal elements |
| ModularLattice.lean | Modular lattices: IsModularLattice (satisfies `a ≤ c → (a ⊔ b) ⊓ c = a ⊔ (b ⊓ c)`), IsWeakUpperModularLattice, IsWeakLowerModularLattice, infIccOrderIsoIccSup (diamond isomorphism) |
| Nat.lean | Natural number order instances |
| Notation.lean | Order notation and syntax |
| Nucleus.lean | Nuclei on frames (closure operators for frames) |
| OmegaCompletePartialOrder.lean | Omega-complete partial orders (ωCPO): partial orders with suprema of ω-chains; used for programming language semantics to define recursive procedures; includes continuous morphisms (ContinuousHom, notation →𝒄) |
| OrdContinuous.lean | Order-continuous functions |
| OrderIsoNat.lean | Order isomorphisms with natural numbers |
| PFilter.lean | Prime filters |
| Part.lean | Order on Part (partial values) |
| PartialSups.lean | Partial suprema of sequences |
| PiLex.lean | Lexicographic order on Pi types |
| PrimeIdeal.lean | Prime ideals in orders |
| PrimeSeparator.lean | Prime separators in orders |
| PropInstances.lean | Order instances for Prop |
| Quotient.lean | Quotient orders |
| Radical.lean | Radical of sets in orders |
| RelClasses.lean | Relation classes: reflexive, transitive, symmetric, antisymmetric, etc. |
| RelSeries.lean | Relation series: chains of related elements, LTSeries, LEseries; used for composition series and Krull dimension |
| Restriction.lean | Restriction of orders to subtypes |
| SaddlePoint.lean | Saddle points in orders |
| ScottContinuity.lean | Scott-continuous functions |
| SemiconjSup.lean | Semiconjugacy for supremum operations |
| Set.lean | Order on sets via inclusion |
| SetIsMax.lean | Maximum sets in orders |
| SetNotation.lean | Set-builder notation for order theory |
| Shrink.lean | Universe shrinking for small sets |
| Sublattice.lean | Sublattices of lattices |
| Sublocale.lean | Sublocales (subframes of frames) |
| SupClosed.lean | Sup-closed sets (closed under suprema) |
| SupIndep.lean | Supremum independence (generalization of linear independence to lattices) |
| SymmDiff.lean | Symmetric difference in Boolean algebras |
| Synonym.lean | Type synonyms for orders |
| TeichmullerTukey.lean | Teichmüller-Tukey lemma |
| TransfiniteIteration.lean | Transfinite iteration of functions |
| TypeTags.lean | Type tags for different order interpretations |
| ULift.lean | Order on ULift (universe lifting) |
| WellQuasiOrder.lean | Well-quasi-orders (WQO): reflexive transitive relations where every infinite sequence has an increasing pair |
| WithBot.lean | Adding a bottom element to orders: WithBot type, order instances, lattice operations, completeness |
| Zorn.lean | Zorn's lemma: exists_maximal_of_chains_bounded and variants (zorn_le, zorn_subset, zorn_superset, with ₀ and _nonempty modifiers) |
| ZornAtoms.lean | Zorn's lemma for atomic orders |

## Subdirectories

- [x] `Atoms/` - Finiteness-specific theory: finite partial orders with boundaries are automatically atomic/coatomic, simple orders are finite, locally finite orders are strongly atomic/coatomic
- [x] `BooleanAlgebra/` - Boolean algebra typeclasses and core API: generalized Boolean algebras (distributive lattices with relative complement `\`), full Boolean algebras (with absolute complement `ᶜ`), De Morgan laws, Heyting implication, and concrete instance for `Set α`
- [x] `BoundedOrder/` - Bounded order theory: `OrderTop`/`OrderBot`/`BoundedOrder` typeclasses for orders with greatest/least elements, fundamental lemmas (top_unique, bot_le, le_top), bounded lattice operations, monotonicity characterizations on bounded orders
- [x] `Bounds/` - Upper/lower bounds for sets: core predicates (`BddAbove`/`BddBelow`, `IsLeast`/`IsGreatest`, `IsLUB`/`IsGLB`), cofinality, behavior under monotone/antitone functions, images, products, unions, and order isomorphisms—foundational infrastructure for analysis and lattice theory
- [x] `Category/` - Concrete categories for order structures: systematically organizes preorders, partial orders, linear orders, lattices, bounded lattices, distributive lattices, Boolean algebras, Heyting algebras, frames, complete lattices, and ωCPO into categories; includes `NonemptyFinLinOrd` as standard simplicial index category
- [x] `Circular/` - Circular order instances: provides `CircularOrder` for `ZMod n`, `Fin n`, and `ℤ` derived from linear orders using "loop around" construction
- [x] `CompactlyGenerated/` - Compactly generated complete lattices: defines compact elements, proves equivalence of four well-foundedness characterizations, establishes compactly generated modular lattices are complemented iff atomistic, includes interval-specific compactness results
- [x] `CompleteLattice/` - Complete lattice core theory: typeclasses (`CompleteLattice`, `CompleteLinearOrder`), `sSup`/`sInf`/`iSup`/`iInf` operations, Hausdorff's maximality principle, finset-indexed operations, group-compatible lattice operations, lexicographic Pi types, SetLike sublattices, bicartesian squares for category theory
- [x] `ConditionallyCompleteLattice/` - Conditionally complete lattices (suprema/infima for nonempty bounded sets): core typeclasses, `csSup`/`csInf` theory with boundedness assumptions, indexed variants (`ciSup`/`ciInf`), extensions to `WithTop`/`WithBot`, connections to finsets and group operations—canonical examples are ℝ, ℕ, ℤ
- [x] `Defs/` - Foundational order definitions: unbundled relation classes (reflexive, transitive, antisymmetric), core typeclasses (`Preorder`, `PartialOrder`, `LinearOrder`), covering relations (`⋖`, `⩿`), minimal/maximal elements, upper/lower sets, decidability, min/max operations
- [x] `Extension/` - Order extension theorems: Szpilrajn extension (partial order → linear order via Zorn's lemma), well-order extension (well-founded → well-order via ordinal rank and lexicographic product)
- [x] `Filter/` - Complete filter theory foundation: filter structure as complete lattice, map/comap Galois connection, monad structure, Tendsto for convergence, NeBot for non-triviality, specialized filters (atTop/atBot with 19-file arithmetic preservation, cofinite, ultrafilters, bases, germs), pointwise operations, boundedness, extrema, products—abstracts limits and "eventual" behavior for topology/measure/analysis
- [x] `Fin/` - Order structures on `Fin n`: bounded linear order, extensive order embeddings/isomorphisms (cast, succ, rev, succAbove), monotonicity results, finset order isomorphisms (orderIsoSingleton, orderIsoPair, orderIsoTriple), tuple ordering (pi_lex, cons/snoc/insertNth isomorphisms)
- [x] `GaloisConnection/` - Galois connections as order-theoretic adjoints: core definitions (`GaloisConnection`, `GaloisInsertion`, `GaloisCoinsertion`), monotonicity and uniqueness, operations on bounds/suprema/infima, lifting order structures (semilattices, lattices, complete lattices) via Galois insertions with choice functions
- [x] `Heyting/` - Heyting algebras (intuitionistic logic model): (co-/bi-)Heyting algebra typeclasses with implication `⇨` and difference `\`, co-Heyting boundary operator (topological boundary), homomorphisms (`HeytingHom`, `CoheytingHom`, `BiheytingHom`), proof that regular elements (satisfying `aᶜᶜ = a`) form a Boolean algebra enabling classical reasoning within intuitionistic logic
- [x] `Hom/` - Bundled order morphisms: `OrderHom` (monotone maps), `OrderEmbedding`, `OrderIso`, lattice homomorphisms (`SupHom`, `InfHom`, `LatticeHom`, `BoundedLatticeHom`), complete lattice homomorphisms (`sSupHom`, `sInfHom`, `FrameHom`, `CompleteLatticeHom`), complete lattice structure on `α →o β`, set-theoretic constructions, lexicographic order, `WithTop`/`WithBot` extensions
- [x] `Interval/` - Three-layer interval formalization: abstract interval objects with lattice operations and lexicographic ordering (`Basic.lean`, `Lex.lean`), finite set intervals via `LocallyFiniteOrder` (`Finset/` proving linear locally finite orders aren't densely ordered, successor interval relations, box decomposition), infinite set intervals with `OrdConnected` typeclass and comprehensive theory (`Set/` with 25 files covering all interval notations, unordered intervals, interactions with monotone functions/projections/type constructors)
- [x] `Lattice/` - Lattice congruence relations: `LatticeCon` structure (equivalence relations compatible with `⊓` and `⊔`), alternative simplified constructor, kernel of lattice homomorphism as congruence
- [x] `Monotone/` - Monotonicity theory: core definitions (`Monotone`, `Antitone`, `StrictMono`, `StrictAnti` with "On" variants), comprehensive API (dual transformations, well-foundedness, linear order reflection, products, Pi types), monotone extension theorem, monovariance (functions varying together without requiring ordered index), odd function monotonicity, union-based monotonicity
- [x] `Partition/` - Partitions in complete lattices and finsets: general partitions as independent families with given supremum, finite partitions (`Finpartition`) with refinement order and bind operations, equipartitions (parts of nearly equal size for Szemerédi regularity), connections to equivalence relations
- [x] `Preorder/` - Specialized preorder theory: chains and flags (comparable element sets, maximal chains, `IsChain`, `Flag` type with SuccChain construction—ported from Isabelle/HOL Zorn theory), finiteness results (minimal/maximal element existence in finite sets), pointwise order on finitely supported functions (`Finsupp`)
- [x] `Prod/` - Product order structures: focuses on lexicographic products (ordering first by first component, then second); `Lex/` subdirectory contains order homomorphisms converting between standard and lexicographic products
- [x] `Rel/` - Relations and Galois connections: constructs Galois connection between power sets from arbitrary binary relation, proves `leftDual`/`rightDual` operations form adjoint functions with inverse bijections between fixed points—applications to topos theory and categorical logic
- [x] `RelIso/` - Relation morphisms foundation: `RelHom` (→r, one-directional preservation), `RelEmbedding` (↪r, injective bidirectional preservation), `RelIso` (≃r, bijective bidirectional preservation); includes composition, identity, dual, constructors, preservation of relation properties, lexicographic sum/product embeddings/isomorphisms, subrelation embeddings, directed/well-foundedness preservation
- [x] `ScottContinuity/` - Scott continuity from domain theory: characterization via supremum preservation on directed sets (`scottContinuous_iff_map_sSup`), Scott continuity of meet in complete linear orders, product space Scott continuity
- [x] `SuccPred/` - Successor/predecessor operations: `SuccOrder`/`PredOrder` typeclasses with comprehensive API, archimedean variants (iterating succ/pred reaches all comparable elements), successor/predecessor limits, proves linear locally finite orders are countable and order-isomorphic to ℤ/ℕ/finite subsets, suprema/infima relations in complete linear orders, interval decompositions, closure properties for relations, initial segment preservation, rooted tree applications, `WithBot`/`WithTop` extensions
- [x] `UpperLower/` - Upper/lower set theory: unbundled predicates (`IsUpperSet`, `IsLowerSet`) and bundled types (`UpperSet`, `LowerSet` ordered by reverse inclusion matching filter convention), complete lattice and completely distributive lattice structures, principal sets (`Ici`, `Iic`, `Ioi`, `Iio`), upper/lower closure operators with Galois connections, set difference operations, products, complementation isomorphism, fibration characterizations, finiteness in locally finite orders, relative upper/lower sets

## Search Tags

order-theory partial-order preorder lattice semilattice complete-lattice Boolean-algebra frame coframe well-founded ordinal initial-segment antichain chain atoms coatoms modular-lattice distributive-lattice Galois-connection filter closure-operator fixed-point Zorn Jordan-Holder Krull-dimension omega-cpo monotone directed supremum infimum bounds covering-relation height well-quasi-order
