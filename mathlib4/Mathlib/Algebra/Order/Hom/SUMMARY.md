---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Hom
generated: 2025-12-01T10:59:30Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 7
subdirs_count: 0
---

# Hom

## Overview

The `Hom/` directory defines homomorphisms and isomorphisms that preserve both algebraic structure and order relations. It provides a comprehensive framework for order-preserving morphisms across monoids, monoids with zero, rings, and their variants, including bundled types (`OrderMonoidHom`, `OrderRingHom`), their isomorphism counterparts, and numerous homomorphism classes for norms and seminorms (group norms, ring norms, submultiplicative/subadditive morphisms). The directory also includes specialized results for submonoids, type tags (Additive/Multiplicative), and units.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Algebraic order homomorphism classes: basic typeclasses (`NonnegHomClass`, `SubadditiveHomClass`, `SubmultiplicativeHomClass`), group seminorms and norms (`AddGroupSeminormClass`, `GroupNormClass`), and ring seminorms and norms (`RingSeminormClass`, `MulRingNormClass`) for functions at the intersection of order theory and algebra |
| Monoid.lean | Ordered monoid/group homomorphisms and isomorphisms: bundled types `OrderMonoidHom` (`→*o`), `OrderAddMonoidHom` (`→+o`), `OrderMonoidIso` (`≃*o`), `OrderAddMonoidIso` (`≃+o`) with composition, identity, coercion infrastructure, and monotonicity characterizations for ordered additive groups |
| MonoidWithZero.lean | Ordered monoid with zero homomorphisms: bundled type `OrderMonoidWithZeroHom` (`→*₀o`) for functions preserving multiplication, one, zero, and monotonicity, plus isomorphisms `OrderMonoidIso.unitsWithZero`, `OrderMonoidIso.withZero`, `OrderMonoidIso.withZeroUnits` connecting units and WithZero constructions |
| Ring.lean | Ordered ring homomorphisms and isomorphisms: bundled types `OrderRingHom` (`→+*o`) and `OrderRingIso` (`≃+*o`) for monotone semiring morphisms, with composition, identity, coercion to ring/order homomorphisms, and partial order instances |
| Submonoid.lean | Order isomorphism between top submonoid and whole monoid: `Submonoid.topOrderMonoidIso` showing `(⊤ : Submonoid α) ≃*o α` |
| TypeTags.lean | Order monoid isomorphisms on type tags: conversions between `OrderMonoidIso` and `OrderAddMonoidIso` via `Additive`/`Multiplicative` type tags, including `toAdditive`, `toMultiplicative`, bidirectional variants, and uniqueness instances |
| Units.lean | Order monoid isomorphism descent to units: `OrderMonoidIso.unitsCongr` showing that an isomorphism of ordered monoids `α ≃*o β` descends to their units `αˣ ≃*o βˣ` |

## Subdirectories

No subdirectories.

## Search Tags

order-preserving-homomorphisms ordered-monoid-homomorphisms ordered-ring-homomorphisms order-isomorphisms seminorms group-norms ring-norms subadditive submultiplicative nonarchimedean bundled-morphisms monoid-with-zero type-tags additive-multiplicative units submonoid funlike-classes
