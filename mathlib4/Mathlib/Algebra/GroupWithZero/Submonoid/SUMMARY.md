---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/GroupWithZero/Submonoid
generated: 2025-12-01T10:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# Submonoid

## Overview

The `Submonoid/` directory provides submonoid-specific theory for monoids with zero, focusing on inheritance of cancellation properties, instance construction for homomorphism ranges, pointwise operations under group-with-zero actions, and identification of special submonoids like primal elements. These results bridge the general submonoid theory with the zero-enriched multiplicative structures of `GroupWithZero`.

## Key Files

| File | Purpose |
|------|---------|
| CancelMulZero.lean | Cancellation inheritance: proves submagmas with zero inherit left/right/full cancellation from ambient `IsLeftCancelMulZero`, `IsRightCancelMulZero`, and `IsCancelMulZero` structures via coercion injectivity |
| Instances.lean | Range submonoid instances: provides `MulZeroOneClass`, `MonoidWithZero`, `CommMonoidWithZero`, `GroupWithZero`, and `CommGroupWithZero` instances for `MonoidHom.mrange f` of a `MonoidWithZeroHom` |
| Pointwise.lean | Pointwise scalar multiplication: lemmas for `a • S` operations on submonoids/additive submonoids under `GroupWithZero` actions, including membership characterizations (`smul_mem_pointwise_smul_iff₀`), order preservation (`pointwise_smul_le_pointwise_smul_iff₀`), and interaction with inverses (requires `a ≠ 0`) |
| Primal.lean | Primal elements submonoid: defines `Submonoid.isPrimal M₀` as the submonoid of primal elements in a cancellative commutative monoid with zero, closed under multiplication and containing units |

## Subdirectories

(none)

## Search Tags

submonoid monoid-with-zero cancellation-inheritance group-with-zero pointwise-operations scalar-multiplication primal-elements homomorphism-range nonzero-divisors additive-submonoid distributed-actions
