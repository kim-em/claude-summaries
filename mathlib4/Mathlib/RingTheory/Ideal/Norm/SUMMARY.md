---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Ideal/Norm
generated: 2026-01-26T21:09:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Norm

## Overview

The `Norm/` directory defines two types of ideal norms for ring extensions. The absolute norm measures the cardinality of quotient rings as natural numbers, while the relative norm captures how ideals behave under ring extensions as ideals themselves. These constructions are fundamental for understanding the arithmetic of ideals in algebraic number theory, particularly in Dedekind domains and rings of integers.

## Key Files

| File | Purpose |
|------|---------|
| AbsNorm.lean | Absolute ideal norm `Ideal.absNorm (I : Ideal R) : ℕ` as cardinality of quotient `R ⧸ I`; proves multiplicativity, determinant formulas, and finiteness results |
| RelNorm.lean | Relative ideal norm `Ideal.relNorm R (I : Ideal S) : Ideal R` as ideal spanned by norms of elements; proves multiplicativity, transitivity, and relationship to absolute norm |

## Subdirectories

(none)

## Search Tags

ideal-norm absolute-norm relative-norm quotient-cardinality Dedekind-domain ring-extension number-theory algebra-norm determinant multiplicative-norm transitivity ring-of-integers ideal-arithmetic fractional-ideal ramification inertia Galois-extension localization prime-ideal maximal-ideal
