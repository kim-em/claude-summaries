---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Divisibility
generated: 2025-12-04T02:23:11Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: preliminary
files_count: 5
subdirs_count: 0
---

# Divisibility

## Overview

The `Divisibility/` directory contains the foundational theory of divisibility relations in algebraic structures, building from basic semigroups to commutative monoids. It defines the divisibility predicate `a ∣ b` as `∃ c, b = a * c` following the ordinal convention (right multiplication), establishes fundamental properties (reflexivity, transitivity, behavior under multiplication), introduces primal elements and decomposition monoids (structures where elements factor through divisors), handles divisibility in product types, proves preservation of divisibility across homomorphisms, provides decidability instances for finite types, develops the theory of units and divisibility (showing units divide everything and divisibility modulo units), and culminates in the theory of relatively prime elements where common divisors are required to be units.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core divisibility theory: defines `semigroupDvd` instance with `a ∣ b ↔ ∃ c, b = a * c`, establishes reflexivity/transitivity/monotonicity, introduces `IsPrimal` elements (factoring through divisors) and `DecompositionMonoid` class, proves fundamental lemmas for semigroups/monoids/commutative structures including power divisibility |
| Finite.lean | Decidability instance for divisibility in finite types with decidable equality |
| Hom.lean | Preservation of divisibility across multiplication-preserving homomorphisms: `map_dvd` theorem and specialized versions for `MulHom` and `MonoidHom` |
| Prod.lean | Divisibility in product and pi types: proves `(x₁, x₂) ∣ (y₁, y₂) ↔ x₁ ∣ y₁ ∧ x₂ ∣ y₂` and analogous result for pi types, shows products of decomposition monoids are decomposition monoids |
| Units.lean | Units and divisibility: proves units divide all elements, divisibility is invariant under multiplication by units (`a ∣ b * u ↔ a ∣ b`), defines `IsRelPrime x y` (common divisors are units), develops relative primality theory including multiplicativity in decomposition monoids and divisibility extraction from products of relatively prime elements |

## Subdirectories

(No subdirectories)

## Search Tags

divisibility divides dvd semigroup monoid commutative units primal decomposition-monoid relatively-prime coprime homomorphism product-types finite-types
