---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/BigOperators/GroupWithZero
generated: 2025-12-01T11:03:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# GroupWithZero

## Overview

This directory extends big operator theory to algebraic structures with zero elements, providing two main components: (1) interaction theorems for finset products/sums in groups and monoids with zero, including zero-propagation, zero-detection (`prod_eq_zero_iff`), and support characterization; and (2) scalar action distributivity lemmas showing how group actions distribute over big operators, with three variants for `DistribSMul` (sums), `MulDistribMulAction` (products with primed names), and `SMulCommClass` (products with power scaling). These results are fundamental for reasoning about products that can vanish and for manipulating scalar actions in summation contexts.

## Key Files

| File | Purpose |
|------|---------|
| Finset.lean | Big operators in monoids/groups with zero: core theorems `prod_eq_zero` (element zero forces product zero), `prod_eq_zero_iff` (product zero iff some element zero, requires no zero divisors), `prod_ne_zero_iff`, `support_prod` (support characterization), conditional products `prod_ite_zero`/`prod_boole`, indicator functions for pi types, and `Units.mk0_prod` for group with zero units |
| Action.lean | Group action distributivity over big operators: three flavors of scalar-product interaction including `Finset.smul_sum` (`r • ∑ x ∈ s, f x = ∑ x ∈ s, r • f x` for `DistribSMul`), `Finset.smul_prod'` (primed variant for `MulDistribMulAction`), and `Finset.smul_prod` (unprimed with power: `b ^ s.card • ∏ x ∈ s, f x = ∏ x ∈ s, b • f x`), plus permutation invariance lemmas and corresponding results for lists, multisets, finprods, and finsums |

## Subdirectories

(none)

## Search Tags

group-with-zero monoid-with-zero big-operators product-zero prod-eq-zero zero-divisors support scalar-action distribsmul muldistribmulaction smulcommclass finset-product finset-sum indicator-function units-mk0 action-distributivity permutation-invariance
