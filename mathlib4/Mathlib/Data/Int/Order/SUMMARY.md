---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Int/Order
generated: 2025-12-09T19:30:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 3
subdirs_count: 0
---

# Order

## Overview

The `Order/` directory defines the linear order structure on integers and proves order-related properties. It establishes the `LinearOrder` instance for ℤ, provides fundamental order elimination lemmas, characterizes multiplication sign patterns, and proves specialized lemmas about natural absolute values, integer square roots, and units in the context of the order structure.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines the `LinearOrder` instance for integers; provides `le.elim` and `lt.elim` elimination lemmas; proves multiplication nonnegative iff both factors have the same sign (`Int.mul_nonneg_iff`) |
| Lemmas.lean | Additional order-related integer lemmas; characterizes natAbs equality/ordering via `a * a` comparisons; proves absolute value bounds for integer square roots |
| Units.lean | Properties of integer units (±1) interacting with order; shows units satisfy `u² = 1`, characterizes units by `abs x = 1`, proves squares less than 4 must equal 1 for nonzero integers |

## Subdirectories

None

## Search Tags

integers order linear-order multiplication-sign natabs absolute-value units square-root lattice less-than-or-equal comparison sign-pattern int-sqrt
