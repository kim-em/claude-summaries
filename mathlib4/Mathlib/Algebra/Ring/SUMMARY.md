---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Ring
generated: 2025-12-01T21:50:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 44
subdirs_count: 9
---

# Ring

## Overview

The `Ring/` directory forms the foundational layer of ring theory in mathlib4, implementing the complete theory of semirings and rings from core definitions through sophisticated algebraic constructions. This directory sits at a critical junction in the algebraic hierarchy, building on group theory (`Mathlib/Algebra/Group/`) and group-with-zero theory (`Mathlib/Algebra/GroupWithZero/`) to establish distributive algebraic structures where multiplication distributes over addition. The implementation spans three major aspects: (1) fundamental type class definitions and basic properties establishing the ring axioms and their immediate consequences, (2) structural theory including ring homomorphisms/equivalences, substructures (subsemirings, subrings), and morphism operations, and (3) element-theoretic properties covering units, regular elements, idempotents, divisibility, and special elements like sums of squares.

The directory architecture reflects a systematic approach to ring theory, with subdirectories devoted to specialized aspects: `Action/` develops the theory of multiplicative group actions on rings (essential for Galois theory and automorphism groups), `Hom/` and `Equiv/` establish the morphism theory, `Subring/` and `Subsemiring/` implement the complete lattice structure of subobjects with closure operations and Galois insertions, `Divisibility/` extends divisibility theory to rings, `Int/` provides the canonical example of a commutative ring, and specialized directories like `Semireal/` and `Pointwise/` develop niche but important theoretical aspects.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `Distrib`, `NonUnital/NonAssoc/Semiring/Ring` type classes with distributivity axioms and basic instances |
| Basic.lean | Fundamental lemmas about semirings and rings: distributivity properties, additive homomorphism constructions (`mulLeft`, `mulRight`), and commutativity characterizations |
| Equiv.lean | Ring equivalences (`RingEquiv`, notation `≃+*`): isomorphisms of semirings/rings/division rings/fields preserving algebraic structure |
| InjSurj.lean | Pullback and pushforward of ring structures along injective/surjective functions |
| BooleanRing.lean | Boolean rings (idempotent multiplication): equivalence with Boolean algebras via type synonyms `AsBoolAlg`/`AsBoolRing` |
| Idempotent.lean | Idempotent elements in rings: `a * a = a`, complementation `1 - a`, and characterizations via orthogonality |
| CentroidHom.lean | Centroid homomorphisms: linear maps commuting with left and right multiplication (`T(ab) = (Ta)b = a(Tb)`) |
| Parity.lean | Even and odd elements in rings: characterizations via `2 * b`, divisibility by 2, and power properties |
| Periodic.lean | Periodic and antiperiodic functions on rings: `f(x + c) = f(x)` and `f(x + c) = -f(x)` |
| GeomSum.lean | Geometric sum formulas: `∑ i < n, x^i` identities and convergence properties |
| NonZeroDivisors.lean | Non-zero divisors: elements `a` where `a * b = 0` or `b * a = 0` implies `b = 0` |
| Commute.lean | Commuting elements: `a * b = b * a` and related properties for ring elements |
| Semiconj.lean | Semiconjugate elements: `a * b = c * a` and conjugation properties |
| Units.lean | Units in rings: invertible elements, group structure on `Rˣ`, and conversions |
| Invertible.lean | Invertible elements (unbundled units): typeclass for elements with two-sided inverses |
| Regular.lean | Regular elements: left/right regular elements (cancellative for multiplication) |
| Associated.lean | Associated elements: `a` and `b` related by multiplication by a unit |
| SumsOfSquares.lean | Sums of squares in rings: representations of elements as sums of squares |
| CompTypeclasses.lean | Compatibility type classes for ring structures |
| Opposite.lean | Opposite rings: ring structure on the opposite type with reversed multiplication |
| Prod.lean | Product rings: componentwise ring operations on product types |
| Pi.lean | Pi types: ring structure on function types `∀ i, α i` |
| CharZero.lean | Characteristic zero rings: natural number coercions are injective |
| NegOnePow.lean | Powers of -1: `(-1)^n` identities and parity properties |
| Identities.lean | Ring identities: Jacobi identity and other polynomial identities |
| Associator.lean | Associator in non-associative rings: `(a * b) * c - a * (b * c)` |
| Center.lean | Center of a ring: elements commuting with all elements |
| Centralizer.lean | Centralizer: elements commuting with a given subset |
| Aut.lean | Ring automorphisms: `Rˣ≃+*`-valued automorphisms |
| AddAut.lean | Additive automorphisms interacting with multiplication |
| TransferInstance.lean | Transferring ring instances along equivalences |
| Torsion.lean | Torsion elements in rings: elements with finite additive order |
| Ext.lean | Extension results for ring homomorphisms |
| MinimalAxioms.lean | Minimal axiomatization of ring structures |
| Fin.lean | Ring instances for `Fin n` types |
| Nat.lean | Ring properties specific to natural numbers |
| Int.lean | Entry point for integer-specific ring theory |
| Rat.lean | Ring properties specific to rational numbers |
| PUnit.lean | Ring instance for the unit type |
| ULift.lean | Ring instance for universe lifts |
| WithZero.lean | Ring-like structures with zero adjoined |
| Shrink.lean | Ring structure on shrunk types |
| Subgroup.lean | Ring structure on additive subgroups |
| Submonoid.lean | Entry point for submonoid theory in rings |
| GrindInstances.lean | Instances for the `grind` tactic automation |

## Subdirectories

- [x] `Action/` - Multiplicative actions by monoids and groups on rings with MulSemiringAction typeclass combining distributive actions with multiplicative compatibility, essential for Galois theory, conjugation by units, automorphism group actions, and field extensions
- [x] `Divisibility/` - Divisibility theory in rings with core divisibility relation properties in semirings and rings, extended theory with scalar multiplication interaction and nilpotent element divisibility, establishing how divisibility interacts with addition, subtraction, negation, and multiplicative equivalence characterizations
- [x] `Hom/` - Ring homomorphism theory with bundled RingHom and NonUnitalRingHom structures, type classes, composition, identity, constructors from monoid/additive homomorphisms, and pullback of domain properties along injective homomorphisms
- [x] `Int/` - Integer ring theory with core CommRing instance for integers, parity theory, and units characterization, establishing integers as the canonical example of a commutative ring with characteristic zero and domain properties
- [x] `Pointwise/` - Pointwise operations on sets in rings with distributive negation instances and subset-based one-sided distributivity laws (equality fails due to cross terms from pointwise operations)
- [x] `Semireal/` - Semireal rings where negative one is not a sum of squares (fundamental in real algebra), with instance showing linearly ordered semirings satisfy this property
- [x] `Submonoid/` - Additive submonoids in rings with closure properties and pointwise multiplication structure yielding monoid structure on the collection of additive submonoids
- [x] `Subring/` - Bundled subrings (subsemirings plus additive subgroups) with complete lattice structure, Galois insertion for closure, map/comap along ring homomorphisms, center and centralizer constructions, polynomial operations for integral elements, opposite ring equivalences, ordered subring instances, pointwise group actions, and positive unit subgroups
- [x] `Subsemiring/` - Bundled subsemirings (closure under addition and multiplication) with complete lattice structure, comap/map/range operations along ring homomorphisms, center and centralizer, opposite semiring equivalences, ordered instances, and pointwise scalar actions

## Search Tags

ring semiring distributive multiplication addition ring-homomorphism ring-equivalence ring-isomorphism boolean-ring idempotent centroid parity even odd periodic antiperiodic geometric-sum non-zero-divisors commute semiconjugate units invertible regular associated sums-of-squares characteristic-zero opposite-ring product-ring pi-type center centralizer automorphism ring-automorphism subring subsemiring divisibility dvd mul-semiring-action group-action galois semireal pointwise submonoid additive-closure integers parity-int units-int int-ring basic-definitions defs type-class
