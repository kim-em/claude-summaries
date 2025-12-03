---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/BigOperators/Ring
generated: 2025-12-01T10:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Ring

## Overview

The `Ring/` directory contains order-theoretic properties of big operators (products and sums) over finsets, lists, and multisets in ordered rings and semirings. The main file `Finset.lean` provides the comprehensive theory including monotonicity of products under nonnegativity conditions (`prod_le_prod`, `prod_nonneg`), sum-of-squares inequalities, submultiplicativity results, the standard **Cauchy-Schwarz inequality** and its variants (including Sedrakyan's/Titu's/Engel's form), and absolute value preservation for products. The `List.lean` and `Multiset.lean` files provide positivity characterizations for products in canonically-ordered structures.

## Key Files

| File | Purpose |
|------|---------|
| Finset.lean | Comprehensive ordered ring theory for finset big operators: product nonnegativity and monotonicity (`prod_nonneg`, `prod_le_prod`, `prod_pos`, `prod_lt_prod`), positivity results for products in ordered commutative monoids with zero, sum-of-squares bounds (`sum_sq_le_sq_sum_of_nonneg`), submultiplicative bounds for functions applied to products, Cauchy-Schwarz inequality in standard and generalized forms (`sum_mul_sq_le_sq_mul_sq`, `sum_sq_le_sum_mul_sum_of_sq_eq_mul`), Sedrakyan's lemma (`sq_sum_div_le_sum_sq_div`), absolute value homomorphism for products, canonical ordering results, and positivity tactic extension for products |
| List.lean | Positivity characterization for list products in canonically-ordered commutative semirings: `0 < l.prod ↔ (∀ x ∈ l, 0 < x)` when the semiring is nontrivial with no zero divisors |
| Multiset.lean | Positivity characterization for multiset products in canonically-ordered structures (`0 < m.prod ↔ ∀ x ∈ m, 0 < x`), and submultiplicative bounds for functions applied to multiset products under nonnegativity conditions |

## Subdirectories

*(No subdirectories)*

## Search Tags

big-operators finset-product finset-sum ordered-ring ordered-semiring cauchy-schwarz inequality sedrakyan titu engel monotonicity prod-le-prod prod-nonneg prod-pos submultiplicative sum-of-squares absolute-value canonically-ordered positivity list-product multiset-product
