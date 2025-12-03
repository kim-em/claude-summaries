---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Ring/Int
generated: 2025-12-01T19:47:30Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Int

## Overview

The `Int/` directory contains the core ring theory specific to the integers `ℤ`. This includes the commutative ring instance definition, parity properties (even/odd characterizations and lemmas), and characterization of units in the integers. These files establish `ℤ` as a foundational example of a commutative ring with additional computational and decidability properties.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core ring instances for `ℤ`: `CommRing`, `CancelCommMonoidWithZero`, `IsDomain`, `CharZero`, casting lemmas for multiplication and powers |
| Parity.lean | Parity theory for integers: odd/even characterization via `n % 2`, decidability, parity of sums/products/powers, `natAbs` parity, square properties |
| Units.lean | Units in `ℤ`: proof that the only invertible integers are 1 and -1 (`units_eq_one_or`), inequality characterizations |

## Subdirectories

(none)

## Search Tags

integers ring commutative-ring characteristic-zero parity even odd units invertible modulo casting int-cast ring-instances isdomain cancel-comm-monoid
