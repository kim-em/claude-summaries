---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Monoid/Canonical
generated: 2025-12-01T19:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Canonical

## Overview

The `Canonical/` directory defines **canonically ordered monoids**, where the ordering precisely corresponds to the divisibility relation (multiplicative) or subtractibility relation (additive). In these structures, `a ≤ b` if and only if there exists `c` such that `b = a * c` (or `b = a + c` additively). This is satisfied by natural numbers but not by integers or other ordered groups with negative elements. The directory establishes the core typeclasses, proves fundamental properties including that all units are trivial (equal to 1), and provides specialized lemmas for linearly ordered variants.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core typeclass definitions: `CanonicallyOrderedMul` (order ↔ divisibility), `CanonicallyOrderedAdd` (order ↔ subtractibility), plus fundamental lemmas including `one_le`, `le_iff_exists_mul`, monotonicity instances, unique units theorem, and distributivity of `min` over multiplication in linear orders |
| Basic.lean | Additional theory for canonically ordered monoids: `Finset.sup` lemmas proving that supremum equals zero iff all elements are zero (both `sup` and `sup'` variants) |

## Subdirectories

None.

## Search Tags

canonically-ordered-monoid canonically-ordered-add divisibility-order subtractibility-order exists-mul-of-le exists-add-of-le one-le zero-le unique-units finset-supremum linear-order natural-numbers bot-eq-one bot-eq-zero min-distributivity
