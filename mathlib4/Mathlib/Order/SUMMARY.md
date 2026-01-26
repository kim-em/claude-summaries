---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order
generated: 2026-01-25T19:30:00Z
git_sha: ffb766c85c7ad82861131c2f10a0669884e4fd5f
git_branch: HEAD
status: preliminary
files_count: 88
subdirs_count: 27
---

# Order

## Overview

The `Order/` directory contains comprehensive formalization of order theory in a broad sense, implementing the foundational hierarchy from basic preorders through complete Boolean algebras. The directory includes extensive theory on partial orders, lattices (semi-, complete, modular, distributive), well-founded relations, ordinals via initial/principal segments, chains and antichains, Galois connections, filters, fixed points, and major theorems (Zorn's lemma, Jordan-Hölder, Knaster-Tarski). It also provides specialized topics including Krull dimension for algebraic geometry, omega-complete partial orders for programming language semantics, and various order-theoretic constructions (closure operators, nuclei, directed sets, supremum/infimum operations on sequences).

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

- [x] `Atoms/` - Atomic and coatomic structures
- [x] `BooleanAlgebra/` - Boolean algebra hierarchy
- [x] `BoundedOrder/` - Bounded orders with top and bottom
- [x] `Bounds/` - Bounds, suprema, and infima
- [x] `Category/` - Categorical structures for orders
- [x] `Circular/` - Circular order theory
- [x] `CompactlyGenerated/` - Compactly generated lattices
- [x] `CompleteLattice/` - Complete lattice theory
- [x] `ConditionallyCompleteLattice/` - Conditionally complete lattices
- [x] `Defs/` - Core definitions for order theory
- [x] `Extension/` - Order extensions
- [x] `Filter/` - Filter theory (partial orders of filters, filter bases, ultrafilters, Gödel's completeness theorem infrastructure)
- [x] `Fin/` - Orders on Fin types
- [x] `GaloisConnection/` - Galois connections and Galois insertions
- [x] `Heyting/` - Heyting algebras
- [x] `Hom/` - Order homomorphisms
- [x] `Interval/` - Intervals in orders
- [x] `Lattice/` - Lattice theory
- [x] `Monotone/` - Monotone and antitone functions
- [x] `Partition/` - Partitions and equivalence relations
- [x] `Preorder/` - Preorders, partial orders, linear orders
- [x] `Prod/` - Product orders
- [x] `Rel/` - Binary relations
- [x] `RelIso/` - Relation isomorphisms and embeddings
- [x] `ScottContinuity/` - Scott continuity theory
- [ ] `SuccPred/` - Successor and predecessor functions
- [ ] `UpperLower/` - Upper and lower sets

## Search Tags

order-theory partial-order preorder lattice semilattice complete-lattice Boolean-algebra frame coframe well-founded ordinal initial-segment antichain chain atoms coatoms modular-lattice distributive-lattice Galois-connection filter closure-operator fixed-point Zorn Jordan-Holder Krull-dimension omega-cpo monotone directed supremum infimum bounds covering-relation height well-quasi-order
