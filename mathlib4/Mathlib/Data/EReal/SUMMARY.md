---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/EReal
generated: 2025-12-09T15:30:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 3
subdirs_count: 0
---

# EReal

## Overview

The `EReal/` directory defines extended real numbers `[-∞, ∞]` (notation `EReal`), implemented as `WithBot (WithTop ℝ)`. It provides a complete linear order structure with both top (`⊤`) and bottom (`⊥`) elements, along with arithmetic operations (addition, negation, subtraction, multiplication, division, inverse) and auxiliary functions (absolute value, sign, toReal, toENNReal). The design makes specific choices for edge cases: `⊥ + ⊤ = ⊥`, `0 * ∞ = 0`, and `⊤⁻¹ = ⊥⁻¹ = 0`, primarily to ensure compatibility with the exponential/logarithm mapping to `ℝ≥0∞` and measure theory conventions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `EReal` as `WithBot (WithTop ℝ)`, type class instances (`CompleteLinearOrder`, `LinearOrder`, `AddCommMonoid`, etc.), coercions from `ℝ` and `ℝ≥0∞`, multiplication structure (`MulZeroOneClass`), conversion functions (`toReal`, `toENNReal`), and basic order/casting lemmas |
| Operations.lean | Addition, negation, subtraction operations on `EReal` with edge case handling (e.g., `⊥ + ⊤ = ⊥`), order properties under arithmetic operations, `SubNegZeroMonoid` instance, and distributivity lemmas (holds under non-negativity constraints) |
| Inv.lean | Absolute value function (`abs : EReal → ℝ≥0∞`), sign function (`sign : EReal → SignType`), `CommMonoidWithZero` instance (using sign/abs characterization for associativity), inversion (`⊤⁻¹ = ⊥⁻¹ = 0`), `DivInvMonoid` instance, and division operation |

## Subdirectories

(none)

## Search Tags

extended-reals ereal arithmetic infinity complete-linear-order addition multiplication negation inverse absolute-value sign coercion ennreal conversions measure-theory
