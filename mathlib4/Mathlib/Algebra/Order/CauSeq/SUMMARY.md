---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/CauSeq
generated: 2025-12-01T12:21:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# CauSeq

## Overview

The `CauSeq/` directory provides a concrete implementation of Cauchy sequences for ordered fields with absolute values, serving as the foundation for constructing completions of rings (particularly ℝ and p-adic numbers). It defines the `IsCauSeq` predicate and `CauSeq` type, proves fundamental algebraic operations preserve the Cauchy property, and constructs the Cauchy completion as a quotient by the equivalence relation of limit-zero differences. This is a computational alternative to the more abstract Cauchy filter approach from topology.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core Cauchy sequence theory: `IsCauSeq` predicate, `CauSeq` type with algebraic structure (ring/module/algebra instances), equivalence relations, continuity lemmas for addition/multiplication/inversion, boundedness results, and convergence criteria |
| BigOperators.lean | Cauchy sequences involving finite sums: convergence of partial sums from term-wise bounds (`of_abv_le`/`of_abv`), Cauchy product formula for multiplying series, bounded monotone/decreasing sequence convergence (Archimedean), geometric series convergence, ratio test for series convergence |
| Completion.lean | Cauchy completion construction: quotient type `Cauchy abv := CauSeq / equiv`, ring/field/division ring instances via `ofRat` embedding, arithmetic operations on completion (`mk_add`, `mk_mul`, etc.), scalar multiplication, and cast operations for ℕ/ℤ/ℚ |

## Subdirectories

*(none)*

## Search Tags

cauchy-sequences absolute-value ordered-fields completion real-numbers p-adic concrete-implementation series-convergence geometric-series ratio-test cauchy-product partial-sums quotient-construction ring-completion
