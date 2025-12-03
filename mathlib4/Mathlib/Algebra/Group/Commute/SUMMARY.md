---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Commute
generated: 2025-12-01T22:40:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# Commute

## Overview

The `Commute/` directory provides the theory of commuting elements in monoids and groups, defining the fundamental predicate `Commute a b := a * b = b * a` and developing a comprehensive library of operations and lemmas for working with commuting pairs. It implements commutativity as a special case of semiconjugation (`SemiconjBy a b b`), enabling substantial code reuse from the semiconjugation theory. The directory includes basic operations on commuting pairs (multiplication, powers, inverses), advanced lemmas for division monoids and groups (including conjugation invariance and complex division identities), preservation under homomorphisms, and specialized theory for units and invertible elements.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `Commute a b` as `SemiconjBy a b b` (i.e., `a * b = b * a`); proves basic properties including reflexivity, symmetry, closure under multiplication and powers, and derives `mul_pow` formula `(a * b) ^ n = a ^ n * b ^ n` for commuting elements; includes both natural power lemmas for monoids and integer power lemmas for division monoids |
| Basic.lean | Additional lemmas requiring more imports; proves `function_commute_mul_left/right` (commutativity of partially applied multiplication functions), inverse commutativity (`inv_inv`, `inv_left/right`), complex division identities (`div_mul_div_comm`, `div_div_div_comm`), conjugation preservation (`(h * a * h⁻¹)` commutes with `(h * b * h⁻¹)` iff `a` commutes with `b`), and integer power lemmas (`zpow_left/right`, `zpow_zpow`) |
| Hom.lean | Homomorphism preservation of commutativity; proves `Commute.map` (homomorphisms preserve commuting pairs), `Commute.of_map` (injective homomorphisms reflect commutativity), and bidirectional iff statements for checking commutativity via homomorphism images |
| Units.lean | Commutativity theory for units (invertible elements); proves units-specific lemmas (`units_inv_left/right`, `units_val`), decomposes unit products into unit factors (`Units.leftOfMul/rightOfMul`), proves `isUnit_mul_iff` characterization for commuting products, `isUnit_pow_iff` showing `a^n` is a unit iff `a` is (for `n ≠ 0`), and constructs units from elements with unit powers (`Units.ofPowEqOne`) |

## Subdirectories

None.

## Search Tags

commute commutativity commuting-elements semiconjugation mul-comm group-theory monoid-theory pow-comm mul-pow div-comm conjugation units invertible homomorphism-preservation to-additive reflexive symmetric
