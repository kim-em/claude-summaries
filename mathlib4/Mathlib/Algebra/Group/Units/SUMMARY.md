---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Units
generated: 2025-12-01T22:05:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 5
subdirs_count: 0
---

# Units

## Overview

The `Units/` directory contains the comprehensive theory of units (invertible elements) in monoids. It defines the bundled `Units M` type (denoted `Mˣ`) representing elements with two-sided inverses, the predicate `IsUnit` for testing invertibility, and extensive supporting lemmas for reasoning about units. The folder covers homomorphisms on units, equivalences between groups and their unit groups, opposite units, and local homomorphisms that preserve unit structure.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: bundled `Units M` structure with value, inverse, and two-sided inverse proofs; `IsUnit` predicate; group structure on `Mˣ`; partial division operator `divp`; utility functions like `mkOfMulEqOne` and `groupOfIsUnit` |
| Basic.lean | Basic lemmas about units in monoids: cancellation laws, injectivity properties, decidable equality, interaction with singleton/subsingleton types; uniqueness results for units and behavior in cancellation monoids |
| Hom.lean | Homomorphism theory: `Units.map` lifts monoid homomorphisms to unit groups; `MonoidHom.toHomUnits` embeds groups into unit groups; `Units.liftRight` and `IsUnit.liftRight` for constructing homomorphisms; `IsLocalHom` class for homomorphisms preserving nonunits |
| Equiv.lean | Equivalences involving units: `toUnits` shows groups are isomorphic to their unit groups; `Units.mapEquiv` lifts multiplicative equivalences; `Units.mulLeft` and `Units.mulRight` show unit multiplication is bijective; `MulEquiv.inv` for division monoids |
| Opposite.lean | Units in opposite monoids: `Units.opEquiv` establishes `Mᵐᵒᵖˣ ≃* Mˣᵐᵒᵖ`; `IsUnit.op` and `IsUnit.unop` transfer unit predicates across opposite structures |

## Subdirectories

None.

## Search Tags

units invertible-elements monoid-units group-units IsUnit divp partial-division units-group homomorphism MulEquiv local-homomorphism opposite-units unit-cancellation unit-equivalence
