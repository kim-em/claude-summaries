---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Group/Unbundled
generated: 2025-12-01T19:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Unbundled

## Overview

The `Unbundled/` directory contains unbundled (typeclass-based) ordered group theory, where ordering constraints are expressed as separate typeclasses (`MulLeftMono`, `MulRightMono`, `MulLeftStrictMono`, `MulRightStrictMono`) rather than bundled into the group structure. This provides fine-grained control over monotonicity assumptions and enables proving results under minimal hypotheses. The directory covers fundamental inequalities involving group inversion and division, absolute value theory in lattice ordered groups, and specialized results for integers as an ordered group.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core unbundled ordered group theory: inequalities with inverses (`a⁻¹ ≤ 1 ↔ 1 ≤ a`, `inv_le_inv_iff`), division comparisons (`div_le_iff_le_mul`), monotonicity of inversion, distinguished lemmas for left/right covariance |
| Abs.lean | Absolute value in lattice ordered groups: definition `\|a\|ₘ = a ⊔ a⁻¹`, triangle inequality, solid sets and solid closure, Birkhoff inequalities, specialized lemmas for linear orders |
| Int.lean | Integer-specific ordered group results: relationship between `abs` and `natAbs`, sign properties, divisibility bounds, modulo operations with absolute values, specialized induction principles |

## Subdirectories

(none)

## Search Tags

unbundled-ordered-groups typeclass-based-order mul-left-mono mul-right-mono mul-strict-mono covariance contravariance group-inversion-inequalities division-inequalities lattice-ordered-groups absolute-value mabs triangle-inequality solid-sets birkhoff-inequalities integer-ordered-group natabs sign-properties modulo-absolute-value
