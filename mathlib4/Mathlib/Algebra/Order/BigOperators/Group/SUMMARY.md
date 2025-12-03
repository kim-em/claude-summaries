---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/BigOperators/Group
generated: 2025-12-01T20:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# Group

## Overview

The `Group/` directory provides order-theoretic properties of big operators (products and sums) in ordered monoids, groups, and related algebraic structures. This is the core implementation layer beneath `BigOperators/`, covering finsets, lists, multisets, and locally-finite orders. The files establish fundamental monotonicity results (`prod_le_prod`, `sum_le_sum`), submultiplicativity/subadditivity lemmas for functions applied to products/sums, comparison theorems between products over subsets, and specialized results for canonically-ordered and cancellative structures.

## Key Files

| File | Purpose |
|------|---------|
| Finset.lean | Order properties of finset big operators: monotonicity (`prod_le_prod'`, `sum_le_sum`), submultiplicativity (`le_prod_of_submultiplicative`), comparison with constants (`prod_le_pow_card`), subset comparisons (`prod_le_prod_of_subset_of_one_le'`), pigeonhole principle lemmas, double-counting arguments, positivity/nonnegativity characterizations (`prod_eq_one_iff_of_one_le'`, `one_lt_prod_iff_of_one_le`), and specialized results for canonically-ordered, ordered-cancel, and linear-order contexts |
| List.lean | Order properties of list big operators: monotonicity for `Forall₂` and sublists (`Forall₂.prod_le_prod'`, `Sublist.prod_le_prod'`), comparison lemmas (`prod_lt_prod'`, `exists_lt_of_prod_lt'`), bounds relative to constants (`prod_le_pow_card`), submultiplicativity results (`le_prod_of_submultiplicative`), and tropical-style max-fold lemmas (`sum_le_foldr_max`) |
| LocallyFinite.lean | Big operators indexed by order intervals (`Ico`, `Ioc`, `Ioo`, `Icc`, `Ioi`, `Iio`, `Ici`, `Iic`): telescoping-style identities relating products/sums over intervals with endpoint adjustments (`mul_prod_Ico_eq_prod_Icc`, `prod_Ioo_mul_eq_prod_Ico`), results for successor-based orders (`prod_Ico_mul_eq_prod_Ico_add_one`), off-diagonal product transformations (`prod_prod_Ioi_mul_eq_prod_prod_off_diag`), and a general theorem for nested finite set sequences (`prod_eq_prod_range_sdiff`) |
| Multiset.lean | Order properties of multiset big operators: monotonicity for related multisets (`prod_le_prod_of_rel_le`, `prod_map_le_prod_map`), single-element bounds (`single_le_prod`), submultiplicativity (`le_prod_of_submultiplicative`), strict comparison theorems for cancellative monoids (`prod_lt_prod'`, `prod_lt_prod_of_nonempty'`), canonically-ordered characterizations (`prod_eq_one_iff`, `le_prod_of_mem`), and absolute value bounds (`abs_sum_le_sum_abs`) |

## Subdirectories

None.

## Search Tags

big-operators finset-product finset-sum list-product list-sum multiset-product multiset-sum ordered-monoid ordered-group monotonicity submultiplicative subadditive prod-le-prod sum-le-sum locally-finite-order interval-arithmetic pigeonhole double-counting canonically-ordered-monoid ordered-cancel-monoid
