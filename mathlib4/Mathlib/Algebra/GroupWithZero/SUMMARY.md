---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/GroupWithZero
generated: 2025-12-01T19:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 30
subdirs_count: 4
---

# GroupWithZero

## Overview

The `GroupWithZero/` directory implements the complete algebraic hierarchy layer between groups and rings, defining structures where multiplication forms a group on nonzero elements while zero absorbs multiplication. The directory provides four major components: (1) fundamental type classes (`GroupWithZero`, `CommGroupWithZero`, `MonoidWithZero`, `CancelMonoidWithZero`) with comprehensive theory including homomorphisms, divisibility, regularity, and the critical nonzero-unit correspondence; (2) the `Action/` subdirectory developing zero-preserving scalar multiplication (`SMulZeroClass`, `DistribMulAction`, `MulActionWithZero`) with pointwise set operations, forming the foundation for module theory; (3) the `Units/` subdirectory establishing that units are precisely nonzero elements (via `Units.mk0`), `Ring.inverse` extending inversion globally, and multiplication-as-permutation equivalences; and (4) the `Submonoid/` subdirectory providing cancellation inheritance, homomorphism range instances, and pointwise operations under group-with-zero actions. Together with the `Pointwise/` theory of set operations and cardinality preservation, these components form the essential bridge between pure group theory and ring/field theory, appearing throughout division rings, valuation theory, field theory, linear algebra, and functional analysis.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core type class definitions: `MulZeroClass`, `MonoidWithZero`, `CancelMonoidWithZero`, `GroupWithZero`, `CommGroupWithZero`, and cancellation properties (`IsLeftCancelMulZero`, `IsRightCancelMulZero`, `IsCancelMulZero`) |
| Basic.lean | Main theory development: multiplication/division lemmas, power laws (npow/zpow), injectivity/surjectivity results, inverse properties, and `GroupWithZero.toDivisionMonoid` instance |
| WithZero.lean | Construction adjoining zero to groups/monoids: `WithZero α ≃* {0} ∪ α` with `exp`/`log` maps for additive groups, monoid homomorphism lifting, and `Mᵐ⁰` notation for valuation theory |
| NonZeroDivisors.lean | Submonoid of non-zero-divisors: definitions of `nonZeroDivisorsLeft`, `nonZeroDivisorsRight`, `nonZeroDivisors` (M₀⁰), `nonZeroSMulDivisors`, characterizations via regularity, and equivalence `nonZeroDivisors G₀ ≃* G₀ˣ` for groups with zero |
| Associated.lean | Equivalence relation of elements differing by unit multiplication: `Associated` relation, `Associates` quotient type as monoid, and basic properties |
| Hom.lean | Homomorphisms: `MonoidWithZeroHom` (notation →*₀), `MonoidWithZeroHomClass`, composition, identity, and preservation of zero/multiplication |
| Units.lean | Units in monoids/groups with zero (located in Units/ subdirectory) |
| Divisibility.lean | Divisibility theory in monoids with zero: dvd relations, divisibility by zero, and interaction with units |
| InjSurj.lean | Injective and surjective homomorphisms: preservation of structures, inverse construction, and characterizations |
| Regular.lean | Regular elements (non-zero-divisors): `IsLeftRegular`, `IsRightRegular`, `IsRegular`, and their characterizations |
| Range.lean | Range of monoid homomorphisms: closure properties and range as submonoid |
| Center.lean | Center of monoids with zero: elements commuting with all others |
| Commute.lean | Commutativity of specific elements: `Commute` relation and properties in presence of zero |
| Semiconj.lean | Semiconjugation in monoids with zero: `SemiconjBy` relation |
| Equiv.lean | Equivalences between monoids/groups with zero |
| Invertible.lean | `Invertible` typeclass for elements with constructive inverses |
| Pi.lean | Product structures: `GroupWithZero` on function types `∀ i, f i` |
| Prod.lean | Product structures: `GroupWithZero` on `α × β` |
| Opposite.lean | Opposite monoid/group with zero structures |
| Indicator.lean | Indicator functions in context of groups with zero |
| NeZero.lean | `NeZero` typeclass: type-level assertion that specific element is nonzero |
| Idempotent.lean | Idempotent elements in monoids with zero |
| Nat.lean | Natural number instances and coercions |
| Int.lean | Integer instances and coercions |
| Torsion.lean | Torsion elements: elements with finite multiplicative order |
| TransferInstance.lean | Transferring instances across equivalences |
| ULift.lean | Universe lifting for groups with zero |
| Shrink.lean | Universe shrinking for groups with zero |
| ProdHom.lean | Product homomorphisms between groups with zero |
| Subgroup.lean | Subgroups in groups with zero |

## Subdirectories

- [x] `Action/` - Complete theory of group and monoid actions in the presence of zero: fundamental action typeclasses (SMulZeroClass, SMulWithZero, MulActionWithZero, DistribSMul, DistribMulAction, MulDistribMulAction) preserving zero/addition/multiplication, instances for all standard constructions (products, Pi types, opposites, units, homomorphism types), homomorphisms and equivalences respecting zero-preserving structures, and pointwise operations on set/finset collections with zero behavior characterizations
- [x] `Pointwise/` - Pointwise operations on both infinite sets (using Cardinals) and finite sets (using natural number cardinalities): zero multiplication/division collapsing behavior, cardinality preservation for nonzero scalar multiplication via injectivity, and cardinality inequalities for finite sets using cancellation properties
- [x] `Submonoid/` - Submonoid-specific theory for monoids with zero: cancellation property inheritance (submagmas inherit IsLeftCancelMulZero, IsRightCancelMulZero, IsCancelMulZero from ambient structures), instance construction for homomorphism ranges (MonoidHom.mrange instances for MulZeroOneClass, MonoidWithZero, CommMonoidWithZero, GroupWithZero, CommGroupWithZero), pointwise scalar multiplication under GroupWithZero actions with membership and order characterizations, and primal elements submonoid in cancellative commutative monoids
- [x] `Units/` - Complete unit theory in monoids/groups with zero: fundamental connection between nonzero elements and invertibility, Ring.inverse function extending inversion to all elements (sending non-units to zero), Units.mk0 constructor embedding nonzero elements as units, permutation equivalences (unitsEquivNeZero, Equiv.mulLeft₀, Equiv.mulRight₀, Equiv.divRight₀, Equiv.divLeft₀), and homomorphism preservation of units/inverses/division/integer powers

## Search Tags

group-with-zero monoid-with-zero cancel-monoid division-monoid non-zero-divisors with-zero adjoined-zero valuation-theory regular-elements units associated-elements homomorphism zero-absorption multiplicative-structure field-foundations division-ring
