---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/GroupWithZero/Action/Pointwise
generated: 2025-12-01T06:12:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Pointwise

## Overview

The `Pointwise/` directory develops the theory of pointwise scalar multiplication on sets and finite sets in the context of groups with zero. It establishes that set and finset collections inherit action structures (`SMulZeroClass`, `DistribSMul`, `DistribMulAction`, `MulDistribMulAction`) from their element types, proves that nonzero scalars act injectively (preserving intersections, set differences, symmetric differences), and characterizes when zero appears in scaled collections (`zero_mem_smul_iff`). This machinery is essential for pointwise operations in algebraic structures with zero, particularly in convexity theory, measure theory, and functional analysis where sets of elements must be scaled.

## Key Files

| File | Purpose |
|------|---------|
| Set.lean | Pointwise scalar multiplication on sets: typeclass instances (`Set.smulZeroClassSet`, `Set.distribSMulSet`, `Set.distribMulActionSet`, `Set.mulDistribMulActionSet`), zero behavior (`zero_smul_set`, `smul_zero_subset`, `zero_mem_smul_iff`), nonzero scalar properties (`smul_set_inter₀`, `smul_set_sdiff₀`, `smul_set_univ₀`), membership characterizations (`smul_mem_smul_set_iff₀`, `mem_inv_smul_set_iff₀`), and no-zero-divisors instances |
| Finset.lean | Pointwise scalar multiplication on finite sets: typeclass instances (`Finset.smulZeroClass`, `Finset.distribSMul`, `Finset.distribMulAction`, `Finset.mulDistribMulAction`), zero behavior (`zero_smul_finset`, `smul_zero_subset`, `zero_mem_smul_iff`), nonzero scalar properties (`smul_finset_inter₀`, `smul_finset_sdiff₀`, `smul_finset_univ₀`), membership characterizations (`smul_mem_smul_finset_iff₀`), inverse distribution (`inv_smul_finset_distrib₀`), and finite-set-specific no-zero-divisors instances |

## Subdirectories

(none)

## Search Tags

pointwise-operations scalar-multiplication sets finite-sets group-with-zero smul-zero-class distrib-smul distrib-mul-action no-zero-smul-divisors zero-membership injective-scaling set-operations finset-operations convexity measure-theory functional-analysis
