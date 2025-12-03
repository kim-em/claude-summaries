---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/GroupWithZero/Units
generated: 2025-12-01T10:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Units

## Overview

The `Units/` directory contains the theory of units in monoids and groups with zero, establishing the fundamental connection between nonzero elements and invertibility. The main results include that units are nonzero (and vice versa in groups with zero), the `Ring.inverse` function extending inversion to all elements by sending non-units to zero, the `Units.mk0` constructor embedding nonzero elements as units, and equivalences showing that multiplication by nonzero elements are permutations of the type.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core unit theory: units are nonzero (`Units.ne_zero`), multiplication cancellation with units, `IsUnit` characterizations, the `Ring.inverse` function (globally defined inverse sending non-units to zero), `Units.mk0` constructor for nonzero elements, equivalence `isUnit_iff_ne_zero`, integer power lemmas (`zpow_ne_zero`, `zpow_sub₀`), and constructions `groupWithZeroOfIsUnitOrEqZero`, `commGroupWithZeroOfIsUnitOrEqZero` for types where every element is either a unit or zero |
| Equiv.lean | Permutation equivalences: `unitsEquivNeZero` (units equivalent to nonzero elements), `Equiv.mulLeft₀`/`mulRight₀` (multiplication by nonzero elements as permutations), `Equiv.divRight₀`/`divLeft₀` (division as permutations in commutative case), and bijectivity lemmas (`mulLeft_bijective₀`, `mulRight_bijective₀`) |
| Lemmas.lean | Homomorphism interaction with units: `map_ne_zero`/`map_eq_zero` characterizations for monoid-with-zero homomorphisms, `map_inv₀` and `map_div₀` preservation, `map_zpow₀` for integer powers, `eq_on_inv₀` uniqueness, `Commute.div_eq_div_iff` and related division identities, `MonoidWithZero.inverse` as homomorphism, `invMonoidWithZeroHom` for commutative groups with zero, and `isLocalHom_of_exists_map_ne_one` instance |

## Subdirectories

(none)

## Search Tags

units nonzero-elements invertible group-with-zero monoid-with-zero ring-inverse mk0 units-equiv permutation multiplication-bijection division-permutation homomorphism-preservation local-homomorphism zpow-integer-powers
