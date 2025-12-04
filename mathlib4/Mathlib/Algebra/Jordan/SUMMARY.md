---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Jordan
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Jordan

## Overview

This folder contains the foundational theory of Jordan rings and Jordan algebras, which are non-associative algebraic structures where multiplication is commutative (in the commutative case) and satisfies a weak associativity law called the Jordan identity: `(a * b) * a^2 = a * (b * a^2)`. The theory includes both commutative Jordan algebras (`IsCommJordan`) and the more general non-commutative Jordan algebras (`IsJordan`), with proofs that every associative algebra becomes a Jordan algebra via symmetrized multiplication, and linearization results expressing Jordan axioms as commuting multiplication operators and Lie bracket relations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and theory: `IsJordan` (non-commutative) and `IsCommJordan` (commutative) type classes capturing Jordan axioms via commuting left/right multiplication operators, instances showing semigroups satisfy Jordan axioms, formulation in terms of Lie brackets `⁅L a, L (a * a)⁆ = 0`, and linearization theorem `two_nsmul_lie_lmul_lmul_add_add_eq_zero` expressing trilinear Jordan identity |

## Subdirectories

*(none)*

## Search Tags

jordan-algebra jordan-ring non-associative commutative-jordan jordan-identity multiplication-operators lie-bracket linearization special-jordan triple-product quadratic-algebra vidav-palmer exceptional-jordan octonions symmetrized-multiplication
