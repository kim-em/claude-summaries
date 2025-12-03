---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/GroupWithZero/Pointwise/Set
generated: 2025-12-01T17:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Set

## Overview

The `Set/` directory provides the theory of pointwise operations on sets (as opposed to finite sets) in groups with zero. This extends general pointwise set operations to handle zero-specific behavior, proving how multiplication and division by zero collapse to the zero set for nonempty sets, and establishing cardinality preservation for scalar multiplication by nonzero elements.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Basic properties of pointwise operations on sets in groups with zero: multiplication/division by zero behavior (s * 0 = 0, s / 0 = 0, 0 * s = 0, 0 / s = 0 for nonempty s), subset relations for zero operations, and inverse of zero set |
| Card.lean | Cardinality results for scalar multiplication by nonzero elements: Cardinal.mk_smul_set₀ and natCard_smul_set₀ showing that scalar multiplication by a ≠ 0 preserves set cardinality via injectivity |

## Subdirectories

None

## Search Tags

pointwise-operations set-operations group-with-zero zero-multiplication zero-division cardinality scalar-multiplication nonzero-scalars set-theory cardinal
