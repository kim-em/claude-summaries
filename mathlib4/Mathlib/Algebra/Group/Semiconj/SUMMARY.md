---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Semiconj
generated: 2025-12-01T21:35:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Semiconj

## Overview

The `Semiconj/` directory defines the semiconjugation relation on algebraic structures and provides operations on semiconjugate elements. The core concept is that element `x` is semiconjugate to `y` by `a` (written `SemiconjBy a x y`) when `a * x = y * a`. This generalizes the notion of commuting elements (where `x = y`) and conjugation (where `a * x * a⁻¹ = y`). The directory provides the definition, basic operations for semigroups and monoids, specialized lemmas for groups and division monoids, and theory for semiconjugation of units.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `SemiconjBy a x y : Prop` as `a * x = y * a`; basic operations including `mul_right`, `mul_left`, `one_right`, `one_left`, `pow_right`; proves the semiconjugation relation is transitive and reflexive; includes `conj_mk` showing `a` semiconjugates `x` to `a * x * a⁻¹` in groups |
| Basic.lean | Group-specific lemmas for semiconjugation including inversion properties (`inv_inv_symm_iff`, `inv_symm_left_iff`, `inv_right_iff`), integer powers (`zpow_right`), and equivalence with identity (`eq_one_iff`); extends semiconjugation theory to division monoids and groups |
| Units.lean | Semiconjugation theory for units (invertible elements) in monoids; provides `units_inv_right`, `units_inv_symm_left`, `units_val` for converting between unit and underlying type semiconjugations; includes `units_zpow_right` for integer powers and helper lemmas `Units.mk_semiconjBy` and `Units.conj_pow` |

## Subdirectories

(none)

## Search Tags

semiconjugation semiconjugate group-theory semigroup monoid group division-monoid units conjugation commute to-additive algebraic-structures
