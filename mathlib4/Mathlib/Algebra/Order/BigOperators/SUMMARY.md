---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/BigOperators
generated: 2025-12-01T19:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 1
subdirs_count: 3
---

# BigOperators

## Overview

The `BigOperators/` directory establishes comprehensive order-theoretic properties of big operators (sums and products) across finsets, lists, and multisets in ordered algebraic structures. The theory is organized by algebraic context: `Group/` covers ordered groups and monoids with monotonicity, submultiplicativity, subset comparisons, and positivity characterizations; `GroupWithZero/` handles nonnegativity preservation and strict monotonicity in monoids with zero; `Ring/` provides the full ordered ring theory including the **Cauchy-Schwarz inequality** in multiple forms (standard, Sedrakyan's/Titu's/Engel's lemma), product/sum monotonicity under nonnegativity (`prod_le_prod`, `sum_le_sum`), and sum-of-squares bounds. The top-level `Expect.lean` file extends this framework to the expectation operator (average over a finset), proving monotonicity, subadditivity, and a specialized Cauchy-Schwarz inequality for expected values.

## Key Files

| File | Purpose |
|------|---------|
| Expect.lean | Order properties of finset expectation (`𝔼 i ∈ s, f i`): monotonicity lemmas, conditions for zero expectations, subadditivity of expectations, positivity extension for the `positivity` tactic, absolute value bound, and Cauchy-Schwarz inequality for expectations |

## Subdirectories

- [x] `Group/` - Order properties of big operators in ordered groups and monoids across finsets, lists, multisets, and locally-finite orders: monotonicity results, submultiplicativity/subadditivity, subset comparisons, pigeonhole and double-counting lemmas, positivity characterizations, and specialized results for canonically-ordered and cancellative structures
- [x] `GroupWithZero/` - Order properties of big product operators on lists and multisets in ordered commutative monoids with zero: nonnegativity preservation, monotonicity under positivity conditions, power bounds, and strict monotonicity results
- [x] `Ring/` - Order properties of big operators in ordered rings: product/sum nonnegativity, monotonicity under nonnegativity conditions (`prod_le_prod`, `sum_le_sum`), Cauchy-Schwarz inequality in its standard form and variants (Sedrakyan's/Titu's/Engel's), sum-of-squares bounds, and submultiplicative results

## Search Tags

big-operators finset-sum finset-product expectation average cauchy-schwarz inequality monotonicity subadditive submultiplicative ordered-monoid ordered-ring positivity nonnegative
