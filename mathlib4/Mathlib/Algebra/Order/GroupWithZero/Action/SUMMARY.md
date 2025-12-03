---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/GroupWithZero/Action
generated: 2025-12-01T08:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# Action

## Overview

The `Action/` directory transfers group action with zero instances to order type synonyms `αᵒᵈ` (order dual) and `Lex α` (lexicographic order). This provides the infrastructure for actions by and on ordered structures with zero, complementing the scalar multiplication instances already defined in the group action hierarchy. The main file provides instances for `SMulWithZero`, `DistribSMul`, `DistribMulAction`, and `MulActionWithZero` for both order dual and lexicographic order synonyms.

## Key Files

| File | Purpose |
|------|---------|
| Synonym.lean | Transfer of group action with zero instances from type `α` to order synonyms: `OrderDual` instances for `SMulWithZero`, `DistribSMul`, `DistribMulAction`, and `MulActionWithZero` on `G₀ᵒᵈ` and `M₀ᵒᵈ`; `Lex` instances for the same typeclasses on `Lex G₀` and `Lex M₀`; all instances simply transfer the underlying structure using `‹...›` |

## Subdirectories

None.

## Search Tags

group-action-with-zero order-synonym order-dual lexicographic-order smul-with-zero distrib-smul distrib-mul-action mul-action-with-zero instance-transfer typeclass-synonym
