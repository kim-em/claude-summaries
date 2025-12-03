---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group
generated: 2025-12-01T05:57:05Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 31
subdirs_count: 19
---

# Group

## Overview

The `Group/` directory constitutes the foundational layer of mathlib4's algebraic hierarchy, providing the complete formalization of group-like structures—semigroups, monoids, and groups—along with their extensive supporting theory. This directory serves as the critical bridge between the bare notation layer (`Algebra/Notation/`) and higher algebraic structures like rings and modules, establishing the fundamental concepts that permeate all of abstract algebra. At its core, `Defs.lean` defines the essential typeclass hierarchy (`Semigroup`, `Monoid`, `Group`, and their additive and commutative variants) with cancellation properties, while `Basic.lean` builds a comprehensive lemma library providing the basic properties, automation infrastructure, and computational tools needed throughout mathlib.

Beyond these fundamental definitions, the directory encompasses a rich ecosystem of group-theoretic concepts organized into specialized files and subdirectories. The `Hom/` subdirectory defines the complete theory of bundled homomorphisms (`MulHom`, `MonoidHom`, `AddMonoidHom`) and their typeclass hierarchy, providing the morphisms that connect algebraic structures. The `Equiv/` subdirectory establishes multiplicative and additive equivalences (`MulEquiv`, `AddEquiv`) as the proper notion of isomorphism for group-like structures. Three nested subdirectories define the substructure hierarchy: `Subsemigroup/` (sets closed under multiplication), `Submonoid/` (adding identity closure), and `Subgroup/` (adding inverse closure), each equipped with complete lattice structures, Galois insertions for closure operators, and extensive mapping theory.

The directory also develops crucial supporting concepts: group actions (`Action/` subdirectory with `MulAction` and `DistribMulAction` typeclasses), commuting elements (`Commute/` with the predicate `a * b = b * a`), semiconjugation (`Semiconj/` with `SemiconjBy a x y` meaning `a * x = y * a`), conjugation and centralizers (`Conj.lean`, `Center.lean`), units and invertible elements (`Units/`, `Invertible/`), endomorphisms and automorphisms (`End.lean`, `Action/End.lean`), and pointwise operations on sets (`Pointwise/` subdirectory enabling set-theoretic algebra). Specialized constructions include product groups (`Prod.lean`), opposite groups (`Opposite.lean`), pi types and dependent functions (`Pi/`), type tags for additive/multiplicative duality (`TypeTags/`), and the `WithOne/` construction adjoining a unit to semigroups.

The directory provides extensive theory for specific algebraic objects including the integers (`Int/`), natural numbers (`Nat/`), finite types (`Fin/`), commutators (`Commutator.lean`), additive characters (`AddChar.lean`), torsion elements (`Torsion.lean`), even elements (`Even.lean`), irreducible elements (`Irreducible/`), and unique products (`UniqueProds/`). All definitions systematically support both multiplicative and additive presentations through Lean's `@[to_additive]` attribute, ensuring unified development without code duplication. This directory forms the theoretical bedrock upon which mathlib's entire algebraic hierarchy is constructed, providing the definitions, lemmas, and infrastructure that enable formalization of ring theory, module theory, field theory, and beyond.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core typeclass definitions for semigroups, monoids, and groups with cancellation properties; defines `Semigroup`, `Monoid`, `Group`, `CommGroup`, and their additive variants, along with `IsLeftCancelMul`, `IsRightCancelMul`, and `IsCancelMul` mixins |
| Basic.lean | Comprehensive lemma library proving basic properties of semigroups, monoids, and groups; includes lemmas for associativity, identity elements, inverses, powers, and proof automation via `simp` and `to_additive` |
| InjSurj.lean | Lifting algebraic structures along injective/surjective maps; provides `Function.Injective.group` and `Function.Surjective.group` to transfer group structures via structure-preserving functions |
| End.lean | Endomorphism monoid `Function.End α` and `Monoid.End M`; automorphism group `Equiv.Perm α` and `MulAut M`; defines monoid structure on endomorphisms and group structure on automorphisms |
| AddChar.lean | Additive characters (homomorphisms from additive to multiplicative monoids); defines `AddChar A M` structure with dual additive/multiplicative group operations and includes ring-specific constructions like `mulShift` |
| Center.lean | Center and centralizer definitions; defines `Set.center`, `Set.centralizer`, `IsMulCentral`, and `IsAddCentral` for elements that commute with all others |
| Commutator.lean | Commutator bracket `⁅g₁, g₂⁆ = g₁ * g₂ * g₁⁻¹ * g₂⁻¹` for group elements |
| Conj.lean | Conjugation operations and conjugacy classes in groups |
| ConjFinite.lean | Finiteness properties of conjugacy classes |
| Prod.lean | Product constructions for groups; group structures on `α × β` given group structures on `α` and `β` |
| Opposite.lean | Opposite groups (reversing multiplication order) |
| Embedding.lean | Group embeddings as injective homomorphisms |
| Even.lean | Even and odd elements in groups (powers of squares) |
| EvenFunction.lean | Even and odd functions on groups |
| Ext.lean | Extensionality principles for group equality |
| Finsupp.lean | Group structures on finitely-supported functions |
| ForwardDiff.lean | Forward difference operators on groups |
| Graph.lean | Graph of a group homomorphism as a subgroup |
| Ideal.lean | Ideals in non-commutative groups (normal subgroups generated by sets) |
| Idempotent.lean | Idempotent elements in monoids |
| Indicator.lean | Indicator functions with group structures |
| MinimalAxioms.lean | Minimal axiom systems for defining groups |
| NatPowAssoc.lean | Natural power associativity and commutativity |
| PNatPowAssoc.lean | Positive natural power associativity |
| PUnit.lean | Group instances for the unit type |
| Shrink.lean | Type equivalences preserving group structure for shrinking universes |
| Support.lean | Support of functions with group codomains |
| Torsion.lean | Torsion elements (elements of finite order) in groups |
| TransferInstance.lean | Transferring group instances across type equivalences |
| Translate.lean | Left and right translation maps in groups |
| ULift.lean | Group instances for universe-lifted types |

## Subdirectories

- [x] `Action/` - Group actions on types with MulAction and DistribMulAction typeclasses, faithful and pretransitive actions, action homomorphisms, connections to endomorphisms and automorphisms, equidecomposition theory, and pointwise actions on sets and finsets
- [x] `Commute/` - Theory of commuting elements with predicate a * b = b * a, implemented as special case of semiconjugation; includes operations on commuting pairs, division monoid lemmas, homomorphism preservation, and units theory
- [x] `Equiv/` - Multiplicative and additive equivalences (MulEquiv, AddEquiv) as the proper notion of isomorphism; bundled equivalences with composition, inversion, opposite groups, type tag conversions, and decidability for finite types
- [x] `Fin/` - Algebraic group structures for finite types Fin n, establishing additive commutative group instances with comprehensive theory for addition, subtraction, negation, and tuple operations
- [x] `Hom/` - Complete theory of bundled homomorphisms (ZeroHom, OneHom, AddHom, MulHom, AddMonoidHom, MonoidHom) with typeclass hierarchies, composition, pointwise operations, algebraic instances on homomorphism spaces, ring structure on endomorphism monoids, and composition tracking typeclasses
- [x] `Int/` - Integer-specific group constructions: additive commutative group and multiplicative commutative monoid instances, parity theory, units characterization (exactly ±1), and Multiplicative ℤ type tag utilities
- [x] `Invertible/` - Type-valued Invertible typeclass for elements with two-sided multiplicative inverses (notation ⅟a), enabling computations with inverses in contexts where not all elements are invertible; bidirectional connection with units
- [x] `Irreducible/` - Irreducible elements in monoids (non-units that cannot factor as products of two non-units), generalizing irreducibility from ring theory; preservation under units multiplication and multiplicative equivalences
- [x] `Nat/` - Natural number group theory: additive and multiplicative commutative monoid instances, parity and evenness decidability, homomorphism characterization via behavior on 1, uniqueness of units (only 1 is multiplicative unit)
- [x] `Pi/` - Pointwise group structures on dependent function types (pi types) with typeclass instances showing product types inherit algebraic structures; homomorphism lifting, Pi.mulSingle for single-component updates, and fundamental equivalence between units in products and products of units
- [x] `Pointwise/` - Comprehensive theory of pointwise algebraic operations on sets (Set) and finite sets (Finset), enabling set-theoretic computations with group operations; includes algebraic instances, big operators, finiteness analysis, cardinality, lattice properties, density preservation, and interval arithmetic
- [x] `Semiconj/` - Semiconjugation relation SemiconjBy a x y meaning a * x = y * a, generalizing both commuting elements and conjugation; includes operations for semigroups, monoids, and groups, integer powers, and units theory
- [x] `Subgroup/` - Complete theory of subgroups as bundled sets closed under identity, multiplication, and inverses; complete lattice structure with closure operators and Galois insertions, image and preimage under homomorphisms, kernels and ranges, normal subgroups and normalizers, pointwise operations, and ZPowers sub-subdirectory for cyclic subgroups
- [x] `Submonoid/` - Complete theory of submonoids (sets closed under identity and multiplication) with bundled Submonoid type; complete lattice structure with closure as Galois insertion, operations (map, comap, products), membership criteria via big operators and directed suprema, pointwise operations, units theory, opposite monoids
- [x] `Subsemigroup/` - Foundational theory of subsemigroups (sets closed under multiplication, the minimal substructure) as the first layer in the algebraic substructure hierarchy; complete lattice structure with closure operators and Galois insertions, membership characterizations for directed suprema with induction principles, operations (map, comap, products)
- [x] `TypeTags/` - Type tags Additive and Multiplicative for converting between additive and multiplicative presentations; comprehensive instance transfer (all group-like structures), conversion functions (ofMul, toMul, ofAdd, toAdd), operation transfer, homomorphism transport, and finiteness preservation (infrastructure for to_additive automation)
- [x] `UniqueProds/` - Unique products property: groups where any two non-empty finite subsets contain a product writable uniquely as element from first times element from second; defines UniqueProds and TwoUniqueProds (stronger variant with two unique pairs), preservation under equivalences and homomorphisms, proves all ℚ-vector spaces have unique sums
- [x] `Units/` - Comprehensive theory of units (invertible elements) in monoids with bundled Units M type (notation Mˣ) and IsUnit predicate; group structure on units, homomorphism theory including Units.map lifting, equivalences showing groups are isomorphic to their unit groups, partial division operator divp, local homomorphisms, and opposite units
- [x] `WithOne/` - Adjoining a unit element to semigroups via WithOne α := Option α to obtain monoids (free functor from semigroups to monoids); includes algebraic instances, bundled homomorphisms for lifting (lift equivalence), and dual WithZero construction adjoining zero

## Search Tags

group monoid semigroup group-theory algebraic-structures typeclasses homomorphism automorphism endomorphism subgroup submonoid subsemigroup center conjugation commutator semiconjugation additive-character product opposite cancellation torsion action mul-action group-action equivalence mul-equiv units invertible to-additive bundled-morphism lattice-structure galois-insertion closure kernel range normal-subgroup pointwise-operations set-multiplication commute faithful-action pretransitive-action equidecomposition pi-types dependent-types fin integers naturals parity even-odd type-tags irreducible unique-products with-one free-monoid equivariant scalar-tower smul-comm-class distrib-mul-action bigoperators finsupp finite-index
