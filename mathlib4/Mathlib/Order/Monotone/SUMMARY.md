---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Monotone
generated: 2026-01-26T21:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 7
subdirs_count: 0
---

# Monotone

## Overview

The `Monotone/` directory contains the core formalization of monotone and antitone functions in Lean's Mathlib. It defines the fundamental concepts of monotonicity (order-preserving functions), strict monotonicity, and their antitone (order-reversing) counterparts, both globally and on subsets. The directory includes a comprehensive API for composing, reflecting, and transforming monotone functions, with specialized results for natural and integer domains, dual orders, product types, and linear orders.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of Monotone, Antitone, StrictMono, StrictAnti and their "On" variants (MonotoneOn, etc.); decidability instances; basic composition and hierarchy lemmas |
| Basic.lean | Extensive API for monotone functions: dual order transformations, well-foundedness propagation, monotonicity in linear orders with reflection lemmas, product and Pi type operations, cmp preservation, ℕ/ℤ-specific theorems (monotone_nat_of_le_succ, etc.) |
| Extension.lean | Monotone extension theorem: bounded monotone functions on a set admit monotone extensions to the whole space in conditionally complete linear orders |
| Monovary.lean | Monovariance: functions that "vary together" (if g i < g j then f i ≤ f j) without requiring an order on the index type; used in rearrangement inequalities |
| MonovaryOrder.lean | Constructs a linear order on the index type that makes monovarying functions simultaneously monotone; proves equivalence between monovariance and existence of compatible order |
| Odd.lean | Monotonicity of odd functions: proves that odd functions (f(-x) = -f(x)) on ordered groups are monotone globally if monotone on non-negative elements |
| Union.lean | Monotonicity on unions: deduces global monotonicity from monotonicity on (-∞, a] and [a, ∞); general union lemmas for monotonicity |

## Subdirectories

(none)

## Search Tags

monotone antitone strictly-monotone strictly-antitone increasing decreasing order-preserving order-reversing function-monotonicity composition reflection dual-order product-order Pi-type monovary antivary extension odd-function linear-order natural-numbers integers
