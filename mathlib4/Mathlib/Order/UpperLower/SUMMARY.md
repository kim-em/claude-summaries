---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/UpperLower
generated: 2026-01-26T07:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 9
subdirs_count: 0
---

# UpperLower

## Overview

The `UpperLower/` directory contains the formalization of upper and lower sets in order theory, including both unbundled predicates (`IsUpperSet`, `IsLowerSet`) and bundled types (`UpperSet`, `LowerSet`). Upper sets are closed upward under the order relation (if `a ∈ s` and `a ≤ b`, then `b ∈ s`), while lower sets are closed downward. The directory provides the complete lattice structure on these types (with upper sets ordered by reverse inclusion to match the convention on filters), principal upper/lower sets (`Ici`, `Iic`, `Ioi`, `Iio`), closure operators for generating upper/lower sets from arbitrary sets, set difference operations, product constructions, and connections to fibrations and locally finite orders. Upper sets and lower sets are order-isomorphic under complementation.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core properties of unbundled `IsUpperSet` and `IsLowerSet` predicates: interactions with set operations (union, intersection, complement), images/preimages under monotone functions and order isomorphisms, characterizations in preorders/partial orders/linear orders, special cases for bounded and well-founded orders |
| Closure.lean | Upper and lower closure operators: `upperClosure s` is the smallest upper set containing `s` (equivalently `⋃ a ∈ s, Ici a`), `lowerClosure s` is the smallest lower set containing `s`; includes Galois connections with coercion, disjointness properties, set difference operations (`UpperSet.sdiff`, `LowerSet.sdiff`, `erase`), and antichain characterizations |
| CompleteLattice.lean | Complete lattice and completely distributive lattice structures on `UpperSet` and `LowerSet` types: upper sets ordered by reverse inclusion (matching filter convention), lattice operations via set intersections/unions, complementation making them order-isomorphic, `map` functions for order isomorphisms, linear order instances when base type is linear |
| Principal.lean | Principal upper and lower sets: `UpperSet.Ici a` (elements ≥ a), `UpperSet.Ioi a` (elements > a), `LowerSet.Iic a` (elements ≤ a), `LowerSet.Iio a` (elements < a); includes strictness and injectivity, lattice operation preservation (`Ici_sup`, `Iic_inf`), completeness results (`Ici_sSup`, `Iic_sInf`) |
| Hom.lean | Bundled homomorphisms for principal upper/lower set constructors: `UpperSet.iciSupHom` (`Ici` as `SupHom`), `UpperSet.icisSupHom` (`Ici` as `sSupHom`), `LowerSet.iicInfHom` (`Iic` as `InfHom`), `LowerSet.iicsInfHom` (`Iic` as `sInfHom`) |
| Prod.lean | Cartesian product of upper/lower sets: product construction (`×ˢ`), preservation of upper/lower set properties, lattice operation interactions (`prod_sup`, `prod_inf`), monotonicity, and closure interactions (`upperClosure_prod`, `lowerClosure_prod`) |
| Fibration.lean | Characterization of fibrations via upper/lower sets: fibration of `≤` relation iff images of lower sets are lower sets (dually for upper sets), equivalences involving `Iic`/`Ici` images, characterizations for monotone functions |
| LocallyFinite.lean | Finiteness of closures in locally finite orders: if `s` is finite and the order is locally finite (with top/bottom), then `upperClosure s` and `lowerClosure s` are finite sets |
| Relative.lean | Relative upper and lower sets (`IsRelUpperSet`, `IsRelLowerSet`): sets that are upper/lower relative to a predicate `P`, including closure under set operations, connection to subtype upper/lower sets, bundled types `RelUpperSet` and `RelLowerSet`, examples with intervals |

## Subdirectories

(none)

## Search Tags

upper-set lower-set IsUpperSet IsLowerSet UpperSet LowerSet closure principal Ici Iic Ioi Iio complement order-dual lattice-structure complete-lattice Galois-connection fibration product relative-upper-set locally-finite antichain
