---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/BigOperators/GroupWithZero
generated: 2025-12-01T11:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# GroupWithZero

## Overview

The `GroupWithZero/` directory provides order-theoretic properties of big product operators on lists and multisets in ordered commutative monoids with zero. It establishes nonnegativity preservation (`prod_nonneg`, `one_le_prod`), monotonicity results for mapped products under positivity conditions (`prod_map_le_prod_map₀`), bounds comparing products to powers (`prod_map_le_pow_length₀`, `prod_map_le_pow_card`), and strict monotonicity results for strictly positive elements (`prod_pos`, `prod_map_lt_prod_map`). The list version proves these lemmas inductively, while the multiset version lifts them via quotient induction.

## Key Files

| File | Purpose |
|------|---------|
| List.lean | Order properties of list products in ordered monoids with zero: nonnegativity preservation (`prod_nonneg`, `one_le_prod`), monotonicity of mapped products with nonnegativity conditions (`prod_map_le_prod_map₀`), power bounds (`prod_map_le_pow_length₀`), strict positivity results (`prod_pos`), and strict monotonicity (`prod_map_lt_prod_map`) |
| Multiset.lean | Order properties of multiset products in ordered monoids with zero, lifting all list results via quotient induction: `prod_nonneg`, `one_le_prod`, `prod_map_le_prod_map₀`, `prod_map_le_pow_card`, `prod_pos`, `prod_map_lt_prod_map` |

## Subdirectories

(none)

## Search Tags

big-operators product list multiset ordered-monoid group-with-zero nonnegative monotonicity positivity strict-monotonicity commutative-monoid zero-le-one posmulmono quotient-induction
